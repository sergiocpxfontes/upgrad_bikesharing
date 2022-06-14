# Linear Regression Assignment - upGrad
> Build a model for predection of bike rental daily count base on the environmental and seasonal settings


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Methodology](#methodology)
* [Analysis](#analysis)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

BoomBikes is a company that rents shared bikes. Their business has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. They want be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. To achieve their goal they need to understand what factors have impact on demand for bike rentals.

The objective of this project is to:

 - Determine what variables are significant in predicting the demand for shared bikes;
 - Determine how well the significant variables describe the demand.

To achieve we need to create a model to predict the shared bikes demand.

The mode will be based on the Bike Sharing dataset available [here](day.csv) and consists on the following variables:

- instant: record index
- dteday : date
- season : season (1:spring, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2018, 1:2019)
- mnth : month ( 1 to 12)
- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
- weathersit : 
	- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
	- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
	- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
	- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : temperature in Celsius
- atemp: feeling temperature in Celsius
- hum: humidity
- windspeed: wind speed
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->
## Methodology

Creating the model will require the usage of machine learning (more details on https://en.wikipedia.org/wiki/Machine_learning) and to do so, several steps  need to be made to ensure we understand the data and making sure the dataset is ready to be submited to the algorithms. The steps will be executed with a Jupyter Notebook file and will follow the following order:

- Step 0 » Importing the necessary python modules and packages
- Step 1 » Reading, understanding and visualize the data
- Step 2 » Preparing Data
- Step 3 » Training the model
- Step 4 » Residual analisys
- Step 5 » Predictions and evaluations on the test set

## Analysis

Within our analysis we looked at the following variables as to how they correlate to bike rental count: 

  - temp
  - atemp
  - hum
  - windspeed
  - season
  - weathersit
  - holiday
  - workingday

On the [Jupyter notebook file](bikerentalstudy.ipynb) you will find:
  
  - Operations made on the initial data, including:
  	- Data quality checks
  	- Handling of categorical variables
  	- Handling og dummy variables
  - Data visualization based on the variables nature to determine possible correlations
  - Notes explaining the steps and decisions made.

[Here](bikerentalstudy.pdf) you will find our analisys and conclusions (also present bellow) of the Bike Rental study and [here](linearregressionsubjectivequestions.pdf) you will find answers to several questions that are also part of this assignment/project.



## Conclusions
- Conclusion 1 from the analysis
- Conclusion 2 from the analysis
- Conclusion 3 from the analysis
- Conclusion 4 from the analysis

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used

- Jupyter Notebook (6.4.5)
- Python (3.9.7)
  - nump (1.20.3)
  - pandas (1.3.4)
  - matplotlib.pyplot
  - seaborn (0.11.2)
  - sklearn (0.24.2)
    - model_selection (train_test_split)  
    - preprocessing (MinMaxScaler)
  - statsmodels (0.12.2)
    - api
    - stats.outliers_influence (variance_inflation_factor)

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- [1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

## Contact
Created by [@sergiocpxfontes] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
