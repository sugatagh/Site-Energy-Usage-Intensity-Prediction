# Site Energy Usage Intensity Prediction

- [**Energy usage intensity**](https://en.wikipedia.org/wiki/Efficient_energy_use#Building_design) (EUI) refers to the amount of energy used per square foot annually. It is calculated by dividing the total energy consumed by the building in a year by the total gross floor area. Like miles per gallon for cars, EUI is the prime indicator of the energy performance of a building.

- The EUI of a site or a building may depend on
  - _building characteristics_: floor area, facility type etc.
  - _weather data for the location of the building_: annual average temperature, annual total precipitation etc.

- In this project, we aim to predict the [**continuous variable**](https://en.wikipedia.org/wiki/Continuous_or_discrete_variable#Continuous_variable) site EUI, given the characteristics of the building and the weather data for the location of the building.

- A detailed [**exploratory data analysis**](https://en.wikipedia.org/wiki/Exploratory_data_analysis) on the dataset is carried out.

- The observations obtained from EDA are used in the [**data preprocessing**](https://en.wikipedia.org/wiki/Data_Preprocessing) stages (consisting of [**missing data**](https://en.wikipedia.org/wiki/Missing_data) [**imputation**](https://en.wikipedia.org/wiki/Imputation_(statistics)) and [**categorical data encoding**](https://en.wikipedia.org/wiki/Categorical_variable#Categorical_variables_and_regression)) and [**feature engineering**](https://en.wikipedia.org/wiki/Feature_engineering) stages (consisting of [**feature extraction**](https://en.wikipedia.org/wiki/Feature_engineering), [**data transformation**](https://en.wikipedia.org/wiki/Data_transformation_(statistics)), and **binarization**).

- We employ the [**random forest**](https://en.wikipedia.org/wiki/Random_forest), [**XGBoost**](https://en.wikipedia.org/wiki/XGBoost), and [**CatBoost**](https://en.wikipedia.org/wiki/CatBoost) regressors to predict site EUI.

- We apply [**hyperparameter tuning**](https://en.wikipedia.org/wiki/Hyperparameter_optimization) to the random forest algorithm, which appears to perform best among the baseline candidates.

- The final model obtains a [**root mean square error**](https://en.wikipedia.org/wiki/Root-mean-square_deviation) (RMSE) score of $32.742930$, a [**mean absolute error**](https://en.wikipedia.org/wiki/Mean_absolute_error) (MAE) score of $17.944242$, and a [**coefficient of determination**](https://en.wikipedia.org/wiki/Coefficient_of_determination) $(R^2)$ of $0.703486$.
