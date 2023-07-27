# 4 - Hospital_wait_time
--------------------
![](photo/wait.jpg)
--------------------
## Introduction

This project is a scenario about the wait time in a hospital
An end-to-end data analytic project with a Microsoft PowerPoint report.

## Problem Statement

### The statement from stakeholder(management)(An Email):
Hello Abdulqader Asiri, our clinics have received many complaints,  
about the general waiting time in the clinic in the last 14 days. 
We want to know why these patients wait so long. 
Is there a specific type of patient who waits for a long time?
Are the types of patients related to their delay? are We too busy? 
Or is this a problem of not having enough staff?
 And if possible, how can we solve this issue?

### My response: (An Email)

#### Okay, but before I start to analyze it ill ask for some more information.
#### What are the clinic's goals?
#### What is our metric of success or failure for this project?
#### What are the trends?
#### And what do you think about this issue?
#### Do you want to know the daily and weekly affected?
#### Do you want a dashboard or just a report? if you want a dashboard, explain how you want it to look like.
#### I usually analyze with Python, but if you want me to use Excel I can do Excel.

### management response: (An Email)
So our goal is (limit long wait times)
Our metric of success or failure for this project is (Wait times)
And our trends are:	
-	Times of the day when waiting times, increase
-	days of the week, when waiting times, increase
we think this issue is because of our staffing or maybe there are a lot of patents.
And yes, we would love to see the daily and weekly affected. 
And we want just a report
Do it with Python or Excel it does, not matter.

In conclusion, The requirements are:
Does the patient type affect the waiting time?
Is there a specific type of patient waiting a long time?
What days of the week are affected?
Are we too busy?
Do we have staffing issues?
How can we fix it?
How much do the patients wait before the doctor can see them?
What type of staff do we need or where do we need them?
------------------------

### TOOLS
- PYTHON
- MICROSOFT EXCEL
- MICROSOFT POWERPOINT


## Data Sourcing

The datasets 
[Kaggle](https://www.kaggle.com/datasets/abdulqaderasiirii/hospital-patient-data) website.
The dataset contains 29998 rows and 11 columns.


### About the data : 
-	Date : The day patient visited
-	Medication Revenue : the revenue of the medication
-	Lab Cost: Lab cost paid by the patient
-	Consultation Revenue: Revenue of the consultation
-	Doctor Type: The type of doctor who treats the patient
-	Financial Class: Patient Financial Class
-	Patient Type: (OUTPATIENT)
-	Entry Time: Entered the (OUTPATIENT) & Hospital
-	Post-Consultation Time: when the doctor tells the patients to enter the clinic room
-	Completion Time: when the patients exit the clinic room or the building.
-	Patient ID: The unique Identity document

## Cleaning & Analysis

1- There are no null values so this is a good start

2 – Replace the spaces between the names of the columns to underline (_), to make the EDA easy.

3 - We don't have the data for patient time waiting, so let's add the timing by sub 'entry time' - 'completion time'.

4 -  We cant sub two dates.time so we need to change 'entry_time' , 'post_consultation_time' , 'completion_time' to_timedelta.

5 -  and more in the code/Report …..

### We could discover the following things in the dataset:
1 - So the Q was: Dose the patient type affect the waiting time?
-	The 'INSURANCE' type of patient is (33.1%) of our patients and they are (9931 patients) and they waiting (44 min ) on average. 
-	The 'PRIVATE' type of patient is (30.4%) of our patients and they are (9121 patients) and they waiting (40 min ) on average. 
-	 The 'CORPORATE' type of patient is (23.1%) of our patients and they are (6915 patients) and they wait (46 min ) on average. 
-	 The 'HMO' type of patient is (12.5%) of our patients and they are (3738 patients) and they waiting (46 min ) on average. 
-	 The 'MEDICARE' type of patient is (1%) of our patients and they are (293 patients) and they waiting (58 min ) on average. 
#### SO No the patient type does not give that big effect on the waiting time, BUT if you 'MEDICARE' type of patient your chance to wait long is higher.
--------------------------
2 - Is there a specific type of patient waiting a long time?
#### Yes there is a specific type of patient waiting a long time, and that type is MEDICARE and they wait (58 min) on average.
------------------

3 – Are we busy?
 #### Yes, we are too busy in the morning period and at 13 hour
In the first heatMap I thoughts it will be less wait time for patients at 7, 13, 17, 21, 22, and 23, But here I found that the rushed time for waiting started at 7 on(Tuesday, Wednesday, Thursday, Saturday) and reach the peak at 9, and decrease after, and start increasing at 13 and decreased after, and increased at 17 Until 20 after that it's decreasing, that means we are short in staff, but im curious about the 7 hour, why the wait time is high?
------------------------
4 – and more in the code/Report …..
---------------------------

## Report : 
These some screnshots of the report:
![]()
----------
![]()
-----------
![]()
----------


# Thank you
