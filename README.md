# -Airplane-Crashes-and-Fatalities-since-1908
This is a Capstone project for Microsoft #NG30daysoflearning 

___
# Project objective : Problem stament
* The goal of our project is to analyze the dataset, develop a visualization aspect which shows the trends of Airplane Crashes and number of Fatalities. We have considered answering some of the questions below:
* What is the Total number of Airplane Crashes from 1908 to 2009?
* what is the Total number of Fatalities from 1908 to 2009?
* What is the Total number of Passengers involved in the Crashes from 1908 to 2009?
 * What is the Fatality rate?
* How many planes crashed per Year? how many people were on board? how many survived? how many died?
* What is the highest number of crashes by operator and Type of aircrafts?
___
# Data sourcing
At the time of this project The Dataset was created in Kaggle (2016-09-09), the original version was hosted by Open Data by Socrata at the  [at[{https://opendata.socrata.com/Government/Airplane-Crashes-and-Fatalities-Since-1908/q2te-8cvq,} but unfortunately that is not available anymore. The dataset contains data of airplane accidents involving civil, commercial and military transport worldwide from 1908-09-17 to 2009-06-08.
___

# Data Transformation 
*Changing each column to  an appropriate Data type 
* Expanding necessary column's width to prevent text overflow
* Using the Date column to create new Year, Month and Day columns
___
# Data Modelling 


* We Calculated a new Dax measure to ascertain the Total number of Crashes, by Counting the Total number of rows using the following formula : Total crashes = Count((Airplane_Crashes_and_Fatalities_since_1908[).
* We Calculated a new Dax measure to ascertain the Total number of Fatalities,  by summing the Fatalities column using the formula: Total fatalities = sum(Airplane_Crashes_and_Fatalities_since_1908[Fatalities])
* We Calculated a new Dax measure to ascertain the Total number of Passengers,  by summing the Passengers column using the formula: Total passengers = sum(Airplane_Crashes_and_Fatalities_since_1908[Passengers])
* We Calculated the Fatality rate using the formula: Fatality rate = Divide([Total Fatalities],[Total passengers]×100
___
# Data Visualization/Analysis.
Visualization was done using simple visuals for easy comprehension
___
# Total Crashes
![Total crashes](https://user-images.githubusercontent.com/108596514/178623148-0aa7ea4a-e6a2-411e-b402-658760aac9e5.jpg)
There is a Total of crashes of 5,268 crashes
___
# Total fatali![Total fatalities ](https://user-images.githubusercontent.com/108596514/178623326-675971f1-5788-4014-9810-63dbcb0b65b7.jpg)
There is a Total of 105,479 Fatalities 
ties 
___
#Fatality Rate![fatttality rate](https://user-images.githubusercontent.com/108596514/178623560-a36c0b8d-a31c-4900-be9d-985ee7abbe80.jpg)
There is a Fatality rate of 72.97%
___
# Slucers
Year, Month and D![slicers](https://user-images.githubusercontent.com/108596514/178623732-b7658f6e-7066-4e0e-8159-331b3141818f.jpg)
ay slicers to filter visuals
___
# Top![Top 5 years with most crashes](https://user-images.githubusercontent.com/108596514/178623852-77ba2f33-88ff-47b7-b679-b1022311cc81.jpg)
1972 has the highest number of crashes with a Total 
__-
# Top 5 years![Top 5 years with most fatalities ](https://user-images.githubusercontent.com/108596514/178624032-82faf5da-aa8f-4950-8ada-b59ed17926ef.jpg)
1972 has the highest number of Fatalities with a Total of 2,937 Fatalities 
___

# Top![Top 5 operators with highest crashes ](https://user-images.githubusercontent.com/108596514/178624268-e0133f56-d052-4e02-a051-b56b1166c7bf.jpg)
 5 Operators with highest crashes 
Aeroflot has the highest number of crashes with a Total of 179 crashes 
---
# Top 5 Airplane Types with most Crashes 

![Top 5 Airplane types with most crashes](https://user-images.githubusercontent.com/108596514/178624425-5d3a0d07-96d5-49cb-b416-dc755ec7d0ca.jpg)
Douglas DC-3 has the highest number of  crashes with a Total of 334 crashes.
___
#Conclusion.
*The 1972 has the highest number of Fatalities and highest number of crashes.
*Douglas Airplanes have the highest number of crashes as the planes took first,third,fourth and fifth places in number of Crashes 
*Year with high crashes might not have the highest Fatalities 



