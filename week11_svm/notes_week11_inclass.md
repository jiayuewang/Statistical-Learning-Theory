# 11/07 wed
### q&a in piazza.
dimension discussion on p in logiestic regression.

### question on last class 
- definition of forbidden direction.
- how to establish the lagrange definition (special attention ot the signal of lambda.)
- shine


### non-separable data
two parallel ways:
- kernel machine (non-linear svm)
- soft margin method.

### practical issues:
- binary decision ot probability
- multi-class svm

### understand the four groups of restraints.

### gamma  = c(svminR_FSS2006.pdf)
consequences of increase gamma:
- less number of support vectors,
- complex model
- overfitting


# 11/09 Fri

1. reviews
   - Hard Margin but problems.
   - solutions: Soft Margin or kernel selection
   
2. Practical issue a: from binary decision to probability
   - run a logistic regression wrt f(x_i)
   - di = f(xi) = xi^t*beta_hat+beta0_hat for {yi, di} in each i from 1 to n.
3. discussion on hinge loss???
4. Practical issue b: how to go from binary to multi-class.
   - Recall how logistic regression and QDA/LDA/NB, {{y|x} could be as many as you want}
   - vanilla extension to multicalss
     - one vs all C10-1=10 fit 10 SVMs
     - one vs one (python) C10-2 fit 45 SVMs
     - fit a ball. radias = sqrt(d)/2 - 1/2. Notice when d>9, radius is larger than 1!!!

5. for nonlinear SVM, we want to use the linear SVM model.
   - (x1, x2) -> (x1, x2, x1x2, x1^2, x2^2)
   - x -> Phi(x)
   - K_phi(x,z) = <phi(x), phi(z)>, obviously, the matrix is symatric.

6. K(x,z) = sigma (yita_i) * g_i(x) * g_i(z) {Mercer's condition}
7. kernel machine f(x) = a1K(x1,x)+...+anK(xn, x)+a0
   - pay attention to this symetric kernel matrix.
   - For SVM, we have Hinge-loss + Ridge-Penalty
   - For SVM, the sparsity is from Hinge-Loss

8. All this methodology is not depending the features given, but the relationship between the datasets. {very IBK}
9. RKHS is reproducing kernel hilbert space 
   1. {check SVM_RKHS to see how we extend the linear method to non-linear model}
   2. {check on the Hinge loss}




# 
- other recommendations on courses: 

1. cs 225; - Bro. Kai is taking care of it.
2. cd 440; - very interesting
3. cs 410/510; (star) - Prof. Zhai is super nice; 510 is very mathmatical.
4. cs 412/512; (star) - star
5. cs 498 AML (star)
6. info 490
7. ECE498 DSU / CS 498 DSU Data Science and Analytics (star)
