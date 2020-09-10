# Ford_Bike_Communicating_Findings: (January-December 2018 data files)

# Dataset: https://s3.amazonaws.com/fordgobike-data/index.html 
2017-fordgobike-tripdata.csv
The dataframe consists of 15 different variables such as duration_sec (seconds)
start_time,end_time,Start Station ID,start_station_name,Start Station Latitude,Start Station Longitude,End Station ID
End Station Name,End Station Latitude,End Station Longitude,Bike ID,User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
member_birth_year,member_gender
It contains 519700 bike rides. Ages in dataset from 20 to 60 takes 95% of the users in dataset.
i have more outliers between 60-more than 120. So, i removed users more than 60 years as a cleaning to make data more reliable .
-I generated new features such as Month,Month_Name,days,Hours,Minutes and Age groups becuse i need to comaper beween them and user type to get more analysis
like duration_sec and age group or gender type or user type and so on and calculaye the time in minute to knoq what the specific time type of gender spend on each trip and so on 


###############################################################################################
#                              Summary of Findings:                                           #
###############################################################################################

For Data Analysis, I considered 2017 dataset  (2017-fordgobike-tripdata.csv)
from June to December and found very interesting facts from Exploratory Data Analysis.
 In 2017 people took around 519700 bike rides.
 In which 20-60 yrs took around 453159  bikes rides. 
 22-25 and 45-45 years Age group users are rapidly growing compared to other user groups. 
- month of october is highest number appear  and june is least one appear. so starting from July to December the frequently ratio is higher and  
- Subscriers use the service during days from Monday to Friday  between 7-9 am and 5-7pm are busy hours for daily bike riders to goto the work and returns into their home.
- frequanyly of ride the bike is 76.5% male 22.1% female ,1.4% other 
- 88% of Subscribers are using bike service compare to customers using bike service with 11.7%.
- the system is used mainly around 8-9am and 5-6pm when people get to and gat back from work.
- hourly usage of the bike sharing system to know what the specific time we need to know to push more offer on it to make a good motovition
- people use this service when they has a vacation as well.
- the mean of the ages is 39.59 so most of them beteen 25-45 more than other
- user type frequently 89% subscriber ,11% customer
- customers increased from July to October that in the summer and both subscribers and customers service decrease during winter season.
- the male more than gender type with customer and subscriber but the female rate on customer around the 50% but on subscribe i think the rate close to 30%
- the males are using the system more than females and others However, the ratio is much smaller between males and females for customers around 50% and in subsribe around 30%
- the age between 25-45 more than any period and from 45-50 is second one higher on the subscriber
- the ages between 25-45 more than on the both side of user types 
- the ages between 45-55 higher on the subscribe rather than customer 
so i thing this age related by the mans on the moderate ages and they almost married and have a good job so they subscribers because they have stable life reverse on the customer user during all months almost the same number 
- most of their take more time trip on the vactions days on sat and sun days and the pinter less almost of the reminder days on the week

###############################################################################################
#                          Key Insights for Presentation:                                     #
###############################################################################################
- For this  Data Analysis, First I started exploring data-set with People age some of them has over 60 years so i put them as outliers . 
For Analysis purpose I decrease  dataset to under than 60 years age people.
i used three types of visualization 

- univariate i know the most frequesny appear is the subscribers more than customer 
- biviaraite i compare and make corroletion co-effection between between this feature (categorical and some features like numerical featurs and categorical feature so i used bar char to make this investigation and retrieve more information from this relations like in the 
(usertype and gender the male is the heiger rate used the bike)also time using i found most of them not more than 30 min and most frequent appear on the morning when they went to work and the time of return back from the work and also as per month i found the july to october most frequency appear on oth of user type
- multivariate i used more than feature to compare also used Polishing Plots to Polishing the data to be good way in data explanatory
so used for example the relation between month name and user_type group of categories ages so i make some idea at the beginning to retrieve that information 
like extract the age from the birthday and grouped them into more groups and so on ,

