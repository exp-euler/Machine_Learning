# Predicting House Prices

This ML predictive model is built for competing in
[this](https://www.kaggle.com/competitions/home-data-for-ml-course/) competition.
The implementation is done through a pipeline framework in order to keep
everything scalable and well organised. Hyper-parameter tuning of the
`XGBRegressor()` is done through `GridSearchCV`.

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

