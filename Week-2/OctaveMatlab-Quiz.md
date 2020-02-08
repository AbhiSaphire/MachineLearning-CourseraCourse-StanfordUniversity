## 1. Question 1
Suppose I first execute the following Octave/Matlab commands:
```matlab
A = [1 2; 3 4; 5 6]; 
B = [1 2 3; 4 5 6];
```

Which of the following are then valid commands? Check all that apply. (Hint: A' denotes the transpose of A.)
<ul>
<b><li>C = A * B;
<li>C = B' + A;</b>
<li>C = A' * B;
<li>C = B + A;
</ul>


## 2. Question 2
Let A=[16, 2, 3, 13; 5, 11, 10, 8; 9, 7, 6, 12; 4, 14, 15, 1].

Which of the following indexing expressions gives B=[16, 2; 5, 11; 9, 7; 4, 14]? Check all that apply.
<ul>
<b><li>B = A(:, 1:2);
<li>B = A(1:4, 1:2);</b>
<li>B = A(:, 0:2);
<li>B = A(0:4, 0:2);
</ul>


## 3. Question 3
Let AA be a 10x10 matrix and xx be a 10-element vector. Your friend wants to compute the product Ax and writes the following code:

```matlab
v = zeros(10, 1);
for i = 1:10
  for j = 1:10
    v(i) = v(i) + A(i, j) * x(j);
  end
end
```

How would you vectorize this code to run without any FOR loops? Check all that apply.
<ul>
<b><li>v = A * x;</b>
<li>v = Ax;
<li>v = A .* x;
<li>v = sum (A * x);
</ul>


## 4. Question 4
Say you have two column vectors v and w, each with 7 elements (i.e., they have dimensions 7x1). Consider the following code:
```matlab
z = 0;
for i = 1:7
  z = z + v(i) * w(i)
end
```
Which of the following vectorizations correctly compute z? Check all that apply.
* z = sum (v .* w);
* <b>z = v' * w;</b>
* z = v * w';
* z = v .* w;


## 5. Question 5
In Octave/Matlab, many functions work on single numbers, vectors, and matrices. For example, the sin function when applied to a matrix will return a new matrix with the sin of each element. But you have to be careful, as certain functions have different behavior. Suppose you have an 7x7 matrix X. You want to compute the log of every element, the square of every element, add 1 to every element, and divide every element by 4. You will store the results in four matrices, A, B, C, D. One way to do so is the following code:
```matlab
for i = 1:7
  for j = 1:7
    A(i, j) = log(X(i, j));
    B(i, j) = X(i, j) ^ 2;
    C(i, j) = X(i, j) + 1;
    D(i, j) = X(i, j) / 4;
  end
end
```
Which of the following correctly compute A, B, C or D? Check all that apply.

* <b>C = X + 1;</b>
* <b>D = X / 4;</b>
* <b>B = X .^ 2;</b>
* B = X ^ 2;
