# Model Development

## Model Development

- Simple and Multiple Linear Regression
- Model Evaluation using Visualization
- Polynomial Regression and Pipelines
- R-squared and MSE for In-Sample Evaluation
- Prediction and Decision Making

## 1. Linear Regression and Multiple Linear Regression

The parameter is the output of trainning models be fitted with trainning points.

- <u>Simple Linear Regression(SLR)</u> useually be used for explore the correlation between two variables.

  <img src="./photos/image-20230403171859856.png" alt="image-20230403171859856" style="zoom:50%;" />

  <img src="./photos/image-20230403173116217.png" alt="image-20230403173116217" style="zoom:50%;" />

- <u>Multiple Linear Regression(MLR)</u> 

  <img src="./photos/image-20230403173337739.png" alt="image-20230403173337739" style="zoom:50%;" />

  z = df[['A','B','C','D']]

  Lm.fit(Z, df['price'])

  Yhat = lm.predict(X)

## 2. Model Evaluation using visualization

Residual Plot:<img src="./photos/image-20230403213023153.png" alt="image-20230403213023153" style="zoom:50%;" /><img src="./photos/image-20230403213129997.png" alt="image-20230403213129997" style="zoom:50%;" />
<img src="./photos/image-20230403213336098.png" alt="image-20230403213336098" style="zoom:50%;" />
<img src="./photos/image-20230403214318331.png" alt="image-20230403214318331" style="zoom:50%;" />

Residual plot:

Sis.residplot(df['highway-mpg'], df['price'])



## 3. Polynomial Regression and Pipelines

##### High-order polynomial regression

<img src="./photos/image-20230403220223661.png" alt="image-20230403220223661" style="zoom:50%;" />

##### Polynomial regression with more than **One D** (polyfit can not handle this case)

<img src="./photos/image-20230403222217358.png" alt="image-20230403222217358" style="zoom:50%;" />

<img src="./photos/image-20230403222350979.png" alt="image-20230403222350979" style="zoom:50%;" />

##### Pipelines

<img src="./photos/image-20230403215833337.png" alt="image-20230403215833337" style="zoom:50%;" />

<img src="./photos/image-20230403222614694.png" alt="image-20230403222614694" style="zoom:50%;" />

 <img src="./photos/image-20230403222737005.png" alt="image-20230403222737005" style="zoom:50%;" />

<img src="./photos/image-20230403222841970.png" alt="image-20230403222841970" style="zoom:50%;" />

## 4. Measures for In-sample Evaluation

Numerically evaluation: a way to numerically determine how good the model fits on dataset.

- Mean Squared Error(MSE): <u>From sklearn.metrics import mean_squared_error</u>

  <img src="./photos/image-20230403224401722.png" alt="image-20230403224401722" style="zoom:50%;" />

  Mean_squared_error(df['price'], Y_predict_simple_fit)

  <u>Both use the average value of the data points</u>

- R-squared(R^2): **<u>lm.score(X,Y)</u>**  normally between 1 and 0

  <img src="./photos/image-20230403225431780.png" alt="image-20230403225431780" style="zoom:50%;" />
  <img src="./photos/image-20230403230423860.png" alt="image-20230403230423860" style="zoom:50%;" />

  R^2 near 1, means 1- **0**, which means the line good fit for data







## 5. Prediction and Decision Making









