# (Go-Bike Dataset)
## by (Alexis Kurtz)


## Dataset

> The Ford Go-Bike dataset contains 183412 records of bike rentals in the bay-area in February 2019 and divided between 16 columns. The dataset gives informations about the attributes of each trips such as the duration, the start and end station (including location data) and about users such as the date of birth or gender.

> The following wrangling issues were tkaen care of :

> Quality issues

> - 'start_time', 'end_time' to convert in date format
> - 'start_station_id' and 'end_station_id' to convert in text, remove '.0'
> - Remove the 197 rows with missing data (in start_station_id/start_station_name/end_station_id/end_station_name)
> - Rename 'duration' in 'duration_sec'
> - Drop rows where calculated 'age' is more than 100
> - Drop too extreme values for distances columns

>Tidyness issues

> - Add 2 new columns calculating duration in minutes and hour ('duration_min', 'duration_hour')
> - Add an 'age' field calculated on 'member_birth_year' (based on start_date)
> - Create new columns extracting 'hour of the day', Weekday, Month and Year for both start and end of trip
> - Creation of a new categorical variable 'Weekends'


## Summary of Findings

> Throughout this study, we have been able first  to 'draw a portrait' of average user of the Go-Bike service on February 2019; usually male, subscriber to the service and below its 40's.

> Then, we pointed that the weekday variable has an influence on bike rental trends and not in the way you would expact, as trips tends to be be less numerous on weekends but a bit longer in duration. 

> Finally, we were able to establish that the portrait of go-bike users was not consistant between business days and weekends as more customers (non-subscribers) usethe service out of business days. In the same 'spirit'; less women use the go bike in weekends than business days.


## Key Insights for Presentation

> The presentation will mostly communicate on the impact of weekday on go-bike users practices, using the plots made for the multivariate exploration part.