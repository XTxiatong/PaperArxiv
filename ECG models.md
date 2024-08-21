
## Report generation

[MIDL22] Learning to automatically generate accurate ECG captions
  - Architecture: ECG encoder + transformer
  - Loss: report text cross entropy
  - Novelty: using diagnosie label for cross-modality learing
  - Data: private UMCU
  - Code: adapted from [ACL 2018](https://arxiv.org/abs/1711.08195) [Github](https://github.com/havecats/Medical-Report-Generation-OntheAutomaticGeneration?tab=readme-ov-file)

[medRxiv] Biosignal copilot: Leveraging the power of LLMs in drafting reports for biomedical signals
  - Architecture: ECG features from NeruKIt + LLMs
  - Loss: Using pormot and buffer, not training
  - Note: big framework but only used ECG for experiments
  - Data: TNMG
  - Code: [github](https://github.com/NeuroSyd/signal_copilot)

  - 
