# Predicting House Prices

This folder contains predictive models built for competing in
[this](https://www.kaggle.com/competitions/home-data-for-ml-course/) Kaggle 
competition.

## Machine Learning Approach
This model is available through the file `House_Prices_XGB.ipynb`.
The implementation is done through a pipeline framework in order to keep
everything scalable and well organised. Hyper-parameter tuning of the
`XGBRegressor()` is done through `GridSearchCV`. The two main libraries used are
`SciKit-Learn` and `XGBoost`.

### Model Accuracy
Currently the model achieves a Mean Absolute Error of `14568.98`, which ranks it
`668th` in the leaderboard of the competition mentioned above. At the time of
writing, the competition has `38808` different slutions uploaded, so this model
is in top `1.7%` (username ThomaZoto).

## Deep Learning Approach
This model is available through the file `House_Prices_Skorch.ipynb`.
The implementation is done through a pipeline framework in order to keep
everything scalable and well organised. Hyper-parameter tuning of the
`NeuralNet Regressor` is done through `GridSearchCV`. The main libraries used are
`SciKit-Learn`, `Dask`, `PyTorch` and `Skorch`.

### Model Training
The model has been trained and optimized in parallel using the `Dask` library.
As is, the code will run on a local `dask cluster` over 4 CPU cores, however,
it can easily be made to run in one or more GPUs (if available). Moreover, the
dask client can also be an AWS cluster. To set up the AWS cluster for using
`Dask`, I advise using the book 'Data Science with Python and Dask' by Jesse
C. Daniel.
The whole book is nicely structured and the configuration of a `Dask` cluster on
AWS is explained in Chapter 11.

## Usage
All of the libraries needed to run each of the files are mentioned above and can
be easily installed using `pip`. Make sure you install the latest versions of
each library, because early versions had bugs that were very hard to track down
and only fixable by using a newer version of the library. \
\
To run the project locally, first create a **`input/`** directory inside
**`House_Prices/`** by running:
```sh
user@user:~/Machine_Learning/House_Prices$ mkdir input
```
Then, download the training and testing data from
[here](https://www.kaggle.com/competitions/home-data-for-ml-course/data) and
copy it to **`House_Prices/input`**. You should be ready to run
**`House_Prices.ipynb`** using Jupyter Notebook.

