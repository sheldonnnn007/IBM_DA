# w5_ModelEvaluation

##### Out-of-sample evaluation or test set

- Model Evaluation and Redfinement
- Overfitting, Underfitting and model Selection
- Ridge Regression
- Grid Search

Tell us how our model works in a real world

## 1. Model Evaluation and Redfinement

<img src="./photos/image-20230404122044992.png" alt="image-20230404122044992" style="zoom:50%;" />

Using a *lot of data for training*, gives us a accurate means to determing how well our model will perform in the real world. But the precision of perfomance will be low.

If we use *fewer data points* to train the model and more to test the model, the accuracy of the generalization performance will be less but the model will have good precision.

- Cross validation : **cross_val_score()**

  the dataset will be split to several folds. And we continue use most for traning and less for test until every fold is used for bith testing and training.

  <img src="./photos/image-20230404130336098.png" alt="image-20230404130336098" style="zoom:50%;" /><img src="./photos/image-20230404130230887.png" alt="image-20230404130230887" style="zoom:50%;" />

- Cross_val_predict()
  <img src="./photos/image-20230404130703422.png" alt="image-20230404130703422" style="zoom:50%;" />

## 2. Overfitting, Underfitting and model Selection

Undercutting:  model is too simple to fit the data

Overfitting: Estimated function oscillate not tracking the function. Estimated function extramly good at tracking the data but estimating the function.

<img src="./photos/image-20230404145358308.png" alt="image-20230404145358308" style="zoom:50%;" />

## 3. Ridge Regression

##### Normalization and Regularisation: 

Normalization is useful when your data has varying scales and the algorithm you are using does not make assumptions about the distribution of your data, such as **k-nearest neighbors** and artificial neural networks. Regularization is a feature scaling technique that is intended to **solve the problem of overfitting**.

<img src="./photos/image-20230404152100444.png" alt="image-20230404152100444" style="zoom:50%;" />



<img src="./photos/image-20230404152428924.png" alt="image-20230404152428924" style="zoom:50%;" />



- How to determine Alpha

1.Cross<img src="./photos/image-20230404153009768.png" alt="image-20230404153009768" style="zoom:50%;" />

2.MSE

<img src="./photos/image-20230404153426579.png" alt="image-20230404153426579" style="zoom:50%;" />

## 4. Grid Search (Tune hyper-parameters of an estimator)

<img src="./photos/image-20230404163232841.png" alt="image-20230404163232841" style="zoom:50%;" />

<img src="./photos/image-20230404163444202.png" alt="image-20230404163444202" style="zoom:50%;" />

<img src="./photos/image-20230404163930029.png" alt="image-20230404163930029" style="zoom:50%;" />

<img src="./photos/image-20230404164657895.png" alt="image-20230404164657895" style="zoom:50%;" />







<img src="./photos/image-20230404165032336.png" alt="image-20230404165032336" style="zoom:50%;" />

<img src="./photos/image-20230404165134533.png" alt="image-20230404165134533" style="zoom:50%;" />

<img src="./photos/image-20230404165210528.png" alt="image-20230404165210528" style="zoom:50%;" />
