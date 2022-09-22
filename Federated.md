## Survey and benckmarks
- [FedEval: A Benchmark System with a Comprehensive Evaluation Model for Federated Learning](https://arxiv.org/pdf/2011.09655.pdf)
- 


## Deterministics
- [ICML2022 Spotlight] [On the Practicality of Deterministic Epistemic Uncertainty](https://proceedings.mlr.press/v162/postels22a/postels22a.pdf)
  - Performance of detecting correct/incorrect predictions
  <img src="https://user-images.githubusercontent.com/26398708/187662495-f691e79a-e6dd-4c57-beba-cc2f3ae3025c.png" width="400">
  
  - uncertainty with increasing data shift
 <img src="https://user-images.githubusercontent.com/26398708/187662750-036eb3ca-b4db-424b-ae87-b6e6cfabba8a.png" width="400">

## Mix
- [Approaches to Uncertainty Quantification in Federated Deep Learning](https://pdfl.iais.fraunhofer.de/preprints/PDFL_2.pdf)


## Bayesian/Personalisation 
- [NeurIPS2020][citation 200+][Personalized federated learning with moreau envelopes](https://proceedings.neurips.cc/paper/2020/hash/f4f1f13c8289ac1b1ee0ff176b56fc60-Abstract.html)
- [ICML2022] [Personalized Federated Learning via Variational Bayesian Inference](https://proceedings.mlr.press/v162/zhang22o/zhang22o.pdf)
  -   FegAvg is applied on Bayesian neural networks, but uncertainty is not well studied. 
  -   Non-IID setting, each client owns 5/10 classes. 
        <!--<img src="https://user-images.githubusercontent.com/26398708/188150594-7d76df5f-f83e-4622-a61e-df130567ce40.png" width="200">-->
  
  
<img src="https://user-images.githubusercontent.com/26398708/186911075-2c1d2632-2fab-44f0-8709-3391a5e7d73e.png" width="300">

  
- [ICML2022][Federated Learning with Label Distribution Skew via Logits Calibration](https://proceedings.mlr.press/v162/zhang22p.html)
- 

## Ensembles
  - [NeurIPS2020][Ensemble Distillation for Robust Model Fusion in Federated Learning](https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf)
  - [UAI2022][Self-Distribution Distillation: Efficient Uncertainty Estimation](https://openreview.net/forum?id=rhNgEI8s5xc)
  - [ICLR2021][FedBE: Making Bayesian Model Ensemble Applicable to Federated Learning](https://openreview.net/forum?id=dgtpE6gKjHn)

## Prototype:
 - [AAAI2022][Fedproto: Federated prototype learning across heterogeneous clients](https://arxiv.org/abs/2104.01893)
    - A regularization term to approach local prototype to the global one is reuired. Otherwise, it is hard to gurantte they are in the same feature space. 


## Generativ model and federated learning:
  - [AAAI2020] [Uncertainty-Aware Deep Classifiers Using Generative Models](https://ojs.aaai.org/index.php/AAAI/article/view/6015)


## For health
  - [Nature Medicine 2021] [Federated learning for predicting clinical outcomes in patients with COVID-19](https://www.nature.com/articles/s41591-021-01506-3)
  -
