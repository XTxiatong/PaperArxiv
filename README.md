# Predictive Uncertainty
Estimating the uncertainty of deep learning models has gained exponential interest recent years, mainly due to the safty concerns for real applications. 
In this Arxiv, latest literature from NIPS, ICML, ICLR, etc will be covered (on-updating). some papers may be included multiple times if they cover across topics.

## Survey:
- [[Information Fusion 2021] A review of uncertainty quantification in deep learning: Techniques, applications and challenges](https://www.sciencedirect.com/science/article/pii/S1566253521001081)
![image](https://user-images.githubusercontent.com/26398708/143864354-de4a2e38-fc8a-4095-9056-52f0e74ca710.png)
- [[arXiv2020] A Survey of Uncertainty in Deep Neural Networks](https://arxiv.org/abs/2107.03342)
![image](https://user-images.githubusercontent.com/26398708/143865096-85099b9f-723c-4fb0-bba7-b679bb5f107b.png)
- [[ACM Computing Surveys 2020] A Survey on Bayesian Deep Learning](http://wanghao.in/paper/CSUR20_BDL.pdf) ([github](https://github.com/js05212/BayesianDeepLearning-Survey))
  - application: [KDD 2021 Quantifying Uncertainty in Deep Spatiotemporal Forecasting](https://arxiv.org/pdf/2105.11982.pdf)
- [[ACM Computing Surveys] A survey on concept drift adaptation (citation 2K+)](https://dl.acm.org/doi/abs/10.1145/2523813)
- [[AIES2021] Uncertainty as a form of transparency: Measuring, communicating, and using uncertainty](https://dl.acm.org/doi/abs/10.1145/3461702.3462571)
- [[arXiv2020] A Survey on Assessing the Generalization Envelope of Deep Neural Networks](https://arxiv.org/abs/2008.09381)
- [[arXiv2021] A Unified Survey on Anomaly, Novelty, Open-Set, and Out-of-Distribution Detection: Solutions and Future Challenges](https://arxiv.org/abs/2110.14051)
- [[NeurIPS2020] Tutorial: (Track2) Practical Uncertainty Estimation and Out-of-Distribution Robustness in Deep Learning](https://nips.cc/virtual/2020/public/tutorial_0f190e6e164eafe66f011073b4486975.html)
- [[NeurIPS2021] Workshop: Bayesian Deep Learning](http://bayesiandeeplearning.org/)
- [[NeurPS2021] Workshop: Distribution shifts: connecting methods and applications (DistShift)](https://nips.cc/virtual/2021/workshop/21859)
- [I Can’t Believe It’s Not Better! (ICBINB) Workshop](https://i-cant-believe-its-not-better.github.io/)
- [[A Survey on Evidential Deep Learning For Single-Pass Uncertainty Estimation](https://arxiv.org/pdf/2110.03051.pdf)]

## Dataset and Benchmarking:
- [[NeurIPS2019] Can you trust your model's uncertainty? Evaluating predictive uncertainty under dataset shift](https://proceedings.neurips.cc/paper/2019/hash/8558cb408c1d76621371888657d2eb1d-Abstract.html)
- [[ICLR2019] Benchmarking neural network robustness to common corruptions and perturbations](https://openreview.net/forum?id=HJz6tiCqYm)
- [[NeurIPS2021] Benchmarking Bayesian Deep Learning on Diabetic Retinopathy Detection Tasks](https://openreview.net/forum?id=jyd4Lyjr2iB)
- [[NeurIPS2021]Reliable and Trustworthy Machine Learning for Health Using Dataset Shift Detection](https://proceedings.neurips.cc/paper/2021/hash/17e23e50bedc63b4095e3d8204ce063b-Abstract.html)
 - [[ICML2021]Evaluating Robustness of Predictive Uncertainty Estimation: Are Dirichlet-based Models Reliable?](http://proceedings.mlr.press/v139/kopetzki21a/kopetzki21a.pdf)
   - Openreview from [ICLR](https://openreview.net/forum?id=uRKqXoN-Ic9) 
 - [[IJCAI2019]Statistical Guarantees for the Robustness of Bayesian Neural Networks (Robustness measurement)](https://www.ijcai.org/proceedings/2019/0789.pdf)


## Uncertainty Quantificatoin:
- [[ICML2016] Dropout as a Bayesian Approximation: Representing Model Uncertainty in Deep Learning (MCDropout)](http://proceedings.mlr.press/v48/gal16.html)
- [[NeurIPS2019] A simple baseline for bayesian uncertainty in deep learning (SWAG)](https://proceedings.neurips.cc/paper/2019/file/118921efba23fc329e6560b27861f0c2-Paper.pdf)
  - [[Video and codes](https://www.youtube.com/watch?v=5WOj_ZZJ2wM)]
  - [[UAI2018] Averaging Weights Leads to Wider Optima and Better Generalization(SWA)](http://auai.org/uai2018/proceedings/papers/313.pdf)
  - [[PDFL Workshop 2021] Approaches to Uncertainty Quantification in Federated Deep Learning (Federated SWAG)](https://pdfl.iais.fraunhofer.de/preprints/PDFL_2.pdf)
- [[NeurIPS2019]Using Self-Supervised Learning Can Improve Model Robustness and Uncertainty](https://arxiv.org/pdf/1906.12340.pdf)
- [[NeurIPS2020] Simple and Principled Uncertainty Estimation with Deterministic Deep Learning via Distance Awareness](https://proceedings.neurips.cc/paper/2020/hash/543e83748234f7cbab21aa0ade66565f-Abstract.html)
- [[NeurIPS2020] Liberty or Depth: Deep Bayesian Neural Nets Do Not Need Complex Weight Posterior Approximations](https://proceedings.neurips.cc/paper/2020/hash/2dfe1946b3003933b7f8ddd71f24dbb1-Abstract.html)
- [[NeurIPS2020] Posterior Re-calibration for Imbalanced Datasets](https://proceedings.neurips.cc/paper/2020/hash/5ca359ab1e9e3b9c478459944a2d9ca5-Abstract.html)
- [[ICLR2020] Your classifier is secretly an energy based model and you should treat it like one](https://openreview.net/forum?id=Hkxzx0NtDB&utm_campaign=piqcy&utm_medium=email&utm_source=Revue%20newsletter)
- 
### Confidence (Representation learning-based):
- [[NeurIPS2018] To Trust Or Not To Trust A Classifier (Trust Score)](https://openreview.net/forum?id=HkZFuPbubr)
- [[ICLR2018] Training Confidence-calibrated Classifiers for Detecting Out-of-Distribution Samples (uniform distribution)](https://openreview.net/forum?id=ryiAv2xAZ)
- [[NeurIPS2019] Addressing Failure Prediction by Learning Model Confidence (ConfidNet)](https://papers.nips.cc/paper/2019/hash/757f843a169cc678064d9530d12a1881-Abstract.html)
- [[NeurIPS2019] Accurate Layerwise Interpretable Competence Estimation (ALICE)](https://proceedings.neurips.cc/paper/2019/hash/a11da6bd58b95b334f8cd49f00918f16-Abstract.html)
- [[ICML2020] Confidence-Aware Learning for Deep Neural Networks (Correctness Ranking Loss)](http://proceedings.mlr.press/v119/moon20a.html)


### Ensemble:
- [[NeurIPS2017] Simple and Scalable Predictive Uncertainty
Estimation using Deep Ensembles](https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf)
- [[NeurIPS2019] Accurate Uncertainty Estimation and Decomposition in Ensemble Learning](https://proceedings.neurips.cc/paper/2019/hash/1cc8a8ea51cd0adddf5dab504a285915-Abstract.html)
- [[ICLR2021] Training independent subnetworks for robust prediction (MIMO)](https://openreview.net/forum?id=OGg9XnKxFAH)
- [[NeurIPS2021] Scaling Ensemble Distribution Distillation to Many Classes with Proxy Targets (A Malinin and M Gales, Ensemble+Dirichlet)](https://proceedings.neurips.cc/paper/2021/hash/2f4ccb0f7a84f335affb418aee08a6df-Abstract.html)

### Calibration:
 - [[ICML2017] On calibration of modern neural networks (T-Scaling)](http://proceedings.mlr.press/v70/guo17a.html)
 - [[NeurIPS2019] Verified Uncertainty Calibration](https://openreview.net/forum?id=rkxluVHeLB)
 - [[NeurIPS2020] Improving model calibration with accuracy versus uncertainty optimization](https://proceedings.neurips.cc/paper/2020/hash/d3d9446802a44259755d38e6d163e820-Abstract.html)
 - [[ICML2020] Mix-n-match: Ensemble and compositional methods for uncertainty calibration in deep learning](http://proceedings.mlr.press/v119/zhang20k.html)
 - [[NeurIPS2020] Posterior Re-calibration for Imbalanced Datasets (a single
hyper-parameter.)](https://proceedings.neurips.cc/paper/2020/hash/5ca359ab1e9e3b9c478459944a2d9ca5-Abstract.html)

### Gradient method:
- [[NeurIPS2019] A simple baseline for bayesian uncertainty in deep learning (SWAG)](https://proceedings.neurips.cc/paper/2019/file/118921efba23fc329e6560b27861f0c2-Paper.pdf)
- [[NeurIPS2021] On the Importance of Gradients for Detecting Distributional Shifts in the Wild (GradNorm)](https://proceedings.neurips.cc/paper/2021/hash/0607f4c705595b911a4f3e7a127b44e0-Abstract.html)

### Distance method:
- [[NeurIPS2018] A Simple Unified Framework for Detecting Out-of-Distribution Samples and Adversarial Attacks (Mahalanobis Distance)](https://proceedings.neurips.cc/paper/2018/hash/abdeb6f575ac5c6676b747bca8d09cc2-Abstract.html)
- [[ICML2020]Uncertainty Estimation Using a Single Deep Deterministic Neural Network](http://proceedings.mlr.press/v119/van-amersfoort20a.html)

## Test augmentation
- [[UAI2020] Greedy Policy Search: A Simple Baseline for Learnable Test-Time Augmentation](https://arxiv.org/pdf/2002.09103.pdf)
- [[MIDL2021] Test-Time Mixup Augmentation for Uncertainty Estimation in Skin Lesion Diagnosis](https://openreview.net/forum?id=aGfL5C9wRx_)
- [[ICML2021]Evaluating Robustness of Predictive Uncertainty Estimation: Are Dirichlet-based Models Reliable?](http://proceedings.mlr.press/v139/kopetzki21a/kopetzki21a.pdf)

## Truthyworthy AI and application:
- [[NeurIPS2021] Reliable and Trustworthy Machine Learning for Health Using Dataset Shift Detection](https://openreview.net/forum?id=hNMOSUxE8o6)
- [[Google 2021] Does Your Dermatology Classifier Know What It Doesn't Know? Detecting the Long-Tail of Unseen Conditions](https://arxiv.org/pdf/2104.03829.pdf)

## Out-of-distribution Detection: 
### Type of shift:
 - [[NeurIPS2021]An Information-theoretic Approach to Distribution Shifts](https://proceedings.neurips.cc/paper/2021/hash/93661c10ed346f9692f4d512319799b3-Abstract.html)
    - distribution shift = Covariate shift + Concept shift

### Emperical and theoretical:
 - [[NeurIPS2020] Why Normalizing Flows Fail to Detect Out-of-Distribution Data](https://proceedings.neurips.cc/paper/2020/hash/ecb9fe2fbb99c31f567e9823e884dbec-Abstract.html)
 - [[NeurIPS2020] On the Value of Out-of-Distribution Testing: An Example of Goodhart's Law](https://proceedings.neurips.cc/paper/2020/hash/045117b0e0a11a242b9765e79cbf113f-Abstract.html)
 - [[NeurIPS2021] Exploring the Limits of Out-of-Distribution Detection](https://proceedings.neurips.cc/paper/2021/hash/3941c4358616274ac2436eacf67fae05-Abstract.html)
 - [[NeurIPS2021] A Winning Hand: Compressing Deep Networks Can Improve Out-of-Distribution Robustness](https://proceedings.neurips.cc/paper/2021/hash/0607f4c705595b911a4f3e7a127b44e0-Abstract.html)

### Uncertainty estimation for sequence-to-sequence model:
- [[ICML2020] Frequentist Uncertainty in Recurrent Neural Networks via Blockwise Influence Functions](http://proceedings.mlr.press/v119/alaa20b/alaa20b.pdf)


### OOD detection:
#### Without exposure:
- [[ICIR2017] A Baseline for Detecting Misclassified and Out-of-Distribution Examples in Neural Networks (Softmax)](https://openreview.net/forum?id=Hkg4TI9xl)
- [[ICLR2018] Enhancing The Reliability of Out-of-distribution Image Detection in Neural Networks (ODIN = T scaling + input perturbation)](https://openreview.net/forum?id=H1VGkIxRZ)
- [[NeurIPS2020] Certifiably Adversarially Robust Detection of Out-of-Distribution Data](https://proceedings.neurips.cc/paper/2020/hash/b90c46963248e6d7aab1e0f429743ca0-Abstract.html)
- [[NeurIPS202] Energy-based Out-of-distribution Detection (Energy score)](https://proceedings.neurips.cc/paper/2020/hash/f5496252609c43eb8a3d147ab9b9c006-Abstract.html)
- [[NeurIPS2021] On the Importance of Gradients for Detecting Distributional Shifts in the Wild (GradNorm)](https://proceedings.neurips.cc/paper/2021/hash/0607f4c705595b911a4f3e7a127b44e0-Abstract.html)
- [[NeurIPS2021] ReAct: Out-of-distribution Detection With Rectified Activations](https://proceedings.neurips.cc/paper/2021/hash/01894d6f048493d2cacde3c579c315a3-Abstract.html)
- [[NeurIPS2021] Single Layer Predictive Normalized Maximum Likelihood for Out-of-Distribution Detection](https://proceedings.neurips.cc/paper/2021/hash/093b60fd0557804c8ba0cbf1453da22f-Abstract.html)
- [[NeurIPS2021] 
Learning Causal Semantic Representation for Out-of-Distribution Prediction](https://proceedings.neurips.cc/paper/2021/hash/310614fca8fb8e5491295336298c340f-Abstract.html)
- [[NeurIPS2021] STEP: Out-of-Distribution Detection in the Presence of Limited In-Distribution Labeled Data](https://proceedings.neurips.cc/paper/2021/hash/f4334c131c781e2a6f0a5e34814c8147-Abstract.html)
- [[NeurIPS2021] Task-Agnostic Undesirable Feature Deactivation Using Out-of-Distribution Data](https://proceedings.neurips.cc/paper/2021/hash/21186d7b1482412ab14f0332b8aee119-Abstract.html)

##### Evidential network:
 ![image](https://user-images.githubusercontent.com/26398708/144141888-9e777456-404b-4f0d-a0a1-103032958c99.png)
- [[NeurIPS2018] Evidential deep learning to quantify classification uncertainty](https://proceedings.neurips.cc/paper/2018/file/a981f2b708044d6fb4a71a1463242520-Paper.pdf)
  - [[video](https://www.youtube.com/watch?v=toTcf7tZK8c)][[Github](https://github.com/aamini/evidential-deep-learning/)][[Codes](https://github.com/muratsensoy/muratsensoy.github.io)][[ICCV2021](https://openaccess.thecvf.com/content/ICCV2021/papers/Bao_Evidential_Deep_Learning_for_Open_Set_Action_Recognition_ICCV_2021_paper.pdf)]
- [[NeurIPS2020] Posterior Network: Uncertainty Estimation without OOD Samples via Density-Based Pseudo-Counts](https://proceedings.neurips.cc/paper/2020/hash/0eac690d7059a8de4b48e90f14510391-Abstract.html)
 [[Codes](https://github.com/sharpenb/Posterior-Network)]
 - [[ICML2021]Evaluating Robustness of Predictive Uncertainty Estimation: Are Dirichlet-based Models Reliable?](http://proceedings.mlr.press/v139/kopetzki21a/kopetzki21a.pdf)
 - [[ICLR2022] Natural Posterior Network: Deep Bayesian Predictive Uncertainty for Exponential Family Distributions](https://openreview.net/forum?id=tV3N0DWMxCg)
 - [[AAAI2021] Multidimensional Uncertainty-Aware Evidential Neural Networks](https://arxiv.org/pdf/2012.13676.pdf)
 - [[ICASP2022] SEED: SOUND EVENT EARLY DETECTION VIA EVIDENTIAL UNCERTAINTY](https://arxiv.org/pdf/2202.02441.pdf)
##### Generative model:
- [[NeurIPS2019] Likelihood Ratios for Out-of-Distribution Detection](https://proceedings.neurips.cc/paper/2019/hash/1e79596878b2320cac26dd792a6c51c9-Abstract.html)
- [[ICLR2019] Do Deep Generative Models Know What They Don't Know?](https://openreview.net/forum?id=H1xwNhCcYm)
- [[NeurIPS2020] Likelihood Regret: An Out-of-Distribution Detection Score For Variational Auto-encoder](https://proceedings.neurips.cc/paper/2020/hash/eddea82ad2755b24c4e168c5fc2ebd40-Abstract.html)
- [[NeurIPS2021] Locally Most Powerful Bayesian Test for Out-of-Distribution Detection using Deep Generative Models](https://proceedings.neurips.cc/paper/2021/hash/7d3e28d14440d6c07f73b7557e3d9602-Abstract.html)

#### With exposure (Dirichlet Distribution and Evidential Perspective):
- [[NeurIPS2018] Predictive Uncertainty Estimation via Prior Networks (A Malinin, M Gales)](https://proceedings.neurips.cc/paper/2018/hash/3ea2db50e62ceefceaf70a9d9a56a6f4-Abstract.html)
  - [[video](https://www.youtube.com/watch?v=uuXFDGvNKjs)]
  ![image](https://user-images.githubusercontent.com/26398708/144079754-2ac68535-70b4-4f2f-afb1-0e40df1e1fc9.png)
- [[NeurIPS2019] Reverse KL-Divergence Training of Prior Networks: Improved Uncertainty and Adversarial Robustness (A Malinin, M Gales)](https://proceedings.neurips.cc/paper/2019/hash/7dd2ae7db7d18ee7c9425e38df1af5e2-Abstract.html)  
- [[NeurIPS2020] Towards Maximizing the Representation Gap between In-Domain & Out-of-Distribution Examples](https://proceedings.neurips.cc/paper/2020/hash/68d3743587f71fbaa5062152985aff40-Abstract.html)
- [[NeurIPS2020] OOD-MAML: Meta-Learning for Few-Shot Out-of-Distribution Detection and Classification](https://proceedings.neurips.cc/paper/2020/hash/28e209b61a52482a0ae1cb9f5959c792-Abstract.html)

#### OOD generalization:
- [[NeurIPS2021] Characterizing Generalization under Out-Of-Distribution Shifts in Deep Metric Learning](https://proceedings.neurips.cc/paper/2021/hash/d1f255a373a3cef72e03aa9d980c7eca-Abstract.html)
- [[NeurIPS2021] Towards a Theoretical Framework of Out-of-Distribution Generalization](https://proceedings.neurips.cc/paper/2021/hash/c5c1cb0bebd56ae38817b251ad72bedb-Abstract.html)
- [[NeurIPS2021] On the Out-of-distribution Generalization of Probabilistic Image Modelling (Cam&Huawei)](https://proceedings.neurips.cc/paper/2021/hash/1f88c7c5d7d94ae08bd752aa3d82108b-Abstract.html)



## Non-parametric Gaussian Process:
 - [[NeurIPS2020]Simple and Principled Uncertainty Estimation with Deterministic Deep Learning via Distance Awareness](https://papers.nips.cc/paper/2020/file/543e83748234f7cbab21aa0ade66565f-Paper.pdf)


## Without re-training methods:
- [[ICLR2018] Enhancing The Reliability of Out-of-distribution Image Detection in Neural Networks (ODIN)](https://openreview.net/forum?id=H1VGkIxRZ)
- [[NeurIPS2018] A Simple Unified Framework for Detecting Out-of-Distribution Samples and Adversarial Attacks (Mahalanobis Distance)](https://proceedings.neurips.cc/paper/2018/hash/abdeb6f575ac5c6676b747bca8d09cc2-Abstract.html)
- [[ICML2020] Detecting out-of-distribution examples with gram matrices (Gram)](http://proceedings.mlr.press/v119/sastry20a/sastry20a.pdf)
- [[NeurIPS202] Energy-based Out-of-distribution Detection (Energy score)](https://proceedings.neurips.cc/paper/2020/hash/f5496252609c43eb8a3d147ab9b9c006-Abstract.html)
