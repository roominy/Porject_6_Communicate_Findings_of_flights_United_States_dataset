# (Dataset Exploration Title)
## by (your name here)


## Dataset

> This dataset that reports flights in the United States, including carriers, airports, times of sechedued and actual arrival and departure delays, and times of reasons for delays. It contains approximately 7,000,000 Flights in 2008.

> Wrangling was done in a seprate notebooks 'download and decompress data file.ipynb' 

>- to download the compressed data file decompress it then save it

> then 'data_cleaning.ipynb'

> where the following was done:
    
    1- The main flights data set &the supporting airports & carriers data sets were loaded
    2- added Dest & the Destation & Origin cities, airports & states  columns containing iata data and rename iata to Origin for joining the main flights & airports tables 
    3- Renamed Code column to UniqueCarrier and  Description to CarrierName for joining the main flights & carriers tables 
    4- Dropped 'TailNum','FlightNum','Diverted', 'ActualElapsedTime','CRSElapsedTime','TaxiIn' & 'TaxiOut' colunms
    5- Converted CRSArrTime, CRSDepTime, ArrTime & DepTime times to time string and gettig Dep & Arr hours
    6- Converted CRSArrTime, CRSDepTime, ArrTime & DepTime string to timedelta
    7- get the Origin & Destination airports, citys and states form airports data by joining the main flights & airports table
    8- Get the flight CarrierName data by joining the main flights & carrier tables
    9- saved the cleaned filghts data as 2008_cleaned.csv in data files folder




## Summary of Findings

>I'm interested in finding out which contribute to the the main feature Depature Delay (DepDelay).

>In this dataset I'm interested in answering the following questions:

>- What time of the year and day that flights are most likely to be dalayed?
>- Which are the top 15 carrier that contribute the most to flights delays?
>- Which are the top 15 airports that contribute the most to flights delays?
>- Which time of the year / states weather delays are most occring?

> *  For the time of the year that flights are most likely to be dalayed:
> - It was found that  for the dalayed flights ratios the most delayes happen during holiday season that and you can see that june and july see to have darker shades this could be due to thra summer vacation starts in June and so does the months form February to April this could be due to Spring Break that spans late February to mid-April, with March being the peak period.
> - Also, dalays are higher in start of all the of the seasons (March for Spring, June for Summer, & December for Winter) except for Fall (September).

>* For the time day that flights are most likely to be dalayed:
> - Generally there's seem to be peak interval for Depature delays between 2:00 PM and 9:00 PM
How day like friday and Sunday seen to have the highest delay percentage in this interval
> - Also there seem to be sudden peaks in Depature delays in 3:00 AM

>* Top carrier that contribute the most to flights delays:
>-  Southwest Airlines  had The highset Departure delayes cocunts while Mesa Airline Inc occupied the 12th place and jet blue had the 14th place while mean wise jet blue has the hights delay meaning. Meaning that although Southwest Airlines Departure delayes cocunts are higher that Mesa Airline's & jet blue's but the amount Mesa Airline's & jet blue delay time are higher than Southwest Airlines.
>- When it comes to Daley that is can be caused & controlled by Airlines for Airline Mesa Airline Inc seems to the worst of in preformance in terms of Carrier delay followed by Hawaiiian Airlines's while for late AirTran Airways Corporation while in for of the Late Aircraft Delay AirTran Airways Corporation followed by United Air Lines Inc. then JetBlue Airways
>- The worst performing air line is Pinnacle Airlines Inc. as its mean of the general Departure daley is higher than the average so deos its Carrier (Airlines) & Late Aircraft Delays.

>* Top  airports that contribute the most to flights delays:
> - All of the top 20 airports  have higher departure delay means than departure delay mean of all airport the same goes for top 20 cities and states
>- None of the top 20 airports and cities have higher departure delay seem to belong to the top 20 airport and cities counts of delayed flights at depature However, The 5 highest departure delay means for airports list seem to agree with 5 highest departure delay means for cities all the 5 all highest departure delay means for airports are in the 5 highest departure delay means for cities receptively

>
>* Time of the year states weather delays are most occring:
> - It was found that most of weather dalay occured during Winter months and scilt in holidays season
> - There is an sudden incease in of weather dalay in the 19th of june and 10th of July when I searched about them found that due to exterrm weather condtions ( a severe thunderstorm in the 19th of june & a high winds and dry conditions for the 10th of July) (weather.gov)
- https://www.weather.gov/otx/July-WeatherHistory
- https://www.weather.gov/ama/june19_2008_severe

>* States weather delays are most occring:
>- All of 15 the highest Weather delay count States belong 20 highest Departure delay count States but in diffrent order However the both agree on Texas being the frist.
> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.


## Key Insights for Presentation

> I'm interested in finding out which contribute to the the main feature Depature Delay .

> In this investigation, I'm interested in answering the following questions:

> - What time of the year and day that flights are most likely to be dalayed?
> - Which are the top 15 carrier that contribute the most to flights delays?

> For the first question, the features will be flight's Depature Delay, Month, Day of Month, Day of the week & Depaturer hour .

> While for the the second question, the features will be flight's airlines, Depature Delay, Airlines Delay & Late Aircraft Delay.

