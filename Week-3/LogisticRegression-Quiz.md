## 1. Question 1
Suppose that you have trained a logistic regression classifier, and it outputs on a new example x a prediction hθ(x) = 0.7. This means (check all that apply):

* Our estimate for P(y=0|x;θ) is 0.7. 
* <b>Our estimate for P(y=1|x;θ) is 0.7. 
* Our estimate for P(y=0|x;θ) is 0.3.</b>*
* Our estimate for P(y=1|x;θ) is 0.3.


## 2. Question 2
Suppose you have the following training set, and fit a logistic regression classifier hθ(x) = g(θ(0)+θ(1)x(1)+θ(2)x(2)).
Which of the following are true? Check all that apply.

![](Template/quiz1-Q2.png)


* <b> J(θ) will be a convex function, so gradient descent should converge to the global minimum.
* Adding polynomial features (e.g., instead using hθ(x)=g(θ(0)+θ(1)x(1)+θ(2)x(2)+θ(3)x(1)^2+θ(4)x(1)x(2)+θ(5)x(2)^2)) could increase how well we can fit the training data. </b>
* The positive and negative examples cannot be separated using a straight line. So, gradient descent will fail to converge.
* Because the positive and negative examples cannot be separated using a straight line, linear regression will perform as well as logistic regression on this data.

## 3.Question 3
For logistic regression, the gradient is given by ∂/∂θ(j)J(θ) = 1/m∑(1->m)(hθ(x(i))−y(i))x(i)j. Which of these is a correct gradient descent update for logistic regression with a learning rate of α? Check all that apply.

* θj := θj − α/m ∑(i=1->m)(transpose(θ)x−y(i))xj(i) (simultaneously update for all j).
* <b>θ := θ − α/m ∑(i=1->m)(1/(1+e^(−transpose(θ)x(i))) − y(i))x(i). </b>
* θ := θ − α/m ∑(i=1->m)(transpose(θ)x−y(i))x(i).
* <b>θ := θ − α/m∑(i=1->m)(hθ(x(i))−y(i))x(i). </b>


## 4.Question 4
Which of the following statements are true? Check all that apply.

* <b>The one-vs-all technique allows you to use logistic regression for problems in which each y(i) comes from a fixed, discrete set of values. </b>
* For logistic regression, sometimes gradient descent will converge to a local minimum (and fail to find the global minimum). This is the reason we prefer more advanced optimization algorithms such as fminunc (conjugate gradient/BFGS/L-BFGS/etc).
* <b>The cost function J(θ) for logistic regression trained with m≥1 examples is always greater than or equal to zero. </b>
* Since we train one classifier when there are two classes, we train two classifiers when there are three classes (and we do one-vs-all classification).


## 5.Question 5
Suppose you train a logistic classifier hθ(x)=g(θ(0)+θ(1)x(1)+θ(2)x(2)). Suppose θ(0)=−6,θ(1)=1,θ(2)=0. Which of the following figures represents the decision boundary found by your classifier?

![](Template/quiz1-Q4.png)

**Correct option - B**
