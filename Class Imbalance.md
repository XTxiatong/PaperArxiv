# Class Imbalanced Solutions

## Review
- [Intelligent data analysis, 2002] [The class imbalance problem: A systematic study](https://content.iospress.com/download/intelligent-data-analysis/ida00103?id=intelligent-data-analysis%2Fida00103).
- [Journal of Big Data, 2019] [Survey on deep learning with class imbalance](https://link.springer.com/content/pdf/10.1186/s40537-019-0192-5.pdf)
- [TKDE, 2008] [Learning from imbalanced data](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=5128907)
         
## Data-level Methods
 ### Resampling
   - [ICML 2017] Random up/over-sampling RUS, ROS [Experimental perspectives on learning from imbalanced data](https://dl.acm.org/doi/abs/10.1145/1273496.1273614)
   - [Arkiv 2015] ROS [The impact of imbalanced training data for convolutional neural networks](https://www.diva-portal.org/smash/get/diva2:811111/FULLTEXT01.pdf)
   -The experiments show that applying ROS to the level od class balance canbe effective in addressing slight class imlance.
   - [IEEE MIPR 2018] Dynamic sampling. [Dynamic sampling in convolutional neural networks for imbalanced data classifcation](https://ieeexplore.ieee.org/document/8396983)
   - [Weighted Random Sampler] Pytorch API choose samples according to the given weights, i.g., N/N_c
        - rf. [Improving The ResNet-based Respiratory Sound Classification Systems With Focal Loss](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9948543)

### Sythetic data
 - [IEEE 2012] SMOTE [Experimental perspectives on learning from imbalanced data](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=3477)
 - [IEEE 2016] RUS via image augmatation, [paper](https://www.diva-portal.org/smash/get/diva2:811111/FULLTEXT01.pdf)
   #### the use of RUS can eliminate class imbalance during traning, but it may be not not effective with the relatively big but extremely imbalanced data. 


## Algorithm-level Methods
  ### new loss function
  - [ICCV 2017]  [Focal Loss for Dense Object Detection](https://openaccess.thecvf.com/content_ICCV_2017/papers/Lin_Focal_Loss_for_ICCV_2017_paper.pdf)
     - Focal loss is orignially designed for binary classification, with gamma and alpha for the positive class.
     - When generalising FL to mutli-class case, there is no official papers.
     - Only using gamma [paper (1)](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9948543)
     - Using a tensor alpha as weights [code](https://github.com/AdeelH/pytorch-multi-class-focal-loss)
    
  ### cost-sensitive
   - [Trans 2018]  [Predicting Hospital Readmission via Cost-Sensitive Deep Learning](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8338085&tag=1)
   - a cost-matrix $C_{n,k}$ (sample n to class k) is needed and used in the loss function. 
  ### threshold moving 
   - [Neural Netw 2018] [A systematic study of the class imbalance problem in convolutional neural networks](https://www.sciencedirect.com/science/article/pii/S0893608018302107?via%3Dihub)
  - Threhold can be set according the prior class probability. But it is more useful when combined with ROS.
  ### Two phase training
  
  
  ### max margin 
  - [CVPR 2019] Bayesian Uncertainty [striking the rught balance with uncertainty](https://arxiv.org/pdf/1901.07590.pdf)
  - [CVPR 2019] [Class-Balanced Loss Based on Effective Number of Samples](https://openaccess.thecvf.com/content_CVPR_2019/papers/Cui_Class-Balanced_Loss_Based_on_Effective_Number_of_Samples_CVPR_2019_paper.pdf)
  - [NeurIPS 2019] [Learning Imbalanced Datasets with Label-Distribution-Aware Margin Loss](https://proceedings.neurips.cc/paper/2019/file/621461af90cadfdaf0e8d4cc25129f91-Paper.pdf)
  - [NeurIPS 2019][Rethinking the Value of Labels for Improving Class-Imbalanced Learning](https://proceedings.neurips.cc/paper/2020/file/e025b6279c1b88d3ec0eca6fcb6e6280-Paper.pdf)
  - [NeurIPS 2020] Posterior [Posterior Re-calibration for Imbalanced Datasets](https://proceedings.neurips.cc/paper/2020/file/5ca359ab1e9e3b9c478459944a2d9ca5-Paper.pdf)
    
    
## Hybrid Methods

![1657549471018](https://user-images.githubusercontent.com/26398708/178287065-2a84dc8e-c937-42dd-9e86-04225850592e.png)


## Recent Realted Papaers:
- [AAAI 2022] [Uncertainty-aware Learning Against Label Noise on Imbalanced Datasets](https://www.aaai.org/AAAI22Papers/AAAI-5530.HuangY.pdf)
- [AAAI 2022] [Improving Evidential Deep Learning via Multi-task Learning](https://www.aaai.org/AAAI22Papers/AAAI-2489.OhD.pdf)
- [AAAI 2022] [Addressing class imbalance in federated learning](https://ojs.aaai.org/index.php/AAAI/article/view/17219)
- [AAAI 2020] [A Novel Model for Imbalanced Data Classification](https://ojs.aaai.org/index.php/AAAI/article/view/6145)
- [ICML 2022][Class-Imbalanced Semi-Supervised Learning with Adaptive Thresholding](https://proceedings.mlr.press/v162/guo22e/guo22e.pdf)
- [ICML 2022][Pure Noise to the Rescue of Insufficient Data: Improving Imbalanced Classification by Training on Random Noise Images](https://proceedings.mlr.press/v162/zada22a/zada22a.pdf)
- [AAAI 2023][]()


