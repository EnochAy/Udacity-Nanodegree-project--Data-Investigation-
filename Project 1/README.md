# Udacity-Nanodegree-project--Data-Investigation

# Project: Investigate a Data Set - (No Show for Medical Appointment)


## Table of Contents
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#wrangling">Data Wrangling</a></li>
<li><a href="#eda">Exploratory Data Analysis</a></li>
<li><a href="#conclusions">Conclusions</a></li>
</ul>
<a id='intro'></a>
## Introduction

> I have selected the No-show appointments (original source on
Kaggle) dataset. This dataset collects information from 100k medical appointments in
Brazil and is focused on the question of whether or not patients show up for their appointment. 
A number of characteristics about the patient are included in each row.
● ‘ScheduledDay’ tells us on what day the patient set up their appointment.
● ‘Neighborhood’ indicates the location of the hospital.
● ‘Scholarship’ indicates whether or not the patient is enrolled in Brasilian welfare
program Bolsa Família.
● Be careful about the encoding of the last column: it says ‘No’ if the patient showed up to their
appointment, and ‘Yes’ if they did not show up.


Name (Value(s))          Description
PatienID (number)	    Identification of a patient
AppointmentID (number)   Identification of each appointment
Gender (F or M)	        It says 'F' if female or 'M' if man
ScheduledDay (date)	    Tells us on what day the patient set up their appointment
AppointmentDay (date)	The day of the actuall appointment, when they have to visit the doctor
Age	(number)	            How old is the patient
Neighbourhood (string)	Indicates the location of the hospital
Scholarship (0 or 1)	    Indicates whether or not the patient is enrolled in Brasilian welfare program Bolsa Família
Hipertension (0 or 1)	Indicates if the patient has hipertension
Diabetes (0 or 1)	    Indicates if the patient has diabetes
Alcoholism (0 or 1)	    Indicates if the patient is an alcoholic
Handcap (0 or 1)	        Indicates if the patient is handicaped
SMS_receive (0 or 1)	    1 or more messages sent to the patient
No-show	(Yes or No)	    It says ‘No’ if the patient showed up to their appointment, and ‘Yes’ if they did not show up


## Metadata
110527 rows/records (Medical Appointments) and 14 columns/variables associated with each records.

PatientId: Identification of a patient.

AppointmentID: Identification of each appointment.

Gender: Male (M) or Female (F).

ScheduledDay: The day someone called or registered the appointment, this is before appointment of course.

AppointmentDay: The day of the actuall appointment, when they have to visit the doctor.

Age: How old is the patient.

Neighbourhood: Where the appointment takes place.

Scholarship: True (1) of False (0).

Hypertension: True (1) or False (0).

Diabetes: True (1) or False (0).

Alcoholism: True (1) or False (0).

Handicap: The handcap refers to the number of disabilites a person has. 
For example, if the person is blind and can't walk the total is 2.

SMS_received: 1 or more messages sent to the patient.

No-show: Yes (If the patient did not show up for the appointment. No, if the patient shows up for the apponitment)




The most important variable in this research is "No-show".
This variable describes if the patient shows up or not for appointment.

# Dependent Variable: No-show

# Independent Variables: age, gender, scholarship, and waiting_period.

# Research Questions
1. What factors are important for us to know in order to predict if a patient will 
show up for their scheduled appointment?
2. Is there any correlation between age and those who shows up for appointments?
3. Is there any correlation between gender showing up for appointments?
4. Does receiving scholarship have a significant impact on showing up for appointments?
5. Does receiving messages have a significant impact on showing up for appointments?



# Findings
Q1: What factors are important for us to know in order to predict if a patient will 
show up for their scheduled appointment?

Answer: It was discovered that the following factors are important for us to know in order to predict if a patient will show up for their scheduled appointment:
1. Age (Older/Younger)
2. Scholarship (Yes/No)
3. handicapped (Yes/No)
4. Recieved Message (Yes/No)


Q2: Is there any correlation between age and those who shows up for appointments?

Answer: It was found that children and elderly ones show up more for their medical appointments than the youths.

Q3: Is there any correlation between gender showing up for appointments?

Answer: The percentages of no show patients based on gender were pretty close. So, we can say that the gender can't be considered as a factor to predict if a patient will show up for their scheduled appointment.
Consequently, we can not conclude that gender affects showing up for appointments or not.


Q3: Can the age be considered as a factor to predict if a patient will show up for their scheduled appointment?
Yes, the younger the patient is the more likely he/she is going to miss the appointment. Except the group (0-18) 
since they probably are accompanied by an adult. 

Q4: Does receiving scholarship have a significant impact on showing up for appointments?

Answer: From the analysis and  visualizatin done, it can be concluded that patients without scholarship shows 
up more for their appointments than those with scholarship.
Hence, it patient with a scholarship is more likely to not show up for the appointment.

Q5: Does receiving messages have a significant impact on showing up for appointments?

Answer: From the analysis and  visualizatin done, it can be concluded that patients who did not receive messages show up more for their appointments than those who did.



# Limitations of my Data Analysis and Exploration
The following are the limitations experienced during the cause of this project:
1. The dataset covered only one country. 
It would have been better if we have dataset from more that one country.

2. A more recent data would be much better.
2016 is about 6 years ago and a lot has changed since then.

3. The dataset covers a short period of only 40 days.
Longer period could lead to a better results.


# References
1. Stack Overflow
2. numpy documentation
3. pandas documentation
4. seaborn documentation
5. https://learn.udacity.com/nanodegrees/nd002-alg-t2/parts/cd0000/lessons/ls0526/concepts/f41d3e13-9bbc-45a7-8e7e-14f9e5ba1607
