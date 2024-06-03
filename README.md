# Brief

Cyclistic is a bike-share company that launched in 2016 and is based in Chicago. It operates 5,824 bicycles across 692 docking stations. It offers flexible pricing plans: single ride passes; full-day passes; and annual memberships. Those customers who purchase single ride or full-day passes are referred to by the company as casual riders while those who purchase annual memberships are referred to as Cyclistic members. The finance team at Cyclistic have concluded that annual members are significantly more profitable than casual users. Lily Moreno, Cyclistic’s director of marketing, believes that the key to future growth lies in maximising the number of annual members.

Cyclistic’s marketing strategy has previously relied on building general awareness of the brand and appealing to broad consumer segments. Moving forward, Lily Moreno believes that there is an opportunity to convert casual riders into members, noting that casual riders are already aware of the Cyclistic program and have chosen it for their mobility needs. Moreno has thus set a clear goal for her department: design marketing strategies that are aimed at converted casual riders into annual members. To do that, the team must first understand how annual members and casual riders differ and what encourages casual riders to convert to annual memberships. Moreno has tasked her Junior Data Analyst with the role of answering the question: ‘how do annual members and casual riders use Cyclistic bikes differently?’. 

To fulfil the task, the following deliverables must be met: 
1.	A clear statement of the business task
2.	A description of all data sources used
3.	Documentation of any cleaning or manipulation of data
4.	A summary of the analysis
5.	Supporting visualisations and key findings 
6.	Offer three recommendations based on the analysis
   
# The Business Task

Cyclistic is seeking to boost its profits by running a marketing campaign to convert non-recurring customers to annual memberships. The aim of this study is to analyse historical ride data to understand how non-recurring customers and members use the service differently so that Cyclistic may understand what drives customers to subscribe and subsequently direct a marketing campaign to convert these customers. 

# The Data

(**Note**: Cyclistic is a fictional company and makes used of the data which is originally provided by Motivate International Inc. and may be accessed here and used under the license agreement.) 

This study utilises the previous full-year (2023) Cyclistic ride data. The dataset contains ride information such as the starting and finishing time and location, the type of bike used, and the membership status of the user. It has been stripped of any data which may be used to identify customers. The 2023 dataset contains data on a total of 5,719,877 individual rides.

The raw data may be accessed [here.](https://divvy-tripdata.s3.amazonaws.com/index.html)

Summary of changes made to the raw dataset: 
| Change | Description |
| ------ | ----------- | 
| Compiled raw datasets | The raw data, available in distinct monthly comma-separated values files (.csv), was combined to create a single .csv file containing data for the full year 2023. |
| Ordered chronologically | The data were ordered chronologically. |
| Addition of 'day_of_week' column | A new column was generated that contained the day of the week that each ride was conducted on. | 
| Addition of 'ride_length' column | A new column was generated that provided the length of the corresponding ride in minutes. |
| Removal of negative ride_lengths | Any data that had a negative ride length was dropped from the data set. |
| Removal of outliers | Outliers were defined as those who were in the 1st and the 99th percentile of the ride_length data and were dropped from the table as they were not seen to be legitimate data points. |

# Presentation
[Link to presentation (hosted on OneDrive)](https://1drv.ms/p/s!AsJSX1V3eGPe9wGpaJEe8EyyUJV4?e=mSLxwV)
# Dashboard
[Link to dashboard (hosted on Tableau Public)](https://public.tableau.com/views/Cyclistic_17165555896180/FinalDash?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)

