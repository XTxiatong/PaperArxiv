
## ECG datasets
https://arxiv.org/pdf/2405.17766

## wearable ECG
https://arxiv.org/abs/2406.18069

[JBHI-2024] Large Language Models for Cuffless Blood Pressure Measurement From Wearable Biosignals 
- https://arxiv.org/pdf/2406.18069
- 深圳大学&华为&CityU
- 1272的公开数据
- 
[ISWC-2021] A Transformer Architecture for Stress Detection from ECG
- https://dl.acm.org/doi/abs/10.1145/3460421.3480427
- Ali Etemad
- Data: WESAD and SWELL-KW, for stress detection

[CinC24] Cross-Modal Attention Fusion of Electrocardiogram Emotion and Voiceprint for Depression Detection
- https://cinc.org/2024/Program/accepted/183_Preprint.pdf
- Data: WESAD and SWELL-KW, for stress detection

[Cinc24] Prediction of Sex From a 12-lead ECG Using Deep Learning: External Validation and Interpretation
- https://cinc.org/2024/Program/accepted/288_Preprint.pdf
- Seliency map to higight the features for sex prediction
- Conclusion: this is not for clinical used, but demonstrate ECG contain rich information for profile

  
## ECG foundaiton models
[arxiv23] Scaling Representation Learning from Ubiquitous ECG with State-Space Models
  - Architecture: State-space models: S4
  - Loss: Signal Transformations based SSL
  - Data: Pretraining: TILES 2018 dataset public (bioshirt),  AVEC-16, SWELL-KW,  WESAD + PTB-XL, LUDB, CASE
  - Code: [github](https://github.com/klean2050/tiles_ecg_model)

[arxiv24] Foundation models for ECG  [link](https://arxiv.org/pdf/2407.07110)
  - Architecture: CNN + ViT
  - Method: Contrastive, Generative, Hybrid
  - Data: Pretraining: MIMIC, CODE15, UK Biobank, SAMI, IKEM; test: PTB-XL 
  - Code: not found

[ICLR'24] GUIDING MASKED REPRESENTATION LEARNING TO CAPTURE SPATIO-TEMPORAL RELATIONSHIP OF ELECTROCARDIOGRAM
- https://openreview.net/forum?id=WcOohbsF4H
- 
[ICLR'25] Reading Your Heart: Learning ECG Words and Sentences via Pre-training ECG Language Model
- [paper](https://openreview.net/forum?id=6Hz1Ko087B) ICLR 高分
- 北大的
- learning token-level representation for QRS


## ECG generation
[KDD workshop'24] Multi-Channel Masked Autoencoder and Comprehensive Evaluations for Reconstructing 12-Lead ECG from Arbitrary Single-Lead ECG
- https://arxiv.org/pdf/2407.11481
- https://github.com/CHENJIAR3/MCMA

## Report generation
[MIDL22] Learning to automatically generate accurate ECG captions
  - Architecture: ECG encoder + **transformer**
  - Loss: report text cross entropy
  - Novelty: using diagnosie label for cross-modality learing
  - Data: private UMCU
  - Code: adapted from [ACL 2018](https://arxiv.org/abs/1711.08195) [Github](https://github.com/havecats/Medical-Report-Generation-OntheAutomaticGeneration?tab=readme-ov-file)

[medRxiv23, University of Sydney] Biosignal copilot: Leveraging the power of LLMs in drafting reports for biomedical signals
  - Architecture: ECG features from **NeruKit + LLMs**
  - Loss: Using pormot and buffer, no training
  - Note: big framework but only used ECG for experiments
  - Data: TNMG public
  - Code: [github](https://github.com/NeuroSyd/signal_copilot)

[ML4H23, Akane, Rice] Zero-shot ECG Diagnosis with Large Language Models and Retrieval-augmented Generation
  - Architecture: ECG **features + LLMs**, construct database of domain knowledge, **RAG**
  - Loss: Using pormot no training
  - Note: big framework but only used ECG for experiments
  - Data: PTB-XL+ (five arrhythmia), Apena-ECG (presence of apnea)

[EACL23, CMU] Transfer Knowledge from Natural Language to Electrocardiography: Can We Detect Cardiovascular Disease Through Language Models?  
  - Architecture: Encoder (ECG + ECG features), Decoder (**LLMs**) 
  - Loss: No promot, report generation loss
  - Note: Trained with report generation, test with both report generation and zero-shot disease diganosis (**how ?**)
  - Data: PTB-XL (report + five conditions), 
  - Takeaway: For **ECG Encoder, transformer > Resnet** > LSTM > MLP; For text decoder, BioClinical BEART is good

[MIDL23, Shenda Hong from PKU, Rossella and Che Liu from IC] Frozen Lauguage Models Healps ECG Zero-Shot Learning
[ICASSP24, Rossella] ETP: Learning Transferable ECG Representations via ECG-Text Pre-traning
  - Architecture: ECG Encoder + LLM Decoder in a constrastive way, 
  - Loss: **CLIP** loss with ECG reports
  - Note: Trained with report, test with both report and zero-shot disease diganosis
  - Data: PTB-XL (report + five conditions),  MIT-BIH, CPSC 
  - Takeaway 1: This is good training for reports and tests related to diagnosis. *Reports and labels have similarities*, but how can we reverse this?
  - Takeaway 2: Another anagle to think about this work: we can use LLM to train better encoders,  signal embedding align with text high-level embeddings

[ICML'24, Che Liu from IC] MERL: Zero-Shot ECG Classification with Multimodal Learning and Test-time Clinical Knowledge Enhancement
  - Architecture: ECG Encoder  + LLM Ecnoder constrastive,  expert-konwledge database
  - Loss: Duaring training, reports are used. At test time, customer-rpovided knowledge enhanced.
  - Note: Trained with report, test for zero-shot disease diganosis
  - Data: PTB-XL (report + five conditions), CPSC, CSN
  - Takeaway: This is good training for reports and tests related to diagnosis. *Reports and labels have similarities*, but how can we reverse this?
  - Problem: I agree this allows disease level inferene without disease labels, and it outperms linear probe (10%) -- is 10% reasonable, why not more? 

    
[arXiv'24, Che Liu from IC, Mi Zhang from Ohio] MEIT：Multi-model ECG Instruction tuning on LLM for report generaiton [paper](https://arxiv.org/pdf/2403.04945)
  - Architecture: ECG Encoder + LLM Decoder + promt,  cross-modal attention for alignment
  - Loss: **Instruction tuning, Lora**
  - Note: Trained with report, test with in-domian and new-domian (**zero-shot**) report generation, robust with signal pertubartion
  - Data: PTB-XL, MIMIC-I V-ECG, continenst are different
  - Takeaway: The framework of multi-model LLMs works without instruction tuning, but IT imporves about 5% (not very significant).
  - Porblem: General baseline without LLM is missing, **how good compred to MIDL22**?
  - Performance: PTB-XL BLEU1 0.5ish, F1 0.7ish 

[Neurips'23 workshop] JoLT: Jointly Learned Representations of Language and Time-Series
  - Architecture: ECG Encoder + Qformer + LLM Decoder  
  - Data: PTB-XL (4.46 uncomfirmed report)
  - comparable Meteor to my experiment
  - [paper](https://openreview.net/pdf?id=UVF1AMBj9u)

 [arXiv'24] ECG-Chat: A Large ECG-Language Model for Cardiac Disease Diagnosis
  - Architecture: ECG Encoder + LLM Decoder  
  - Note: ECG pretrained with text
  - Data: PTB-XL, MIMIC-I V-ECG

## ECG-LLM
[arXiv'24]ECG-LM: Understanding Electrocardiogram with Large Language Model
   - Tsinghua AIR
   - PTBXL
   - [paper](https://spj.science.org/doi/pdf/10.34133/hds.0221)
[npj Cardiovascular Health'24] Multi-channel masked autoencoder and conprehensive evlautions for reconsutructing 12-lead ECG from arbitary single-lead ECG


