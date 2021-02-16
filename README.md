# Farm Wind Power Prediction Hackathon at Devpost's [Climate Crisis Hackathon](https://climate-crisis.devpost.com)

We created a python notebook that cleans the data up and uses a simple keras deep learning model to predict the wind power 6.5hrs into the future. It requires the last 500mins of wind measurements and the forecasts from the 500m mins before the target time up to the target time.

i.e. if the time was 11:00, our model would predict the wind power at 17:30. To do so it would use the hourly forecasts between 09:10 (500 mins before 17:30) and 17:30. So that's the 9am forecast, the 10am forecast, etc. It also uses the last 500mins of wind measurements. So that's all the wind speed measurements since 02:40 (11am - 500 mins = 02:40am).

It only attempts to predict the first 6.5hrs of the dataset 3 data as to do more requires more wind measurements, which were not released for the challenge but would be available in a real scenario.
