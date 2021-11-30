# Predictive Uncertainty
Estimating the uncertainty of deep learning models has gained exponential interest recent years, mainly due to the safty concerns for real applications. 
In this Arxiv, latest literature from NIPS, ICML, ICLR, etc will be covered (on-updating). some papers may be included multiple times if they cover across topics.

## Survey:
- [[Information Fusion 2021] A review of uncertainty quantification in deep learning: Techniques, applications and challenges](https://www.sciencedirect.com/science/article/pii/S1566253521001081)
![image](https://user-images.githubusercontent.com/26398708/143864354-de4a2e38-fc8a-4095-9056-52f0e74ca710.png)
- [[arXiv2020] A Survey of Uncertainty in Deep Neural Networks](https://arxiv.org/abs/2107.03342)
![image](https://user-images.githubusercontent.com/26398708/143865096-85099b9f-723c-4fb0-bba7-b679bb5f107b.png)
- [[AIES2021] Uncertainty as a form of transparency: Measuring, communicating, and using uncertainty](https://dl.acm.org/doi/abs/10.1145/3461702.3462571)
- [[arXiv2020] A Survey on Assessing the Generalization Envelope of Deep Neural Networks](https://arxiv.org/abs/2008.09381)
- [[arXiv2021] A Unified Survey on Anomaly, Novelty, Open-Set, and Out-of-Distribution Detection: Solutions and Future Challenges](https://arxiv.org/abs/2110.14051)
- [[NeurIPS2020] Tutorial: (Track2) Practical Uncertainty Estimation and Out-of-Distribution Robustness in Deep Learning](https://nips.cc/virtual/2020/public/tutorial_0f190e6e164eafe66f011073b4486975.html)
- [[NeurIPS2021] Workshop: Bayesian Deep Learning](http://bayesiandeeplearning.org/)

## Dataset and Benchmarking:
- [[NeurIPS2019] Can you trust your model's uncertainty? Evaluating predictive uncertainty under dataset shift](https://proceedings.neurips.cc/paper/2019/hash/8558cb408c1d76621371888657d2eb1d-Abstract.html)

- [[ICLR2019] Benchmarking neural network robustness to common corruptions and perturbations](https://openreview.net/forum?id=HJz6tiCqYm)

- [[NeurIPS2021] Benchmarking Bayesian Deep Learning on Diabetic Retinopathy Detection Tasks](https://openreview.net/forum?id=jyd4Lyjr2iB)

## Bayesian Deep Learning:
- [[ICML2016] Dropout as a Bayesian Approximation: Representing Model Uncertainty in Deep Learning (MCDropout)](http://proceedings.mlr.press/v48/gal16.html)
- [[NeurIPS2019] A simple baseline for bayesian uncertainty in deep learning (SWAG)](https://proceedings.neurips.cc/paper/2019/file/118921efba23fc329e6560b27861f0c2-Paper.pdf)
- [[NeurIPS2020] Simple and Principled Uncertainty Estimation with Deterministic Deep Learning via Distance Awareness](https://proceedings.neurips.cc/paper/2020/hash/543e83748234f7cbab21aa0ade66565f-Abstract.html)
- [[NeurIPS2018] Predictive Uncertainty Estimation via Prior Networks](https://proceedings.neurips.cc/paper/2018/hash/3ea2db50e62ceefceaf70a9d9a56a6f4-Abstract.html)
- [[NeurIPS2020] Posterior Network: Uncertainty Estimation without OOD Samples via Density-Based Pseudo-Counts](https://proceedings.neurips.cc/paper/2020/hash/0eac690d7059a8de4b48e90f14510391-Abstract.html)
- [[NeurIPS2020] Liberty or Depth: Deep Bayesian Neural Nets Do Not Need Complex Weight Posterior Approximations](https://proceedings.neurips.cc/paper/2020/hash/2dfe1946b3003933b7f8ddd71f24dbb1-Abstract.html)
- [[NeurIPS2020] Posterior Re-calibration for Imbalanced Datasets](https://proceedings.neurips.cc/paper/2020/hash/5ca359ab1e9e3b9c478459944a2d9ca5-Abstract.html)

### Confidence:
- [[NeurIPS2018] To Trust Or Not To Trust A Classifier (Trust Score)](https://openreview.net/forum?id=HkZFuPbubr)
- [[NeurIPS2019] Addressing Failure Prediction by Learning Model Confidence (ConfidNet)](https://papers.nips.cc/paper/2019/hash/757f843a169cc678064d9530d12a1881-Abstract.html)
- [[NeurIPS2019] Accurate Layerwise Interpretable Competence Estimation (ALICE)](https://proceedings.neurips.cc/paper/2019/hash/a11da6bd58b95b334f8cd49f00918f16-Abstract.html)
- [[ICML2020] Confidence-Aware Learning for Deep Neural Networks (Correctness Ranking Loss)](http://proceedings.mlr.press/v119/moon20a.html)


### Ensemble:
- [[NeurIPS2017] Simple and Scalable Predictive Uncertainty
Estimation using Deep Ensembles](https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf)
- [[NeurIPS2019] Accurate Uncertainty Estimation and Decomposition in Ensemble Learning](https://proceedings.neurips.cc/paper/2019/hash/1cc8a8ea51cd0adddf5dab504a285915-Abstract.html)
- [[ICLR2021] Training independent subnetworks for robust prediction (MIMO)](https://openreview.net/forum?id=OGg9XnKxFAH)

### Calibration:
 - [[ICML2017] On calibration of modern neural networks (T-Scaling)](http://proceedings.mlr.press/v70/guo17a.html)
 - [[NeurIPS2019] Verified Uncertainty Calibration](https://openreview.net/forum?id=rkxluVHeLB)
 - [[NeurIPS2020] Improving model calibration with accuracy versus uncertainty optimization](https://proceedings.neurips.cc/paper/2020/hash/d3d9446802a44259755d38e6d163e820-Abstract.html)
 - [[ICML2020] Mix-n-match: Ensemble and compositional methods for uncertainty calibration in deep learning](http://proceedings.mlr.press/v119/zhang20k.html)

### Gradient method:
- [[NeurIPS2019] A simple baseline for bayesian uncertainty in deep learning (SWAG)](https://proceedings.neurips.cc/paper/2019/file/118921efba23fc329e6560b27861f0c2-Paper.pdf)
- [[NeurIPS2021] On the Importance of Gradients for Detecting Distributional Shifts in the Wild (GradNorm)](https://proceedings.neurips.cc/paper/2021/hash/0607f4c705595b911a4f3e7a127b44e0-Abstract.html)



## Out-of-distribution Detection: 
### Emperical and theoretical:
 - [[NeurIPS2020] Why Normalizing Flows Fail to Detect Out-of-Distribution Data](https://proceedings.neurips.cc/paper/2020/hash/ecb9fe2fbb99c31f567e9823e884dbec-Abstract.html)
 - [[NeurIPS2020] On the Value of Out-of-Distribution Testing: An Example of Goodhart's Law](https://proceedings.neurips.cc/paper/2020/hash/045117b0e0a11a242b9765e79cbf113f-Abstract.html)
 - [[NeurIPS2021] Exploring the Limits of Out-of-Distribution Detection](https://proceedings.neurips.cc/paper/2021/hash/3941c4358616274ac2436eacf67fae05-Abstract.html)
 - [[NeurIPS2021] A Winning Hand: Compressing Deep Networks Can Improve Out-of-Distribution Robustness](https://proceedings.neurips.cc/paper/2021/hash/0607f4c705595b911a4f3e7a127b44e0-Abstract.html)

 
### OOD detection:
#### Without exposure:
- [[ICIR2017] A Baseline for Detecting Misclassified and Out-of-Distribution Examples in Neural Networks (Softmax)](https://openreview.net/forum?id=Hkg4TI9xl)
- [[NeurIPS2020] Certifiably Adversarially Robust Detection of Out-of-Distribution Data](https://proceedings.neurips.cc/paper/2020/hash/b90c46963248e6d7aab1e0f429743ca0-Abstract.html)
- [[NeurIPS2021] On the Importance of Gradients for Detecting Distributional Shifts in the Wild (GradNorm)](https://proceedings.neurips.cc/paper/2021/hash/0607f4c705595b911a4f3e7a127b44e0-Abstract.html)
- [[NeurIPS2021] ReAct: Out-of-distribution Detection With Rectified Activations](https://proceedings.neurips.cc/paper/2021/hash/01894d6f048493d2cacde3c579c315a3-Abstract.html)
- [[NeurIPS2021] Single Layer Predictive Normalized Maximum Likelihood for Out-of-Distribution Detection](https://proceedings.neurips.cc/paper/2021/hash/093b60fd0557804c8ba0cbf1453da22f-Abstract.html)
- [[NeurIPS2021] 
Learning Causal Semantic Representation for Out-of-Distribution Prediction](https://proceedings.neurips.cc/paper/2021/hash/310614fca8fb8e5491295336298c340f-Abstract.html)
- [[NeurIPS2021] STEP: Out-of-Distribution Detection in the Presence of Limited In-Distribution Labeled Data](https://proceedings.neurips.cc/paper/2021/hash/f4334c131c781e2a6f0a5e34814c8147-Abstract.html)
- [[NeurIPS2021] Task-Agnostic Undesirable Feature Deactivation Using Out-of-Distribution Data](https://proceedings.neurips.cc/paper/2021/hash/21186d7b1482412ab14f0332b8aee119-Abstract.html)


##### Generative model:
- [[NeurIPS2019] Likelihood Ratios for Out-of-Distribution Detection](https://proceedings.neurips.cc/paper/2019/hash/1e79596878b2320cac26dd792a6c51c9-Abstract.html)
- [[NeurIPS2020] Likelihood Regret: An Out-of-Distribution Detection Score For Variational Auto-encoder](https://proceedings.neurips.cc/paper/2020/hash/eddea82ad2755b24c4e168c5fc2ebd40-Abstract.html)
- [[NeurIPS2021] Locally Most Powerful Bayesian Test for Out-of-Distribution Detection using Deep Generative Models](https://proceedings.neurips.cc/paper/2021/hash/7d3e28d14440d6c07f73b7557e3d9602-Abstract.html)
- 

#### With exposure:
- [[NeurIPS2020] Towards Maximizing the Representation Gap between In-Domain & Out-of-Distribution Examples](https://proceedings.neurips.cc/paper/2020/hash/68d3743587f71fbaa5062152985aff40-Abstract.html)
- [[NeurIPS2020] OOD-MAML: Meta-Learning for Few-Shot Out-of-Distribution Detection and Classification](https://proceedings.neurips.cc/paper/2020/hash/28e209b61a52482a0ae1cb9f5959c792-Abstract.html)

#### OOD generalization:
- [[NeurIPS2021] On the Out-of-distribution Generalization of Probabilistic Image Modelling](https://proceedings.neurips.cc/paper/2021/hash/1f88c7c5d7d94ae08bd752aa3d82108b-Abstract.html)
- [[NeurIPS2021] Characterizing Generalization under Out-Of-Distribution Shifts in Deep Metric Learning](https://proceedings.neurips.cc/paper/2021/hash/d1f255a373a3cef72e03aa9d980c7eca-Abstract.html)
- [[NeurIPS2021] Towards a Theoretical Framework of Out-of-Distribution Generalization](https://proceedings.neurips.cc/paper/2021/hash/c5c1cb0bebd56ae38817b251ad72bedb-Abstract.html)



## Non-parametric Gaussian Process:
 - [[NeurIPS2020]Simple and Principled Uncertainty Estimation with Deterministic Deep Learning via Distance Awareness](https://papers.nips.cc/paper/2020/file/543e83748234f7cbab21aa0ade66565f-Paper.pdf)
 - 

