## Question 1
Consider the problem of predicting how well a student does in her second year of college/university, given how well she did in her first year. Specifically, let x be equal to the number of "A" grades (including A-. A and A+ grades) that a student receives in their first year of college (freshmen year). We would like to predict the value of y, which we define as the number of "A" grades they get in their second year (sophomore year). Refer to the following training set of a small sample of different students' performances (note that this training set may also be referenced in other questions in this quiz). Here each row is one training example. Recall that in linear regression, our hypothesis is h_θ(x) = θ(0) + θ(1)x and we use mm to denote the number of training examples. For the training set given above, what is the value of mm? In the box below, please enter your answer (which should be a number between 0 and 10).


## Question 2
For this question, assume that we are using the training set from Q1. Recall our definition of the cost function was J(θ(0), θ(1)) = (1/2m) * ∑{i=1:m} {(hθ(x^(i)) - y^(i))^2}
What is J(0, 1)? In the box below, please enter your answer (Simplify fractions to decimals when entering answer, and '.' as the decimal delimiter e.g., 1.5).


## Question 3
Suppose we set  0(0) = -2, 0(1) = 0.5 in the linear regression hypothesis from Q1. What is hθ(6)?


## Question 4
In the given figure, the cost function J(θ(0),θ(1)) has been plotted against θ(0) and θ(1), as shown in 'Plot 2'. The contour plot for the same cost function is given in 'Plot 1'. Based on the figure, choose the correct options (check all that apply). 
<ul>
<li>If we start from point B, gradient descent with a well-chosen learning rate will eventually help us reach at or near point A, as the value of cost function J(θ(0),θ(1)) is maximum at point A. </li>
<li>If we start from point B, gradient descent with a well-chosen learning rate will eventually help us reach at or near point A, as the value of cost function J(θ(0),θ(1)) is minimum at point A. </li>
<li>Point P (the global minimum of plot 2) corresponds to point A of Plot 1. </li>
<li>Point P (The global minimum of plot 2) corresponds to point C of Plot 1. </li>
<ul>


## Question 5
Suppose that for some linear regression problem (say, predicting housing prices as in the lecture), we have some training set, and for our training set we managed to find some θ(0), θ(1) such that J(θ(0), θ(1))=0
Which of the statements below must then be true? (Check all that apply.)
<ul>
<li>Gradient descent is likely to get stuck at a local minimum and fail to find the global minimum.
<li>For this to be true, we must have y^(i) = 0 for every value of i = 1, 2, ... ,m.
<li>Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.
<li>For this to be true, we must have θ(0) = 0 and θ(1) = 0 so that h_θ(x) = 0.
