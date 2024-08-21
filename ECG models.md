
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

[EACL23, CMU]Transfer Knowledge from Natural Language to Electrocardiography: Can We Detect Cardiovascular Disease Through Language Models?  
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

    
[arXiv'24, Che Liu from IC, Mi Zhang from Ohio] MEIT：Multi-model ECG Instruction tuning on LLM for report generaiton
  - Architecture: ECG Encoder + LLM Decoder + promt,  cross-modal attention for alignment
  - Loss: **Instruction tuning, Lora**
  - Note: Trained with report, test with in-domian and new-domian (**zero-shot**) report generation, robust with signal pertubartion
  - Data: PTB-XL, MIMIC-I V-ECG, continenst are different
  - Takeaway: The framework of multi-model LLMs works without instruction tuning, but IT imporves about 5% (not very significant).
  - Porblem: General baseline without LLM is missing, **how good compred to MIDL22**?
