
## Learning Objectives

Week :one: 
- Define machine learning
- Define supervised learning
- Define unsupervised learning
- Write and run Python code in Jupyter Notebooks
- Define a regression model
- Implement and visualize a cost function
- Implement gradient descent
- Optimize a regression model using gradient descent

Week :two:
- Use vectorization to implement multiple linear regression
- Use feature scaling, feature engineering, and polynomial regression to improve model training
- Implement linear regression in code

Week :three: 
- Use logistic regression for binary classification
- Implement logistic regression for binary classification
- Address overfitting using regularization, to improve model performance

## Notes

- _What is Machine Learning?_: "Field of study that gives computers the ability to learn without being explicitly programmed."
- _Supervised Learning_
  - Learning input (x) to output (y) mapping 
  - Learns from being given __right answers__
 - Regression:
   - Predict a __number__ from __infinitely__ many possible outcomes
 - Classification:
   - Predict __categories__
   - Predict __small number__ of possible outcomes 
  - Examples: 
    1. Spam filtering
        - Input: email
        - Output: spam (1) or not spam (0)
    2. Speech recognition
        - Input: audio
        - Output: text transcripts
    3. Machine translation
        - Input: English
        - Output: Spanish
    4. Online advertising
        - Input: Ad, user info
        - Output: Click (1) or no click (0)
    5. Self-driving car
        - Input: Imagine, radar info
        - Output: Position of the car
    6. Visual inspection
        - Input: Image of phone
        - Output: Defect (1) or no defect (0)

# 1. Linear Regression

__Univariate Linear Regression__:


__Multivariate/Multiple Linear Regression__:


# 2. Loss and Cost Function

- Loss function: Error for a single training example
- Cost function: Total error of a set of data points

# 3. Gradient Descent

__One Feature__:

__Multiple Feature__:

Repeat until convergence:
$$
    w = w - \alpha \frac{1}{m} \sum_{i=1}^{m} (f_{w,b}(x^ {(i)}) - y^{(i)})x^ {(i)} = w - \alpha \frac{\partial}{\partial w} J(w,b) \newline
    b = b - \alpha \frac{1}{m} \sum_{i=1}^{m} (f_{w,b}(x^ {(i)}) - y^{(i)}) = b - \alpha \frac{\partial}{\partial b} J(w,b)
$$

$$
\text{repeat until convergence:} \; \lbrace \\
    w = w - \alpha \underbrace{\frac{1}{m} \sum_{i=1}^{m} (f_{w,b}(x^ {(i)}) - y^{(i)})x^ {(i)}}_{\frac{\partial}{\partial w} J(w,b)} \\
    b = b - \alpha \underbrace{\frac{1}{m} \sum_{i=1}^{m} (f_{w,b}(x^ {(i)}) - y^{(i)})}_{\frac{\partial}{\partial b} J(w,b)} \\
    % \text{simultaneously update} \; w,b \\
    \rbrace
$$

# Logistic Regression

__Loss Function:__

$$
L( f_{\vec{w},b}(\vec{x}^ {(i)}), y^{(i)}) = -y^{(i)} \log(f_{\vec{w},b}(\vec{x}^ {(i)})) - (1 - y^{(i)}) \log (1 - f_{\vec{w},b}(\vec{x}^ {(i)}))
$$

- :white_check_mark: The loss function is convex (single global minimum)

__Cost Function:__

$$
J( \vec{w}, b ) = \frac{1}{m} \sum_{i=1}^{m} [ L( f_{\vec{w},b}(\vec{x}^ {(i)}), y^{(i)}) ]
$$

_Why choose this particular function?_ Has been derived using Maximum Likelihood Estimation (TODO: include proof).