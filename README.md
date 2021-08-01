# Ridge Regression

Ridge Regression (also called Tikhonov regularization) is a regularized version of Linear Regression: a regularization term is added to the cost function.
This forces the learning algorithm to not only fit the data but also keep the model weights as small as possible.
It is important to scale the data (e.g., using a StandardScaler) before performing Ridge Regression, as it is sensitive to the scale of the input features. This is true of most regularized models.

#### Content Includes:
- Perform Ridge Regression with Scikit-Learn using a closed-form solution.
- Perform Ridge Regression using Stochastic Gradient Descent by adding a regularization term to the cost function equal to half the square of the ℓ2 norm of the weight vector.


## Learn More

For more information, please check out the [Project Portfolio](https://tingting0618.github.io).

## Reference

This repo is my learning journal following:
- Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition, by Aurélien Géron (O’Reilly). Copyright 2019 Kiwisoft S.A.S., 978-1-492-03264-9.
