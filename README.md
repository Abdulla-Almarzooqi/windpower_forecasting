# Wind Turbine Power Forecasting Based on Time Series Models

## Description
Our primary objective is to evaluate the efficiency of various models by comparing the models with the baselines and identifying the most reliable one for producing dependable power predictions. 

## Installation
  ```
  # Clone the repository
  git clone https://github.com/Abdulrahman88899/windpower_forecasting.git
  cd windpower_forecasting
  ```
## Setup Instructions
    
  1. Create a conda environment:

     ```
     conda create -n windpower_forecasting
     conda activate windpower_forecasting
     ```

  2. To install the required libraries, run the following command:

   ```
   pip install -r requirements.txt
   ```

## Datasets
1. Turkey dataset:
   The Wind Turbine Scada Dataset from Turkey is a comprehensive collection of wind speed, wind direction, and generated power readings   taken every 10 minutes throughout 2018 `T1.csv`. Key features of this dataset include Low Voltage Active Power (LV ActivePower), which displays the current power output (in kW); Wind Speed at turbine height (in m/s) that is used to generate electricity; Theoretical Power Curve, which shows the theoretical power values (in kWh) based on manufacturer-specified wind speeds; and Wind Direction (in degrees °), which automatically adjusts the turbine direction based on wind direction at turbine height. Also, you can find the [dataset](https://www.kaggle.com/datasets/berkerisen/wind-turbine-scada-dataset).

2. Texas dataset:
   The provided full-year hourly time series are simulated using the National Renewable Energy Laboratory (NREL) software for a location in Texas, US. It has perfect data completeness and no noisy data, which are challenges that hinder forecasting tasks with real datasets and distract from the goal `TexasTurbine.csv`. The dataset contains various weather features that can be analyzed and used as predictors. These features are System Power Generated (in kW), Wind Speed (in m/s), Wind Direction (in degrees °), Pressure (in atm), and Air Temperature (in °C). Also, you can find the [dataset](https://www.kaggle.com/datasets/pravdomirdobrev/texas-wind-turbine-dataset-simulated?select=TexasTurbine.csv).

## Evaluation
1. This notebook, ' ML703project_dataset_1.ipynb, ' refers to the comparison between the models (LSTM, GRU, RNN, and CNN-1D) for the particular Turkey dataset.
2. This notebook, ' ML703project_dataset_2.ipynb, ' refers to the comparison between the models (LSTM, GRU, RNN, and CNN-1D) for the particular Turkey dataset.

## Acknowledgements

1. For the three-time series models (LSTM, GRU, and RNN), we inspired [to this code](https://www.kaggle.com/code/alejopachons/lstm-predictions-wind-turbine-scada/notebook). We made the following changes:
    - Tweaked the hyperparameters completely to be suitable for the datasets.
    - Tried different models (GRU and RNN)
      

