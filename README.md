# **Introduction**

So far you have explored what regression is with sample data gathered of different datasets for different projects. You have also visualized it using Matplotlib and seaborn.
Now you are ready to dive deeper into regression for ML. While visualization allows you to make sense of data, the real power of Machine Learning comes from training models. Models are trained on historic data to automatically capture data dependencies, and they allow you to predict outcomes for new data, which the model has not seen before.
and you will see more about the main types of linear regression and along with some of the math underlying these techniques. Those models will allow us to predict dependiente depending on different input data of independiente values.

1. Linear regression is a **linear model**, e.g. a model that assumes a linear relationship between the input variables (x) and the single output variable (y).

2. More specifically, that y can be calculated from a linear combination of the input variables (x).

3. When there is a **single input variable (x)**, the method is referred to as simple linear regression and When more than **one input variable** multiple input variables.

4. Different techniques can be used to prepare or train the linear regression equation from data, the most common of which is called **Ordinary Least Squares**. It is common to therefore refer to a model prepared this way as Ordinary Least Squares Linear Regression or just Least Squares Regression.

5. **Linear Regression Equation:-**

                                 y = B0 + B1*x

1. The linear equation assigns one scale factor to each input value or column, called a coefficient and represented by the capital Greek letter Beta (B). 

2. One additional coefficient is also added, giving the line an additional degree of freedom (e.g. moving up and down on a two-dimensional plot) and is often called the intercept or the bias coefficient.

3. In higher dimensions when we have more than one input (x), the line is called a plane or a hyper-plane.


**Types**

*    There are many more techniques because the model is so well studied. 

**1. Simple Linear Regression**

With simple linear regression when we have a single input, we can use statistics to estimate the coefficients.

This requires that you calculate statistical properties from the data such as means, standard deviations, correlations and covariance. All of the data must be available to traverse and calculate statistics.


**2. Ordinary Least Squares**

When we have more than one input we can use Ordinary Least Squares to estimate the values of the coefficients.

The Ordinary Least Squares procedure seeks to minimize the sum of the squared residuals. This means that given a regression line through the data we calculate the distance from each data point to the regression line, square it, and sum all of the squared errors together.

This approach treats the data as a matrix and uses linear algebra operations to estimate the optimal values for the coefficients. It means that all of the data must be available and you must have enough memory to fit the data and perform matrix operations.

**3. Gradient Descent**

When there are one or more inputs you can use a process of optimizing the values of the coefficients by iteratively minimizing the error of the model on your training data.

This operation is called Gradient Descent and works by starting with random values for each coefficient. The sum of the squared errors are calculated for each pair of input and output values. A learning rate is used as a scale factor and the coefficients are updated in the direction towards minimizing the error. The process is repeated until a minimum sum squared error is achieved or no further improvement is possible.

When using this method, you must select a learning rate (alpha) parameter that determines the size of the improvement step to take on each iteration of the procedure

**4. Regularization**

There are extensions of the training of the linear model called regularization methods. 

These seek to both minimize the sum of the squared error of the model on the training data (using ordinary least squares) but also to reduce the complexity of the model (like the number or absolute size of the sum of all coefficients in the model).

*  Two popular examples of regularization procedures for linear regression are:

**Lasso Regression:**
        where Ordinary Least Squares is modified to also minimize the absolute sum of the coefficients (called L1 regularization).
        
        
**Ridge Regression:**
        where Ordinary Least Squares is modified to also minimize the squared absolute sum of the coefficients (called L2 regularization).
These methods are effective to use when there is collinearity in your input values and ordinary least squares would overfit the training data.
