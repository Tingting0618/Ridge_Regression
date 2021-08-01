# Ridge Regression

- Ridge Regression (also called Tikhonov regularization) is a regularized version of Linear Regression: a regularization term is added to the cost function.
- This forces the learning algorithm to not only fit the data but also keep the model weights as small as possible.
- It is important to scale the data (e.g., using a StandardScaler) before performing Ridge Regression, as it is sensitive to the scale of the input features. This is true of most regularized models.

  ![download](https://user-images.githubusercontent.com/44503223/127774883-f08a0956-ab8a-487d-a795-33bdd85dca83.png)


#### Content Includes:
- Perform Ridge Regression with Scikit-Learn using a closed-form solution.

  ```python
  from sklearn.linear_model import Ridge
  ridge_reg = Ridge(alpha=1, solver="cholesky")
  ridge_reg.fit(X, y)
  ```
 
- Perform Ridge Regression using Stochastic Gradient Descent by adding a regularization term to the cost function equal to half the square of the ℓ2 norm of the weight vector.

  ```python
  from sklearn.linear_model import SGDRegressor
  sgd_reg = SGDRegressor(penalty="l2")
  sgd_reg.fit(X, y.ravel())
  y_predict_SGD = sgd_reg.predict(X)
  ```
  ![download](https://user-images.githubusercontent.com/44503223/127774872-3f0fd412-6f9d-4da9-a249-483d347d20b5.png)

 
## Learn More

For more information, please check out the [Project Portfolio](https://tingting0618.github.io).

## Reference

This repo is my learning journal following:
- Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition, by Aurélien Géron (O’Reilly). Copyright 2019 Kiwisoft S.A.S., 978-1-492-03264-9.
