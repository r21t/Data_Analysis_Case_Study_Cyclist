# Data_Analysis_Case_Study_Cyclist
This is my first project/Casestudy on Data analysis. This is a case sudy that i got from Google Data analysis certification from coursera.
___________________________________
## Introduction

Welcome to the Cyclistic bike-share analysis case study! In this case study, you will perform many real-world tasks of a junior
data analyst. You will work for a fictional company, Cyclistic, and meet dierent characters and team members. In order to
answer the key business questions, you will follow the steps of the data analysis process: ask, prepare, process, analyze, share,
and act. Along the way, the Case Study Roadmap tables — including guiding questions and key tasks — will help you stay on the
right path.
By the end of this lesson, you will have a portfolio-ready case study. Download the packet and reference the details of this case
study anytime. Then, when you begin your job hunt, your case study will be a tangible way to demonstrate your knowledge and
skills to potential employers.
________________
## Scenario
You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of
marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your
team wants to understand how casual riders and annual members use Cyclistic bikes dierently. From these insights, your team
will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve
your recommendations, so they must be backed up with compelling data insights and professional data visualizations.
Characters and teams

* Cyclistic: A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself
apart by also oering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with
disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8%
of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to
work each day.

* Lily Moreno: The director of marketing and your manager. Moreno is responsible for the development of campaigns and
initiatives to promote the bike-share program. These may include email, social media, and other channels.

* Cyclistic marketing analytics team: A team of data analysts who are responsible for collecting, analyzing, and reporting
data that helps guide Cyclistic marketing strategy. You joined this team six months ago and have been busy learning about
Cyclistic’s mission and business goals — as well as how you, as a junior data analyst, can help Cyclistic achieve them.

* Cyclistic executive team: The notoriously detail-oriented executive team will decide whether to approve the
recommended marketing program.
______________________________
## About the company

In 2016, Cyclistic launched a successful bike-share oering. Since then, the program has grown to a fleet of 5,824 bicycles that
are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and
returned to any other station in the system anytime.
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One
approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and
annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who
purchase annual memberships are Cyclistic members.
Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the
pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will be
key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a very
good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and
have chosen Cyclistic for their mobility needs.
Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do
that, however, the marketing analyst team needs to better understand how annual members and casual riders dier, why casual
riders would buy a membership, and how digital media could aect their marketing tactics. Moreno and her team are interested in
analyzing the Cyclistic historical bike trip data to identify trends.
_________________________________________________________________________________________________________________________________________________________________________________

There are 6 steps involved in this analysis.
1. ASK
2. PREPARE
3. PROCESS
4. ANALYZE
5. SHARE
6. ACT
____________
## ASK
### Three questions will guide the future marketing program:

1. How do annual members and casual riders use Cyclistic bikes dierently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?
_______________________________________________________
## PREPARE

Prepare stage is about Data generation , Collection , Storage and Management of data.

### Where is the data located?
The data that i have acquired is from - https://divvy-tripdata.s3.amazonaws.com/index.html. I have the license to use it.


### IS DATA ROCCC ? - 
1. **R**eadable
2. **O**riginal
3. **C**omprehensive
4. **C**urrent
5. **C**ited

Yes, the data is ROCCC.

### How are you addressing licensing, privacy, security, and accessibility?
***Please refer to license before using it - https://www.divvybikes.com/data-license-agreement (Note: The datasets have a different name because Cyclistic is a fictional company. For the purposes of this case study, the datasets are appropriate and will enable you to answer the business questions. The data has been made available by Motivate International Inc)***

### How did you verify the data’s integrity?
Data has beem provided by the Google Certification - and the data is accuarte.

### How does it help you answer your question?
Data Contains the required columns to answer the questions that are required.

### Are there any problems with the data?
After through check, I have not found any issues with the data.
______________________________________________
## PROCESS
 Process is to perform **Data Cleaning** and check for **Data Integrity**

### What tools are you choosing and why?
* using **Excel** to some basic columns using the formuals in the excel
* Using **Python** for the data cleaning and data analysis.

#### What steps have you taken to ensure that your data is clean?
* There are missing data in the column names of  - start_station_name, start_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng.
* For the Final dataframe, Not included start_station_name, start_station_id, end_station_name, end_station_id. and hence not removing the data.
* In this analysis we are not plotting any maps using start_lat, start_lng, end_lat, end_lng, hence having the data untouched and not removing the null values.
*	No null values found in other columns.

#### How can you verify that your data is clean and ready to analyze?
* Have used pandas isnull() function to check for any null values, Which were not found.

#### Have you documented your cleaning process so you can review and share those results?
* The data cleaning has been done in python and has a section seperately in the jupyter notebook.

#### Columsn added in from the excel sheet
*	Added a new column named – ride_time, describes the ride time in terms of minutes and hours.
*	Added a new column named – day_of_week , this describes the day on which the ride is being taken place on – 1 = Saturday - - - - - - 7 = Sunday. [ used = weekday(column_name , 1)].
* Sorted the data based ascending order for the column started_at.
_________________________________________________________
## ANALYZE 
* This is the stage for data exploration, visualization and analysing the data takes place.

#### How should you organize your data to perform analysis on it?
* Organized the data by adding new columns which contains the extracted data from the other columns - like month, day, year, ride_length, ride_length_minute e.t.c seperately.

#### Has your data been properly formatted?
* Chekced all the data types before analysis and changed the data types as required.

#### What surprises did you discover in the data?
* Discovered that some columns are not in the required format. Changed the same to the required format.

#### What trends or relationships did you find in the data?
* Found many differences on how casual riders and member riders are availing the cycles.
* Found some key insights through visualization.

#### How will these insights help answer your business questions?
* These insights will help the business to get new memberships.
* The business can know where to target the audience and get the memberships.
* Suggestions given on how to use social media platform to get more memberships.

________________________________________________
## Share

#### Were you able to answer the question of how annual members and casual riders use Cyclistic bikes differently?
*Yes, by analyzing the data in different ways i was able to answer how casual riders differ from annual member riders

#### Who is your audience? What is the best way to communicate with them?
Stakeholders/Audience 
* Lily Moreno -Manager and director.
* Cyclistic executive team

The best way to communicate is to create a presentation, with the visualizations.

#### Can data visualization help you share your findings?
Yes, Data visualization helps to share the findings.

____________________________________________________
## ACT

#### My top three recommendations based on analysis
* The Casual_riders AVERAGE ride_length is more than the Member_riders. We can use this to get the casual riders signup for the membership, Where they can be benifited more than the mmeber_riders.
* June , July and August Average ride lengths of the causual_riders are more than the overall year. Can add small offers to get them to signup for membership at Cyclist.
* Anouncing that members can have offers on Weekends can attract casuals as more casuals are riding on weekdays than weekends.
* Should focus on casual riders on months May,July and August as the usage is on peaks in that months.
* 
#### Other recomendations.
* Cyclist Company can push notifications to become a memebr of Cyclist to casual riders on the months of MAY, JULY and AUGUST as the usage is peak on those months.
* Cyclist Company should show how casual riders are missing out on membership features by showing the casual vs membership differences.
* Company Can add small offers in the month June , July and August as the Average ride_lengths of the causual_riders are more in those months and members aswell.




