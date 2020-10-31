# BGD-G3

There are four separate folders in this repository.

1) the sql folder contains a txt file, describing queries that we used for data management. For data management and cleaning, we have checked for the duplicate values and missing data in every table and finally join all tables to gether based on a common attribute (block code) and created three output for the next step of the project.

2) The input folder contains one zipped folder. This is actually the result of the previous part (data management within SQL). The zipped folder has three separate CSV files. The CSV files are the main data set, the weekly aggregated dataset, and the monthly aggregated dataset.
 
3) The Processing folder contains the file called Modelling.ipynb. This file contains python codes related to the data analysis and preprocessing.
  - At first we did a preprocessing on the main data set.
  - After the initail preprocessing on the main dataset, becouse of the problems with the actual data set (for example many records have a value of one), we have decided to aggregate our original dataset.
  - So we have aggregated our original dataset by once by month and again by week. then we developed random forest regression models for each one of these two datasets (weekly aggregated dataset and monthly aggregated dataset). The reseain behind this decision was that we wanted to investigate the impact of data aggregation of the final model and to see how the regression models will react with these two different datasets and of course to use the model with better result.
  - then we explained the process of removing outliers from two datasets (weekly aggregated data and monthly aggregated data). 
  - finally,this file contains data, code, and the resuslt of four separate regression models for the weekly and monthly aggregated data with outliers and without outliers. so you could see the result of random forest regression model and it's associated error for four scenarios (with four different datasets, weekly and monthly aggregated data with and without outliers) and compare the results.
  - comments are associated along with the code snippet.

4) The Output folder contains results of the regression model. The results are listed inside the folder.


