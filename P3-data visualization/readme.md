# Ford_Bike_Communicating_Findings:

# Dataset: https://www.lyft.com/bikes/bay-wheels/system-data 
201903-fordgobike-tripdata.csv
The dataframe consists of 256299 trips and 14 different variables such as 
1- duration_sec             
2- start_time              
3- end_time                    
4- start_station_id           
5- start_station_name         
6- start_station_latitude      
7- start_station_longitude 
8- end_station_id              
9- end_station_name           
10- end_station_latitude        
11- end_station_longitude    
12- bike_id                     
13- user_type                 
14- bike_share_for_all_trip   
It contains 256299 bike rides.

###############################################################################################
#                              Summary of Findings:                                           #
###############################################################################################

For Data Analysis, I considered 2019 dataset  (2019-3-fordgobike-tripdata.csv)
from June to December and found very interesting facts from Exploratory Data Analysis.
 - this data_type not match the real because the start time is date data_type and this appear as object so we need to conert it the true data type
 - One interesting way we can apply bar charts is through the visualization of missing data. We can use pandas functions to create a table with the number of missing values in each column.
 - tidy format start_time include the dd-mm-yyyy and time 00:00:00 so we can extract day and month and years for separate coloumn also the time to now i will splite more coloumn like day and month and year and specific day to make deep analysis
 - I'm most interested duration_sec to know what the specific time spend on each trip and we can compare it with another feature like the extraction feature i do above so this very interesting feature for me
 - i expect the duration time start_time which i split it into four column to make deep specification to make good analysis also bike_share_for_all_trip to also user_type
 
 
###############################################################################################
#                          Key Insights for Presentation:                                     #
###############################################################################################
- For this  Data Analysis, First I started exploring data-set with 
- Univariate Exploration
There was one unusal points for the duration_sec,because after 2500 sec around 41.6 minute i see little number apprear also the beging hour of the day at am between 1 am to 6 am also the number of has bike_share_for_all_trip is very low
and There was one unusal distribution for the duration_sec after 2500 no more long trip very little number
- Bivariate Exploration
the relationships observed in this part of the investigation the user_type because in this feature i really know more information when i test this feature in univariate visualizaion and bivariate and multivariate visualization so in univariate i know the most frequesny appear is the subscribers more than customer and on biviaraite i compare and make corroletion co-effection between between this feature (categorical and some features like numerical featurs and categorical feature so i used barchar to make this investigation and retreive more information from this relations like in the time using i found most of them not more than (3000/60)50 min and most frequent appear on the morining when they went to work and the time of return back from the work 
i extract the year and month and days and hour and specific days  from the strart time for the trip 
- Multivariate Exploration
i observed the strong relationship between bike_share_for_all_trip and duration_sec and user_type because we want to looking for how the duration time effective by user type and bike_share_for_all_trip and i observed time duration very high with custemor but they not has any permission to bike_share_for_all_trip chance so for subsciber have short trips but they used to bike_share_for_all_trip
and i observe also 
duration_sec
user_type
day
hour on the feature of the days ---->Saturday and sundry is the high time duration because this employee vacation because remider the week normal checivement like goto work from monday to friday it the same rate although the customer make long trips on the feature of the hours---->regarding for the figure before i see the customer not stable rate some of peak pint and some down values of duration per sec but on subscriber we see from 9 am to 11 pm the same rate of time except the 1 am is the higher point on both user_type