
## Google
- [Artificial Intelligence and Statistics 2017, McMahan et al.][FedAvg: Communication-Efficient Learning of Deep Networks from Decentralized Data](http://proceedings.mlr.press/v54/mcmahan17a?ref=https://githubhelp.com)

## Survey and benckmarks
- [FedEval: A Benchmark System with a Comprehensive Evaluation Model for Federated Learning](https://arxiv.org/pdf/2011.09655.pdf)
- [JMIR 2020][Reliability and Performance Assessment of Federated Learning on Clinical Benchmark Data](https://www.jmir.org/2020/10/e20891)
- [Neurocomputing 2021] [Federated learning on non-IID data: A survey](https://reader.elsevier.com/reader/sd/pii/S0925231221013254?token=632A399662BA41FDDAB98BB060BC5EE5F1EB11AC093370FABAE5F7A68B1E52D7634200192495EEB568133B75A224CC07&originRegion=eu-west-1&originCreation=20220922101316)
   - A variety types of non-iidness are introduces, including feature space and label space
   - A series of solutions have been compared
   - Some personalisation approched have been covered

- [ICDE 2022][Federated Learning on Non-IID Data Silos: An Experimental Study](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9835537)
- [NeurIPS 2022][FLamby: Datasets and Benchmarks for Cross-Silo Federated Learning in Realistic Settings](https://openreview.net/forum?id=GgM5DiAb6A2)
- [NeurIPS 2022][pFL-Bench: A Comprehensive Benchmark for Personalized Federated Learning](https://openreview.net/pdf?id=2ptbv_JjYKA) [Alibaba FedScope](https://federatedscope.io/)
- [ITNNLS 2022][Towards Personalized Federated Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9743558)

## Scholars 
  - [CMU Tian Li](https://scholar.google.com/citations?user=8JWoJrAAAAAJ&hl=en)
    - FedProx, 2028, 2020
    - Ditto, 2021


##  Uncentainty quanitifcation
- [Approaches to Uncertainty Quantification in Federated Deep Learning](https://pdfl.iais.fraunhofer.de/preprints/PDFL_2.pdf)
- [NeurIPS 2022][FedPop:  A Bayesian Approach for Personalised Federated Learning](https://arxiv.org/abs/2206.03611)
- [ICML2022 Spotlight] [On the Practicality of Deterministic Epistemic Uncertainty](https://proceedings.mlr.press/v162/postels22a/postels22a.pdf)
  - Performance of detecting correct/incorrect predictions
  <img src="https://user-images.githubusercontent.com/26398708/187662495-f691e79a-e6dd-4c57-beba-cc2f3ae3025c.png" width="400">
  
  - uncertainty with increasing data shift
 <img src="https://user-images.githubusercontent.com/26398708/187662750-036eb3ca-b4db-424b-ae87-b6e6cfabba8a.png" width="400">
 
## Non IID
  - [2018, the  primary study showing the negative impact of non-iid][Federated learning with non-iid data](https://arxiv.org/abs/1806.00582)
  
  ![image](https://user-images.githubusercontent.com/26398708/195367715-cbbcac0b-5790-437a-b23e-7b30ed31a1a1.png)
   When data is non-iid, local model is likely to be overfitte and far away from the averaged mode. This is call 'client-drift', which could slow down the global convergence.
  - [MLsys 2020] [FedProx: Federated Optimization in Heterogeneous Networks](https://proceedings.mlsys.org/paper/2020/hash/38af86134b65d0f10fe33d30dd76442e-Abstract.html)
     - A loss regulasition that restrict the local update to aviod 'client-drift'
  - [ICLR 2020] [SCAFFOLD: Stochastic Controlled Averaging for Federated Learning](https://openreview.net/forum?id=rguu45C8oC)
      - Anlysis client drift in detail
  - [ITSP 2021][FedPD: A federated learning framework with adaptivity to non-IID data](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=78)
  - [ICLR 2021] FedBN [FedBN: Federated Learning on Non-IID Features via Local Batch Normalization](https://openreview.net/forum?id=6YEQUn0QICG)
  - [IEEE TRANSACTIONS ON SIGNAL PROCESSING 2021] [FedPD: A Federated Learning Framework With Adaptivity to Non-IID Data](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9556559)
  - [ICLR 2021] From FedPD to CLIME [An Agnostic Approach to Federated Learning with Class Imbalance](https://openreview.net/forum?id=Xo0lbDt975)
  - [NeurIPS 2021] [No Fear of Heterogeneity: Classifier Calibration for Federated Learning with Non-IID Data](https://proceedings.neurips.cc/paper/2021/hash/2f2b265625d76a6704b08093c652fd79-Abstract.html) 
      - Some observation and understanding about the effect of non-IID
      - Debias the classfier
 - [ICML2022][Federated Learning with Label Distribution Skew via Logits Calibration](https://proceedings.mlr.press/v162/zhang22p.html)
     - A prior will be placed before softmax to calibrate the distribution
 - [KDD2021][Fedrs: Federated learning with restricted softmax for label distribution non-iid data](https://dl.acm.org/doi/abs/10.1145/3447548.3467254)

## Personalisation 
- [CoRR 2020] [Adaptive Personalized Federated Learning](https://arxiv.org/pdf/2003.13461.pdf)
   - Prior to this work, the ultimate goal of most FL study is to learn a global model that achieves uniformly good performance over almost all participating clients.
   - **Client drift**: in the presence of statistical data heterogeneity, the global model might not generalize well on the local data of each client individually. -- This means poor generalisation on the client's local testing set.  It is questionable how generalise overall.
   - **Pluralistic approach**: to embrace statistical heterogeneity and mitigate the effect of negative transfer, it is necessary to integrate the personalization into learning instead of finding a single consensus predictor. 
- [ICML 2021][Ditto: Fair and Robust Federated Learning Through Personalization](https://proceedings.mlr.press/v139/li21h.html)
- [CoRR 2021][HypCluster: Three Approaches for Personalization with Applications to Federated Learning](https://arxiv.org/abs/2002.10619)(https://arxiv.org/pdf/2002.10619.pdf)
- [ICLR 2021][FedBN: Federated Learning on Non-IID Features via Local Batch Normalization](https://openreview.net/forum?id=6YEQUn0QICG)
- [NeurIPS 2020][citation 200+][pFedMe: Personalized federated learning with moreau envelopes](https://proceedings.neurips.cc/paper/2020/hash/f4f1f13c8289ac1b1ee0ff176b56fc60-Abstract.html)
- [NeurIPS 2021][FedEM: Federated Multi-Task Learning under a Mixture of Distributions](https://proceedings.neurips.cc/paper/2021/hash/82599a4ec94aca066873c99b4c741ed8-Abstract.html)
- [ICML 2022] [Personalized Federated Learning via Variational Bayesian Inference](https://proceedings.mlr.press/v162/zhang22o/zhang22o.pdf)
  -   FegAvg is applied on Bayesian neural networks, but uncertainty is not well studied. 
  -   Non-IID setting, each client owns 5/10 classes. 
        <!--<img src="https://user-images.githubusercontent.com/26398708/188150594-7d76df5f-f83e-4622-a61e-df130567ce40.png" width="200">-->
<img src="https://user-images.githubusercontent.com/26398708/186911075-2c1d2632-2fab-44f0-8709-3391a5e7d73e.png" width="300">


## Imbalance
"Due to the mismatch among local and global data distribution, general approches to class imbalace on the clients may be not effective.
With the privacy constrict, it is also infeasible to require clients to upload data dsitrbution. "

 - [AAAI 2021] [RatioLoss: Addressing class imbalance in federated learning](https://ojs.aaai.org/index.php/AAAI/article/view/17219)
     - A global dataset is needed to monitor the loss 
 - [ICLR 2022] [CLIMB: An Agnostic Approach to Federated Learning with Class Imbalance](https://openreview.net/forum?id=Xo0lbDt975)
     - No global data
     - Cross silo setting
 - [Infocom workshop 2021][FedCluster: A Federated Learning Framework for Cross-Device Private ECG Classification](https://ieeexplore.ieee.org/document/9797945)
     - cross device clustering
     - a global dataset needed.


## Cross-device
  - [ICLR 2021][MIME: Breaking the centralized barrier for cross-device federated learning](https://proceedings.neurips.cc/paper/2021/file/f0e6be4ce76ccfa73c5a540d992d0756-Paper.pdf)
  - 
## Ensembles
  - [NeurIPS2020][Ensemble Distillation for Robust Model Fusion in Federated Learning](https://proceedings.neurips.cc/paper/2020/file/18df51b97ccd68128e994804f3eccc87-Supplemental.pdf)
  - [UAI2022][Self-Distribution Distillation: Efficient Uncertainty Estimation](https://openreview.net/forum?id=rhNgEI8s5xc)
  - [ICLR2021][FedBE: Making Bayesian Model Ensemble Applicable to Federated Learning](https://openreview.net/forum?id=dgtpE6gKjHn)

## Prototype:
 - [AAAI2022][Fedproto: Federated prototype learning across heterogeneous clients](https://arxiv.org/abs/2104.01893)
    - A regularization term to approach local prototype to the global one is required. Otherwise, it is hard to gurantte they are in the same feature space. 


## Generativ model and federated learning:
  - [AAAI2020] [Uncertainty-Aware Deep Classifiers Using Generative Models](https://ojs.aaai.org/index.php/AAAI/article/view/6015)


## For health
  - [Nature Medicine 2021] [Federated learning for predicting clinical outcomes in patients with COVID-19](https://www.nature.com/articles/s41591-021-01506-3)
  - [Infocom workshop 2021][FedCluster: A Federated Learning Framework for Cross-Device Private ECG Classification](https://ieeexplore.ieee.org/document/9797945)
  - [Arxiv 2022, FedAvg][Application of federated learning techniques for arrhythmia classification using 12-lead ECG signals](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9797945&tag=1)
    - [Cic 2020 winner][ECG abnormalities recognition using convolutional network with global skip connections and custom loss function] (https://ieeexplore.ieee.org/abstract/document/9344393)
  - [Personalized Federated Learning for ECG Classification Based on Feature Alignment](https://downloads.hindawi.com/journals/scn/2021/6217601.pdf)
  - [Infocom 2021][FedSens: A Federated Learning Approach for Smart Health Sensing with Class Imbalance in Resource Constrained Edge Computing](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9488776)

## Client selection
 - [Towards understanding biased client selection in federated learning](https://proceedings.mlr.press/v151/jee-cho22a/jee-cho22a.pdf)

