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

(**Note**: Cyclistic is a fictional company and makes used of the data which is originally provided by Motivate International Inc. and may be accessed [here](https://divvy-tripdata.s3.amazonaws.com/index.html) and used under the license agreement.) 

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

# The Analysis

Upon analysis, the following observations were noted about Cyclistic casual users:
1. Casual users prefer electric bikes
2. Casual users took longer rides​ on average
3. Casual users are part of the evening commuter crowd​
4. Casual users are more active on weekends​
5. Casual users are more active during the summer​
6. Casual users visit more touristic and recreational locations

By taking what we know about our casual users, we can develop a story to describe who they are. 

> # The Regular
> They're the part of the casual user base who ride during the week, in commuter hours. They use the service regularly to get from A to B, but they haven't yet made the leap to an annual subscription. They're probably residents of Chicago. 
> * Resident​
> * High familiarity with Cyclistic​
> * Often uses Cyclistic for commuting or recreation​
> * Has not yet made the leap to annual membership​
> * High potential for conversion

> # The Opportunist
> The part of the casual user base who's more active outside of commuter hours, during the week or on weekends. They visit more recreational and touristic locations. They use Cyclistic sporadically. They're probably residents of Chicago.
> * Resident​
> * Low familiarity with Cyclistic​
> * Sporadically uses Cyclistic for getting around the city and recreation​
> * Potential for conversion, but we must first increase their frequency of use

> # The Tourist
> The part of the casual user base who are more active during summer, on weekends, during the middle of the day. They're not residents of Chicago, and are in town for a short while and are trying out Cyclistic to get from A to B during their stay. They like to visit the touristic and recreational parts of Chicago.
> * Non-resident​
> * Short stay in Chicago ​
> * Unlikely to subscribe annually​
> * High demand for mobility during stay​
> * Potential for short-term capture

# Recommendations

By taking what we learned about our customers during the analysis stage and the customer profiles we built upon that information, we can begin to develop a tailored approach to each segment: 

> # The Regular
> Ripe for conversion. We just need to give them a nudge to subscribe. Repeat exposure to the member benefits should drive subscriptions. Success will be measured by the conversion rate for this segment.
> * **E-mail campaign:** targeting ‘ready-to-subscribe’ regular users highlighting benefits of subscribing, e.g., cost savings, health benefits, avoiding city traffic, etc. ​
> * **In-app promotions:** In-app promotions, e.g., flash discounts for subscriptions, highlight cost savings based on their usage, etc.
> * **Surge pricing:** Introduce surge pricing for casual users. Price will increase during peak hours providing economic incentive for regular commuters and weekend users to subscribe. ​

> # The Opportunist
> Occasionally uses the service. Unlikely to subscribe at this stage. We’ll have to convince or incentivise them to use the service more, and then we can convert. Repeat exposure will increase their familiarity with the brand and hopefully boost usage. Success will be measured by the usage rate of casual users (how many ride minutes are they using per week?).  
> * **E-mail campaign:** E-mail campaign targeting ‘early-stage’ registered users highlighting benefits of continuing to ride with Cyclistic, e.g., health benefits, avoiding city traffic, environmentally friendly, etc. Pair with offers and discounts.
> * **In-app promotions:** In-app promotions, e.g., flash discounts for subscriptions, highlight cost savings based on their usage, challenges, fitness programs, etc.

> # The Tourist
> Non-resident. Has high mobility needs during their stay. Highly unlikely to subscribe annually, but there is potential to capture their custom for the short term. We'll do this by introducing the service to them via a free trial (one-day pass), and then upsell at the end of this free trial to a one-week pass. Success will be measured by the return-rate of free-trial users and of the uptake of one-week passes.
> * **Physical advertising:** Physical media campaign in the busiest stations for casual users. Highlight perks of using Cyclistic (avoid traffic, experience city, etc.). Pitch with free daily pass to introduce users to the service. 
> * **Weekly pass:** Introduce a weekly pass to capture the ‘tourist/visitor’ segment. This will incentivise repeat use across their visit while increasing revenue. 
> * **One free daily pass:** Offer QR codes for one free daily pass to new users. This will allow the product to speak for itself. Follow up by pitching weekly pass to secure custom. 
> * **Appearing in tourism searches (SEO/Google Ads):** Targeted promotion to internet users searching for tourism in Chicago (SEO/ads). ‘Visiting Chicago? Try Cyclistic.’ Drive uptake via free one-day passes. 

# Presentation
[Link to presentation (hosted on OneDrive)](https://1drv.ms/p/s!AsJSX1V3eGPe9wGpaJEe8EyyUJV4?e=mSLxwV)
# Dashboard
[Link to dashboard (hosted on Tableau Public)](https://public.tableau.com/views/Cyclistic_17165555896180/FinalDash?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)

