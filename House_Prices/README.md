# Predicting House Prices

This ML predictive model is built for competing in
[this](https://www.kaggle.com/competitions/home-data-for-ml-course/) competition.
The implementation is done through a pipeline framework in order to keep
everything scalable and well organised. Hyper-parameter tuning of the
`XGBRegressor()` is done through `GridSearchCV`.

## Model Accuracy
Currently the model achieves a Mean Absolute Error of `14568.98`, which ranks it
`668th` in the leaderboard of the competition mentioned above. At the time of
writing, the competition has `38808` different slutions uploaded, so this model
is in top `1.7%`.

## Usage
To run the project locally, first create a **`input/`** directory inside
**`House_Prices/`** by running:
```sh
user@user:~/Machine_Learning/House_Prices$ mkdir input
```
Then, download the training and testing data from
[here](https://www.kaggle.com/competitions/home-data-for-ml-course/data) and
copy it to **`House_Prices/input`**. You should be ready to run
**`House_Prices.ipynb`** using Jupyter Notebook.

