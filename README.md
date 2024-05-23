You are employed as a data scientist at Trivisio. At the moment we are trying to sell the new Colibri Wireless unit, which is an inertial measurement unit (IMU). It is made up of 3 sensors to measure acceleration, angular rate and magnetic field, and separates sensor to measure temperature and orientation. 
We want our product to be superior to our main competitors: Wireless InertiaCube3 by InterSense, MTw Awinda by Xsens, T40s by Vicon, and OptoTrak 3020 by Optotrak Certus. 

We have collected data from 9 subjects who wore 3 IMUs and a heart-rate monitor. They each conducted 12 different physical activities (e.g., walking, cycling, playing football), with some conducting an additional 6 extra activities. 
The data is stored in individual .dat files per each subject. Each row in the dataset represents a single reading on the companion unit (a dongle that plugs into a computer to act as a receiver for the data), containing 54 attributes:

timestamp
activityID
heart-rate bpm (beats per minute)
(4-20) IMU readings from the unit attached to the wrist on the dominant arm
(21-37) IMU readings from the unit attached to the chest
(38-54) IMU readings from the unit attached to the ankle on the dominant leg
The full dataset can be downloaded from here: Dataset.zip Download Dataset.zip (you will need to unzip the file to get access to the following files).

DataCollectionProtocol tells you about how the data was collected for each participant
DescriptionOfActivities gives you an outline of each of the activities
PerformanceActivitiesSummary tells you how long each subject spent doing each activity
subjectInformation gives you relevant information about the characteristics of each subject
TrivisioColibriwirelessBrochure is the advert we released about the Colibri Wireless unit
Report2_data_info gives you an overview of the above documents and information
Protocol/ is the directory that contains all the dat files for the subjects conducting the 12 recommended activities
Optional/ is the directory that contains all the dat files for the subjects who conducted the 6 optional activities
 

I want you to come up with a predictive hypothesis using the data available that you can use a mathematical model to answer. This hypothesis needs to be actionable, but it is up to you decide on how it is actionable (that is, you can come develop your own impact and interpretation of the model). 
Actionable here means that you recommend some policy changes, additional software or addition/reduction of hardware. So it is up to you to choose explanatory variables and a response variable, but the model needs to at least include the activityID (it could be an explanatory variance or a response variable). 
You also need to justify why the other features are not helpful in your model - this does not need to be using feature selection (though you should be doing this at some point in the modelling process), it can be through interpretation. 

For example, my predictive hypothesis could be: what activities can I predict using heart rate bpm, age, height, weight, resting HR, max HR, average acceleration, variance of the acceleration, average angular rate and variance of the angular rate? My actionable insight could be: given the mathematical model, I have developed software that predicts the type of activity and automatically writes it down in the activity tracker. 
I decided not to use dominant hand and sex because there is not enough data for each of the classes, I found temperature is strongly correlated to heart rate bpm (I have not checked this, this is a fictional example), and magnetic field and orientation only really provide information about location. 

This should be treated as a real report - you must imagine that you have this job and that I am your boss at Trivisio. Despite the presence of the code cells (a necessity of the module assessment) all other aspects should be like a report you would submit to your boss. Explain your reasoning, back up your claims with evidence. 
Provide valid, supported conclusions in natural language and give specific recommendations for actions. Reports full of typos, irrelevant or unreadable data plots, and without conclusions would get you fired; here they will receive failing grades.

 

You are employed as a data scientist at Trivisio. At the moment we are trying to sell the new Colibri Wireless unit, which is an inertial measurement unit (IMU). It is made up of 3 sensors to measure acceleration, angular rate and magnetic field, and separates sensor to measure temperature and orientation. We want our product to be superior to our main competitors: Wireless InertiaCube3 by InterSense, MTw Awinda by Xsens, T40s by Vicon, and OptoTrak 3020 by Optotrak Certus. 

 

We have collected data from 9 subjects who wore 3 IMUs and a heart-rate monitor. They each conducted 12 different physical activities (e.g., walking, cycling, playing football), with some conducting an additional 6 extra activities. The data is stored in individual .dat files per each subject. Each row in the dataset represents a single reading on the companion unit (a dongle that plugs into a computer to act as a receiver for the data), containing 54 attributes:

timestamp
activityID
heart-rate bpm (beats per minute)
(4-20) IMU readings from the unit attached to the wrist on the dominant arm
(21-37) IMU readings from the unit attached to the chest
(38-54) IMU readings from the unit attached to the ankle on the dominant leg
The full dataset can be downloaded from here: Dataset.zip Download Dataset.zip (you will need to unzip the file to get access to the following files).

DataCollectionProtocol tells you about how the data was collected for each participant
DescriptionOfActivities gives you an outline of each of the activities
PerformanceActivitiesSummary tells you how long each subject spent doing each activity
subjectInformation gives you relevant information about the characteristics of each subject
TrivisioColibriwirelessBrochure is the advert we released about the Colibri Wireless unit
Report2_data_info gives you an overview of the above documents and information
Protocol/ is the directory that contains all the dat files for the subjects conducting the 12 recommended activities
Optional/ is the directory that contains all the dat files for the subjects who conducted the 6 optional activities
 

I want you to come up with a predictive hypothesis using the data available that you can use a mathematical model to answer. This hypothesis needs to be actionable, but it is up to you decide on how it is actionable (that is, you can come develop your own impact and interpretation of the model). Actionable here means that you recommend some policy changes, additional software or addition/reduction of hardware. So it is up to you to choose explanatory variables and a response variable, but the model needs to at least include the activityID (it could be an explanatory variance or a response variable). You also need to justify why the other features are not helpful in your model - this does not need to be using feature selection (though you should be doing this at some point in the modelling process), it can be through interpretation. 

For example, my predictive hypothesis could be: what activities can I predict using heart rate bpm, age, height, weight, resting HR, max HR, average acceleration, variance of the acceleration, average angular rate and variance of the angular rate? My actionable insight could be: given the mathematical model, I have developed software that predicts the type of activity and automatically writes it down in the activity tracker. I decided not to use dominant hand and sex because there is not enough data for each of the classes, I found temperature is strongly correlated to heart rate bpm (I have not checked this, this is a fictional example), and magnetic field and orientation only really provide information about location. 

This should be treated as a real report - you must imagine that you have this job and that I am your boss at Trivisio. Despite the presence of the code cells (a necessity of the module assessment) all other aspects should be like a report you would submit to your boss. Explain your reasoning, back up your claims with evidence. Provide valid, supported conclusions in natural language and give specific recommendations for actions. Reports full of typos, irrelevant or unreadable data plots, and without conclusions would get you fired; here they will receive failing grades.

 

Your report should contain details relating to the following three issues:

Exploratory data analysis you have carried out with the Physical Activity Monitoring data.
Develop and test at least one model which uses multiple attributes to make predictions.
Actionable recommendations based on the analyses you have conducted. should contain details relating to the following three issues:

Exploratory data analysis you have carried out with the Physical Activity Monitoring data.
Develop and test at least one model which uses multiple attributes to make predictions.
Actionable recommendations based on the analyses you have conducted.
