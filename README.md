# Ford GoBike Data Exploration
## by Mayssa Soussia


## Dataset

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. It can be found through this [link](https://www.kaggle.com/datasets/ahmedmohameddawoud/ford-gobike-system-data).
The data was preprocessed, nan values were dropped and only records with valid values were remained as well as many variables were converted to the right datatype. 


Once cleaned, the data consists of 60606 records in the dataset with 16 columns (duration_sec, start_time, end_time, start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude, bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip).

A new column was also created which is part_of_the_day where hours were extracted from start_time column to compute the values morning, afternoon, evening and night. 


## Summary of Findings

In the exploration, I found that duration of trip can be varying between user types where subscribers tend to have shorter trips than customers. However, the gender doesn't have much of effect on duration, males and females almost have the same average of trip duration. On the other hand, duration seemed to have a moderate positive relationship with member_birth_year, users who are younger tend to have longer trips than older users.  


## Key Insights for Presentation

For the presentation, I focused on the distribution of some categorical 
variables and their relationship with the variable of interest, then 
investigated if there is a correlation between duration and the numeric 
variable member_year_birth. 

I started by introducing the categorical variables: member_gender, user_type and 
part_of_the_day. For this matter, I used the bar charts. Afterward, I used the violin 
plots to compare these variables against duration_sec and then used the scatter plot to 
seek what kind of relationship between the feature of interest and age. 
In the last part, I used the multivariate analysis to see if there is any additionnal 
patterns or trend between user_type, part_of_the_day against the feature of interest
duration_sec. 
