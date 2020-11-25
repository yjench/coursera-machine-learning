# Linear Regression with Multiple Variables

1. Suppose m=4 students have taken some class, and the class had a midterm exam and a final exam. You have collected a dataset of their scores on the two exams, which is as follows:

   | midterm exam | (midterm exam)^2 | final exam |
   | ------------ | ---------------- | ---------- |
   | 89           | 7921             | 96         |
   | 72           | 5184             | 74         |
   | 94           | 8836             | 87         |
   | 69           | 4761             | 78         |

   You'd like to use polynomial regression to predict a student's final exam score from their midterm exam score. Concretely, suppose you want to fit a model of the form hθ(x)=θ0+θ1x1+θ2x2, where x1 is the midterm score and x2 is (midterm score)^2. Further, you plan to use both feature scaling (dividing by the "max-min", or range, of a feature) and mean normalization.

   What is the normalized feature x1^(3)? (Hint: midterm=94, final=87 is training example 3.) Please round off your answer to two decimal places and enter in the text box below.

   Answer: 0.52

   

2. You run gradient descent for 15 iterations with α=0.3 and compute J(θ) after each iteration. You find that the value of J(θ) **decreases** quickly then levels off. Based on this, which of the following conclusions seems most plausible?

   - [ ] Rather than use the current value of α, it'd be more promising to try a larger value of α (say α=1.0).
   - [ ] Rather than use the current value of α, it'd be more promising to try a smaller value of α*α* (say α=0.1).
   - [ ] α=0.3 is an effective choice of learning rate.

   

3. Suppose you have m=23 training examples with n=5 features (excluding the additional all-ones feature for the intercept term, which you should add). The normal equation is $\theta = (X^T X )^{-1} X^T y$. For the given values of m and n, what are the dimensions of θ, X, and y in this equation?

   - [ ] X is 23x5, y is 23x1, θ is 5x5
   - [ ] X is 23x5, y is 23x1, θ is 5x1
   - [ ] X is 23x6, y is 23x6, θ is 6x6
   - [x] X is 23x6, y is 23x1, θ is 6x1

   

4. Suppose you have a dataset with m=50 examples and n=15 features for each example. You want to use multivariate linear regression to fit the parameters θ to our data. Should you prefer gradient descent or the normal equation?

   - [ ] The normal equation, since gradient descent might be unable to find the optimal θ.
   - [ ] Gradient descent, since $(X^T X)^{-1}$ will be very slow to compute in the normal equation.
   - [x] The normal equaton, since it provides an efficient way to directly find the solution.
   - [ ] Gradient descent, since it will always converge to the optimal θ.

   

5. Which of the following are reasons for using feature scaling?

   - [x] It speeds up gradient descent by making it require fewer iterations to get to a good solution.
   - [ ] It prevents the matrix $X^TX$ (used in the normal equation) from being non-invertable (singular/degenerate).
   - [ ] It is necessary to prevent the normal equation from getting stuck in local optima.
   - [ ] It speeds up gradient descent by making each iteration of gradient descent less expensive to compute. 

