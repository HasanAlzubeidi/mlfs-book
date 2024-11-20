# Air quality prediction in Stockholm Sant-Eriksgatan 83 
This project is the first assignment in the ID2223 course. The aim of this lab is to predict the air quality using weather features.  
The main work is done in the notebooks/ch03 directory, where the involved files are:

notebooks\ch03\1_air_quality_feature_backfill.ipynb

notebooks\ch03\2_air_quality_feature_pipeline.ipynb

notebooks\ch03\3_air_quality_training_pipeline.ipynb

notebooks\ch03\4_air_quality_batch_inference.ipynb

A brief description of how it works can be started from the 1_air_quality_feature_backfill.ipynb file:

In this file we start by picking an air quality sensor from https://waqi.info/ in our case it was Sant-Eriksgatan 83 in Stockholm that we chose. From this sensor, we download the historical data to be used later in the training. Save the sensor URL and AQI API key so it can be accessed from the code automatically.  The data that we have from the AQI is daily air quality is PM2.5 which are atmospheric aerosols with a maximum diameter of 2.5 micrometers. We got 2200 data points daily, but some of them were missing so dropping out the missing data points was necessary. The next step was to download the weather data for the city of Stockholm. Now we have the data ready so we can save these to Hopsworks by inserting the data to the feature group. 
