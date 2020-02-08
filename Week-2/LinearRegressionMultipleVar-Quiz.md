## 1. Question 1
Suppose m=4 students have taken some class, and the class had a midterm exam and a final exam. You have collected a dataset of their scores on the two exams, which is as follows: 
<table>
<tr><th>midterm exam	<th>(midterm exam)^2 <th>final exam</th>
<tr><td>89	<td>7921	<td>96
<tr><td>72	<td>5184	<td>74
<tr><td>94	<td>8836	<td>87
<tr><td>69	<td>4761	<td>78
</table>
You'd like to use polynomial regression to predict a student's final exam score from their midterm exam score. Concretely, suppose you want to fit a model of the form h_θ(x) = θ(0) + θ(1)x(1) + θ(2)x(2), where x(1)  is the midterm score and x(2) is (midterm score)^2. Further, you plan to use both feature scaling (dividing by the "max-min", or range, of a feature) and mean normalization.

What is the normalized feature x(1)^(3)? (Hint: midterm = 94, final = 87 is training example 3.) Please round off your answer to two decimal places and enter in the text box below.

<b>0.52</b>
<code>Since X(1)^3, Average = 81, std deviation(Max-Min) = 25. Hence (94 - 81)/(94 - 69) = 0.52</code>

## 2. Question 2
You run gradient descent for 15 iterations with α=0.3 and compute J(θ) after each iteration. You find that the value of J(θ) decreases quickly then levels off. Based on this, which of the following conclusions seems most plausible?
<ul>
<li>Rather than use the current value of α, it'd be more promising to try a larger value of α (say α=1.0).
<li>Rather than use the current value of α, it'd be more promising to try a smaller value of α (say α=0.1).
<b><li>α=0.3 is an effective choice of learning rate.</b>
</ul>


## 3. Question 3
Suppose you have m = 28training examples with n = 4 features (excluding the additional all-ones feature for the intercept term, which you should add). The normal equation is θ = (transpose(X)*X)^(-1) * transpose(X)*y. For the given values of m and n, what are the dimensions of θ, X, and y in this equation?
<ul>
<li>X is 28×5, y is 28×1, θ is 5×1
<li>X is 28×4, y is 28×1, θ is4×1
<li>X is 28×5, y is 28×5, θ is 5×5
<b><li>X is 28×4, y is 28×1, θ is 4×4</b>
</ul>


## 4. Question 4
Suppose you have a dataset with m = 1000000 examples and n = 200000 features for each example. You want to use multivariate linear regression to fit the parameters θ to our data. Should you prefer gradient descent or the normal equation?
<ul>
<li>The normal equation, since gradient descent might be unable to find the optimal θ.
<li>The normal equation, since it provides an efficient way to directly find the solution.
<b><li>Gradient descent, since (transpose(X)*X)^(-1) will be very slow to compute in the normal equation.</b>
<li>Gradient descent, since it will always converge to the optimal θ.
</ul>


## 5. Question 5
Which of the following are reasons for using feature scaling?
<ul>
<b><li>It speeds up gradient descent by making it require fewer iterations to get to a good solution.</b>
<li>It is necessary to prevent the normal equation from getting stuck in local optima.
<li>It prevents the matrix transpose(X)*X(used in the normal equation) from being non-invertable (singular/degenerate).
<li>It speeds up gradient descent by making each iteration of gradient descent less expensive to compute.
