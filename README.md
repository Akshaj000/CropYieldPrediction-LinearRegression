# CropYieldPrediction-LinearRegression


Crop yield prediction is one of the challenging tasks in agriculture. It plays an essential role in decision making at global, regional, and field levels.   
  
We have removed categories and id parameter from the dataframe. This is because category contained multiple categories which was complicated to represent as numbers. We handled Nan value for each column by replacing it with the median of that column. We had to replace one of the uv value which crossed 5000 which effected the data representation.
  
The prediction of crop yield here is based on water, fertiliser_usage, pesticides, area, uv and region parameters. We have used Linear regression to create various models with combination of various such parameters. We calculated root mean square error for each model and found the best model with least rmse. We are also checking r square value to get the score of each model.