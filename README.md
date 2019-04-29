# "Making of" Data Visualization for the Mayor of The City of Chicago.

Chicago experiences roughly 3,000 crashes annually between motor vehicles and pedestrians, about 800 of which involve children.The City of Chicago started enforcing automated speed violations around the children's Safety Zone and violations data is available from 1st of July 2014 [Source](https://www.chicago.gov/city/en/depts/cdot/supp_info/children_s_safetyzoneporgramautomaticspeedenforcement.html)

I have downloaded the speed violations data of the City of Chicago from the [city's website](https://data.cityofchicago.org/Transportation/Speed-Camera-Violations/hhkd-xvj4) which contains speed violations from Q3-2014 to Q1-2019.

I prepared a [visual presentation](https://public.tableau.com/profile/srinivasan.vasudevan#!/vizhome/InduvidualProject-ThreeAspects/ThreeAspects) for the Mayor of the City of Chicago. The visual presents the three important aspects namely interesting story from the data, non-trivial information and unexpected story from the data.

I will dive in to the "making of" this visualization.

## Interesting Story

The first aspect is telling an interesting story from the data. The dataset contains information such as Address of the speed light camera, X and Y co-ordinates of location the camera, Date of Violation, Camera ID, latitude and longitude of camera location. I wanted to give an overview of the data in terms of total violations by "time" to review, how the city has performed over the years since the start of the program. I initially chose the columns as month, year and bar graph which provided a great detail of the data but it was lot of information to digest. Picture-1 below shows the graph. ![alt text](images/Overview-1.png)

I thought showing variation by year and month presents lot of details but the mayor won't be able to make out anything from this. I wanted to try with year and quarter (which best represents seasons). Pie charts are great in representing quadrants. I tried with Pie charts. 
Picture-2 below shows the graph. ![alt text](images/Overview-3.png)

This pie chart is not able to reflect the seasonal difference, any improvement over years and future forecast accurately. The mayor needs to review this pie chart very closely to understand the details. In a nutshell, this pie chart is not engaging and not able to draw attention. I think using a bar graph and correctly arranging the columns season first and then year will portray the story well. Picture-3 below shows the Overview in an interesting way.![alt text](images/Overview-final.png).

This bar graph shows the decreasing trend of total violations for every quarter across years. This graph also clearly show that, Q1 quarter which is the winter season incurred least violations for all the years. The forecast is also clearly shown with the forecasted number of violations in each years (2019 and 2020).
A line graph might not be a good choice because it will not be able to tell the magnitude of change for all the years from base 0. I like the way this graph portrays an interesting story of how the program has been working since the start of the program across various seasons and how it will work in the near future as well.

## Non-trivial Story

## Unexpected Story




