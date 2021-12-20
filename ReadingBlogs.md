## Evidential Network/ PriorNetwork/ Posteroir Network

Instead of estimiating the distribition on weights, i.e., Beyasian learsning, evidential deep learning is to find the distribution over predictors. \
Assume that what we obatin from a nueral network is not the categorical probability *P*, but a distribution *u* over *P*. \
Note: If the prior of the distribution is Dirichlet, then the posterior is still Dirichlet because Mulitnomial is conjugated to that. \
![image](https://user-images.githubusercontent.com/26398708/144232674-8744daa1-7ca4-47f8-984a-8817c772fc89.png)

Three strong but non-realistic assumptions:
1. An arbitary target prior *D(1)*
2. OOD exposure during training
3. Differential entropy can be nagetive (no sense)
4. No bound for alpha. 

NIPS2020 (2021 with graph based) paper overcame those limitations: 

*Posterior Network: Uncertainty Estimation without OOD Samples via Density-Based Pseudo-Counts* 

![image](https://user-images.githubusercontent.com/26398708/144252840-c937d419-df0a-4005-b378-ff9f7c07fb38.png)

Research questions:
1. To what degree is the estimated uncertainty calibrated? (ECE)
2. How to transfer the Pseudo-Counts into human-interpretable confidence score?
3. How to determine the threhold to distingish the incorrect and OOD samples?

