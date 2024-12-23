
# **Car Fuel Consumption Prediction using Linear Regression**

## **Project Description**
This project implements a **simple and multiple linear regression model** to predict a car's **fuel consumption** based on various vehicle features such as engine size, transmission type, and vehicle class. The goal is to predict the combined fuel consumption (in liters per 100 kilometers) for a given car based on the given input features.

The model is trained on a dataset that includes information about car specifications and their corresponding fuel consumption values.

## **Dataset**

The dataset contains several features related to vehicles and their fuel consumption. Below are the columns in the dataset:

| **Feature**               | **Description**                                                                |
|---------------------------|--------------------------------------------------------------------------------|
| `MODELYEAR`               | The year the car model was released.                                           |
| `MAKE`                    | The manufacturer of the car.                                                   |
| `MODEL`                   | The specific model of the car.                                                 |
| `VEHICLECLASS`            | The class of the vehicle (e.g., Compact, SUV).                                |
| `ENGINESIZE`              | The engine size of the car (in liters).                                        |
| `CYLINDERS`               | The number of cylinders in the engine.                                         |
| `TRANSMISSION`            | The transmission type (e.g., Automatic, Manual).                               |
| `FUELTYPE`                | The type of fuel used by the car (e.g., Gasoline, Diesel).                     |
| `FUELCONSUMPTION_CITY`    | Fuel consumption in city driving (liters per 100 km).                         |
| `FUELCONSUMPTION_HWY`     | Fuel consumption on highways (liters per 100 km).                              |
| `FUELCONSUMPTION_COMB`    | Combined fuel consumption (liters per 100 km).                                 |
| `FUELCONSUMPTION_COMB_MPG`| Combined fuel consumption in miles per gallon.                                 |
| `CO2EMISSIONS`            | The amount of CO2 emissions (grams per kilometer).                            |

### **Dataset Sample**

| MODELYEAR | MAKE  | MODEL         | VEHICLECLASS | ENGINESIZE | CYLINDERS | TRANSMISSION | FUELTYPE | FUELCONSUMPTION_CITY | FUELCONSUMPTION_HWY | FUELCONSUMPTION_COMB | FUELCONSUMPTION_COMB_MPG | CO2EMISSIONS |
|-----------|-------|---------------|--------------|------------|-----------|--------------|----------|----------------------|---------------------|----------------------|--------------------------|--------------|
| 2014      | ACURA | ILX           | COMPACT      | 2.0        | 4         | AS5          | Z        | 9.9                  | 6.7                 | 8.5                  | 33                       | 196          |
| 2014      | ACURA | ILX           | COMPACT      | 2.4        | 4         | M6           | Z        | 11.2                 | 7.7                 | 9.6                  | 29                       | 221          |
| 2014      | ACURA | ILX HYBRID    | COMPACT      | 1.5        | 4         | AV7          | Z        | 6.0                  | 5.8                 | 5.9                  | 48                       | 136          |
| 2014      | ACURA | MDX 4WD       | SUV - SMALL  | 3.5        | 6         | AS6          | Z        | 12.7                 | 9.1                 | 11.1                 | 25                       | 255          |
| 2014      | ACURA | RDX AWD       | SUV - SMALL  | 3.5        | 6         | AS6          | Z        | 12.1                 | 8.7                 | 10.6                 | 27                       | 244          |

## **Model Evaluation**

The model was evaluated using the following metrics:

- **Mean Absolute Error (MAE):** 20.65  
- **Residual Sum of Squares (MSE):** 964.56  
- **R²-Score:** 0.72  

The R²-Score of 0.72 indicates that the model is able to explain 72% of the variance in the fuel consumption based on the features used in the dataset.

## **Technologies and Tools Used**
- **Programming Language:** Python  
- **Main Libraries:**  
  - `scikit-learn` for linear regression model implementation.  
  - `pandas` and `NumPy` for data manipulation.  
  - `matplotlib` and `seaborn` for visualizations.  
- **Development Environment:** Jupyter Notebook  

## **How to Use the Project**

1. Clone this repository:  
   ```bash
   git clone https://github.com/SebasKHE/Car-Fuel-Consumption-Prediction-using-Linear-Regression.git
   ```
2. Install the required dependencies:  
   ```bash
   pip install scikit-learn
   pip install pandas
   pip install matplotlib
   pip install seaborn
   ```
3. Open the Jupyter notebooks:  
   ```bash
   jupyter notebook notebooks/simlpe_linear_regression.ipynb
   jupyter notebook notebooks/multiple_linear_regression.ipynb
   ```
4. Run the cells to train the model and evaluate its performance.

## **Conclusion**
This project demonstrates how **simple linear regression** can be applied to predict the fuel consumption of cars based on several vehicle-related features. The model's accuracy can be improved with more complex techniques and additional data features.

---
