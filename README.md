# "Making of" Data Visualization for the Mayor of The City of Chicago.

Chicago experiences roughly 3,000 crashes annually between motor vehicles and pedestrians, about 800 of which involve children.The City of Chicago started enforcing automated speed violations around the children's Safety Zone and violations data is available from 1st of July 2014 [Source](https://www.chicago.gov/city/en/depts/cdot/supp_info/children_s_safetyzoneporgramautomaticspeedenforcement.html)

I have downloaded the speed violations data of the City of Chicago from the [city's website](https://data.cityofchicago.org/Transportation/Speed-Camera-Violations/hhkd-xvj4) which contains speed violations from Q3-2014 to Q1-2019.

I prepared a [visual presentation](https://public.tableau.com/profile/srinivasan.vasudevan#!/vizhome/InduvidualProject-ThreeAspects/ThreeAspects) for the Mayor of the City of Chicago. The visual presents the three important aspects namely interesting story from the data, non-trivial information and unexpected story from the data.

I will dive in to the "making of" this visualization.

The first aspect is telling an interesting story from the data. The dataset contains information such as Address of the speed light camera, X and Y co-ordinates of location the camera, Date of Violation, Camera ID, latitude and longitude of camera location. I wanted to give an overview of the data in terms of total violations by "time" to review, how the city has performed over the years since the start of the program. I initially chose the columns as month, year and bar graph which provided a great detail of the data but it was lot of information to digest. Picture-1 shows the result graph. ![alt text](images/Overview-1.png "test")

This will give the mayor a review and glance to the future of this program at a 1000 ft height. I started with a pie chart thinking we have 4 quarters in a year.

