# 1022

intro to classification 
 * data
 * goal
 * loss function (eg: 0-1 loss, L(f(x),y) = 0, if y =f(x); 1, otherwise)
 
intro to discriminant analysis
 * joint dist = conditioans of x|y * marginal of y. P(x,y) = P(X=x | Y=y) * P(Y = y)
 
dist of p-dim x given y=k (QDA, LDA, FDA, NB)
 
* LDA here is Linear discriminant analysis, which is not equal to Latent dirichlet allocation
 
### 0-1: clear.
This could be extended to multi-classes (eg: digital example.)

### BT for 
(\pi_k)*f_k(x)

### QDA
Q (rank deficiency):
x in R256,n1 = 100, Sigma1_hat in 256*256, but the rank is only 99. <understand why>

Attention: we are removing a mean for each group. (dof deduction)


P14, these three parts help to make prediction. (undestand why)

### LDA
P15, grey are not needed to calculate.

P16, null space, keep inverse of 0 slice also 0.

P17, reduced rank LDA.

here p-dim can be reduced to k-1 dim. <2points fom a line, etc.>






# 1024
* OBS: software to record the screen.
* DA - QDA <P13>
* LDA - equivalent to linear.
* when Sigma^(-1) does not exist due to the rank deficiency, deal with it as if it exists. (Sigma+yita*Ip)
* Reduced Rank LDA --> (k-1) dim.
 - Use the covariance matrix to rotate the coordinates.
* FDA ratio of intra group variation and inter group variation.
* difference between PCA and GEP 
 - (GEP/FDA has more subjection and less assumption)
 - FDA is supervised triming and PCA is unsupervised.
* slice inverse regression is based on FDA
* GEP: understand, a, b, B, W. and eigenvalue decomposition keeps the rank.

### Two projects.
* Digits Project 
  - LDA is 75% precision on the test data;
  - FDA is very bad on the test data (serious overfitting problem)
  - PCA + LDA is 87% precision on the test data. <although they are same dimension as FDA>
  
* KlaR Prediction.
  - notice the difference between KlaR and NB <due to floating point calculation, tiny numbers should take their log before calculating.>
  
* Summary:
  - when P is very large, QDA, LDA, FDA are all very bad (not recommended.)
  - Logestic regression and other tree models introduced next weeks are better.
  - check their relationship 


# 1026
## Discriminant Analysis
summary: QDA, LDA, RDA, FDA, NB, etc.

### LDA: mu1, mu2, 
### 

### Should we worry about hte normality assumption?
* No, CLT.

### joint
supervised learning: LDA 
un - EM
semi- joint

### LDA square (LDA+LDA)
* image classification<>
* patches catching
* SIFT (mature function of describing patches)
* KMeans (eg, k = 4 or 15)

* LDA+LDA+boosting.works to 95%.
* DL of course works, but with more requirements on the machine.
* disadvantage: bad for categorical data, eg: Ames.

### LDA/NB high-dim
* 2-sample t-test (test the means of two groups are the same with t-test)

### RDA: Regularized Discriminant Analysis
* NC gamma=1, lambda=1, only consider the identity matrix, all the covariance matrix outside the diagnose are zero.

### Data analysis question on Ames categorical data (do we need to order the categorical data?)
comparison on different methods.
There are different different design matrix. but the yhat (prediction) is the same for all!









