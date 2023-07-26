# Car Price Prediction

This project aims to build a machine learning model to predict the prices of cars based on various features such as make, fuel type, aspiration, body style, drive wheels, engine location, engine type, number of cylinders, engine size, fuel system, compression ratio, city miles per gallon (MPG), and highway MPG.
The dataset used in this project can be found in the file cars-data.csv.

## Project Structure

- notebooks/
  - Cars_Price_Prediction_Model.ipynb   <!-- Jupyter Notebook with the code -->
- data/
  - cars-data.csv                      <!-- Dataset used for training the model -->
- models/
  - regressor_pickle                   <!-- Pickle file for saving the trained model using pickle -->
  - regressor_joblib                   <!-- Joblib file for saving the trained model using joblib -->
- car_image.jpg                        <!-- An image representing the project -->
- README.md                            <!-- This README file -->


## Libraries Used
-pandas
-numpy
-matplotlib
-seaborn
-scikit-learn

## Dataset Description

The dataset contains the following columns:

- `symboling`: Insurance risk rating (-3 to +3)
- `make`: Manufacturer of the car
- `fuel-type`: Type of fuel used by the car (gas or diesel)
- `aspiration`: Aspiration method (std or turbo)
- `body-style`: Body style of the car (convertible, hatchback, sedan, etc.)
- `drive-wheels`: Type of drive wheels (fwd, rwd, 4wd)
- `engine-location`: Location of the engine (front or rear)
- `wheel-base`: Wheel base measurement
- `length`: Length of the car
- `width`: Width of the car
- `h8`: Height of the car
- `engine-type`: Type of engine (dohc, ohcv, ohc, etc.)
- `num-of-cylinders`: Number of cylinders in the engine
- `engine-size`: Size of the engine
- `fuel-system`: Type of fuel system
- `compression-ratio`: Compression ratio of the engine
- `city-mpg`: Miles per gallon in city driving
- `highway-mpg`: Miles per gallon on the highway
- `price`: Price of the car (target variable)

## Data Preprocessing

Before building the model, the dataset was preprocessed as follows:

1. **Handling Missing Values**: No missing values were found in the dataset. Therefore, no imputation or handling of missing values was required.

2. **Encoding Categorical Features**: Categorical features such as `make`, `fuel-type`, `aspiration`, `body-style`, `drive-wheels`, `engine-location`, `engine-type`, `num-of-cylinders`, and `fuel-system` were encoded using LabelEncoder and OneHotEncoder. This step is essential to convert categorical data into numerical format, as most machine learning algorithms require numerical input.

## Model Building

In this project, a machine learning model, specifically a Linear Regression model, is trained to predict car prices based on the given features in the dataset. The model achieved an R-squared value of approximately 0.93, indicating a good fit to the data.

## Model Saving

We saved the trained model using both pickle and joblib libraries to the 'models' directory. The files `regressor_pickle` and `regressor_joblib` contain the trained model, which can be used for inference.

## How to Use

To use this project, follow these steps:

1. Clone this repository to your local machine.
2. Install the required libraries mentioned in the 'notebooks/Cars_Data_Analysis_and_Prediction.ipynb' file.
3. Run the Jupyter Notebook 'notebooks/Cars_Data_Analysis_and_Prediction.ipynb' to perform data analysis and train the prediction model.
4. After running the notebook, the trained model will be saved in both pickle and joblib formats in the 'models' directory.
5. You can use the saved model for predicting car prices on new data.

## Conclusion

This project provides data analysis and a machine learning model to predict car prices based on various features. It can be used to gain insights into the dataset and make price predictions for new car entries.

For any questions or suggestions, feel free to contact the project contributors.

## Contributors

- Keerthi

