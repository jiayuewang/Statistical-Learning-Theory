# 11/12
### review from week 11
kernel function K discussion

### compare linear classifiers
lDA vs logistic regression vs linear svm

### unbalanced data 
- When you use LR, the results are similar (except the intercept term)
- a weird example on 302+160 vs 302+1.

# 11/14
### tree boosting, which is useful for project 3
- when to split (calculate the gain); 
- when to stop (define the goodness of fit)
- impurity measures

### Boosting overview
- 

### the algorithm of AdaBoosting
- initialize wi, 
- for t in 1 to T, fit g_t(x), compute \alpha_t, update the weights.

- notice: when T goes to infinity, Training-Error (G_T) will go to 0.
  - the key is the inequality function on the exponential loss.
  - when the training error is 0.5, there will be an running error.

# 11/16
### comparison between misclassification and entrophy
- the first two are more popular

### check r file 
- after pruning, you will see 0 and 0 on both left and right. That's indicator to stop.

### algorithm
- upper bound keeps decreasing when the value is not 1/2.
- toy example
  - tip1: when error rate > 1/2, flip the sigh: h1(x)
  - tip2: update the weights with the formula.
 
### adaboosting tree is not strictly monologue
- check the rcode_old_boost.html
- check Feng's boosting algorithm
- the loss function is the exponential loss eta*e^-a+(1-eta)*e^a = Omega.
- overfitting issue in the rcode (n=10 performs best)

### Boosting: forward stagewise additive modeling
- Additive model: f(x) = a1g1+a2g2+...+aTgT.
- Forward: select a1, g1 to min(fx), and then freeze them; and then a2, g2, and so on.....
- take the diravative to get the best ai.

### L2-Boosting
### GBM is going to retire???
### check cs.washington.edu/~tqche website for lightGBM, CatBoost, GBM3





###课后，(today)
- 尝试cloud computering
- 完成quiz
- github version control
- github webpage design
- 找个师父打刀塔
- 收拾屋子
- 检查日程
- artifact problem



