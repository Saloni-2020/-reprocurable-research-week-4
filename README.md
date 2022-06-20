Synopsis
In this project, we analyze the storm database taken from the U.S. National Oceanic and Atmospheric Administration (NOAA). We estimate the fatalities, injuries, property damage, and crop damage for each type of event (e.g., Flood, Typhoon, Tornado, Hail, Hurricane, etc.). Our goal is to determine which event is most harmful to US population (health) and which event has the largest economic consequences. Our analysis on Fatalities and Injuries conclude that Tornado is the most harmful event in respect to the US health (population). On the other hand, based on the Property and Cost damage, we conclude that Flood has the greatest economic consequences to the US.

Introduction
Storms and other severe weather events can cause both public health and economic problems for communities and municipalities. Many severe events can result in fatalities, injuries, and property damage, and preventing such outcomes to the extent possible is a key concern.

This project involves exploring the U.S. National Oceanic and Atmospheric Administration’s (NOAA) storm database. This database tracks characteristics of major storms and weather events in the United States, including when and where they occur, as well as estimates of any fatalities, injuries, and property damage.

Data
The data for this assignment come in the form of a comma-separated-value file compressed via the bzip2 algorithm to reduce its size. You can download the file from the following link:

Storm Data [47Mb] There is also some documentation of the database available. Here you will find how some of the variables are constructed/defined.

National Weather Service Storm Data Documentation National Climatic Data Center Storm Events FAQ The events in the database start in the year 1950 and end in November 2011. In the earlier years of the database there are generally fewer events recorded, most likely due to a lack of good records. More recent years should be considered more complete.

Questions
The data analysis address the following questions: 1.Across the United States, which types of events are most harmful with respect to population health? 2.Across the United States, which types of events have the greatest economic consequences?

Let’s get to the project
The first step is always loading the necessary libraries to work on the project
![image](https://user-images.githubusercontent.com/88283525/174536003-9345d093-6a50-4f5c-9faf-8e18404040f1.png)
Loading the data into the work space
![image](https://user-images.githubusercontent.com/88283525/174536106-76839348-5163-4c4e-9744-35309acd5318.png)
Data Processing
Analysis 1
Sub-setting the data for analyzing the most harmful event type
Grouping the data by event type
Summarizing the data by the sum of each outcome
Arranging the data in a descending order for fatalities
Choosing the top 10 events causing harm
melting the data so it can be graphically represented right
![image](https://user-images.githubusercontent.com/88283525/174536173-d8d08957-1f98-40dc-a6cf-5d385ed558ab.png)
Bar plot for the most fatal events
![image](https://user-images.githubusercontent.com/88283525/174536254-fb4c1a36-5e25-4826-ba45-885fbc9cb9c2.png)
![image](https://user-images.githubusercontent.com/88283525/174536326-71b039d8-6db8-4d0e-a5fc-6591365a1b51.png)
Selecting the columns needed for the analysis
![image](https://user-images.githubusercontent.com/88283525/174536516-be4e8712-cea5-417c-9bcf-817dd0fa8f20.png)
Transforming the column “PROPDMGEXP” into numbers
![image](https://user-images.githubusercontent.com/88283525/174536593-713b89d0-06cb-4cfd-bebb-6af01c0022db.png)
Change into numeric values
![image](https://user-images.githubusercontent.com/88283525/174536719-6dbb535c-a77b-4a0f-84b1-f97f131383ad.png)
Transforming the column “CROPDMGEXP” into numbers
![image](https://user-images.githubusercontent.com/88283525/174536803-d1965167-9272-4657-a100-b793a45efa66.png)
Changing into numeric values
![image](https://user-images.githubusercontent.com/88283525/174536911-accb85db-52da-4496-8ea4-e89046887d90.png)
making a new columns with the proper CROPDMG & PROPDMG
![image](https://user-images.githubusercontent.com/88283525/174536966-a45230b4-480e-4c16-841c-54925bc0b229.png)
Select the coulmns will be used
Grouping by the event type
Summarizing the total crop damage and the total property damage
Making a new column by the total damage
Arrange by the total damage in a descending order and selecting the only top 10 results
![image](https://user-images.githubusercontent.com/88283525/174537053-8583ae6a-27ca-4826-b016-d8ddaf11d36f.png)
Reshaping the data to be represented on a bar graph
![image](https://user-images.githubusercontent.com/88283525/174537136-aab306ba-516e-4719-8da3-dbc1030dba60.png)
Bar plot for the most fatal events
![image](https://user-images.githubusercontent.com/88283525/174537415-8ee379cb-5a4e-4b32-8b39-c77fe83bd957.png)
![image](https://user-images.githubusercontent.com/88283525/174537462-5843b443-3091-4610-8fb9-f8a93448e677.png)














