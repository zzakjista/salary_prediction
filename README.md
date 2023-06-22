# salary_prediction
The salary prediction model that is built by Machine Learning sturcture in kaggle competition
<u> we are two-man team and 3rd winner in this competition. </u>

## feature engineering
there are many feature to manipulate.
dataset has user's profile such as age, sex, education, major, etc.
The mainly engineering methods are feature selection, generation and PCA(dimenstion reduction).

## modeling 
we used two model to contribute ensemble model, Catboost and LightGBM.
especially, CatBoostRegressor is well in processing nominal variable and predicting numeric variable.
LightGBM is Gradient Boost Model that has more speed to train.
[single model] folder is consist of 5 catboost model that would be trained from different preprocessed dataset.
※ In our knowledge, Catboost model showed best performance is this dataset

## stacking
we conjucated contributing 10 models to ensemble with stacking method.
catboost and LGBM model of each Model A ~ B were used to prediction.
for buling stacking model with our results, we used LinearRegressor to predict final result.
we set ridge 1.0. finally, we completed sucessful result!


### 🛑 Notice 🛑
There are no datasets to use because of users privacy issue. 
but you can check all the process from preprocessing to prediction.
