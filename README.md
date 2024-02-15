# Understanding-the-psychological-effects-of-COVID-19



## Introduction

## Executive Summary

## Data Sourcing
Our data was downloaded as a .csv file from Kaggle.  It’s a data collected in 2020 to help understand people’s opinion of the lockdown. It was collected using Google forms.

For the data source link
[Click here](https://www.kaggle.com/datasets/hemanthhari/psycological-effects-of-covid)

Metadata (this contains the definition of each column content) as posted by Hemanth Harikrishnan on Kaggle.
-	**age**: Age group of the person
-	**gender**: Gender of the person
-	**occupation**: Occupation/sector where the person works
-	**line_of_work**: The line of work performed by the person
-	**time_bp**: The time spent on work before pandemic
-	**time_dp**: The time spent on work during pandemic
-	**travel_time**: The travel time spent
-	**easeof_online**: Rating of work going online
-	**home_env**: Liking of home environment
-	**prod_inc**: Rating Productivity Increase
-	**sleep_bal**: The rating of sleep cycle
-	**new_skill**: Whether any new skill was learnt
-	**fam_connect**: Rating how well the person connected with his family
-	**relaxed**: Rating of how relaxed the person is feeling
-	**self_time**: Rating how much self-time was procured
-	**like_hw**: Liking of working from Home
-	**dislike_hw**: Disliking Working from Home
-	**prefer**: Preference of the person to work from home/office
-	**certaindays_hw**: Liking whether certain days of working from home is needed


## Data Cleaning
Most of the data cleaning was done on the Power query extension of Microsoft Excel.
We started off by renaming some columns. This can be done on excel or query. The old and new names are given below
- age: Age Group
- gender: Gender
- occupation: Occupation
- time_bp: Time Before Pandemic
- time_dp: Time During Pandemic
- easeof_online: Ease of Online Work
- home_env : Home environment
- prod_inc: Productivity Increase
- sleep_bal: Sleep Balance
- new_skill: New Skill
- fam_connect : Family Connection
- self_time: Self Time

In the ‘Age’ column the values ‘Dec-18’ which was a formatting error was replaced with ‘12-18’. This was done after looking carefully at the categories in that column and also Dec is 12 in numbers.

The column ‘travel+work’ which contained completely blank cells,’time_bp’ which was a column duplicate, and two other completely blank columns were deleted.

The values of the columns ‘Ease of Online Work’, ‘Home Environment’ were changed to labels. The value-label pair is listed in the following dictionary

{1: “Strongly Disagree”, 2: “Disagree”, 3: “Neutral”, 4: “Agree”, 5: “Strongly Agree”}

The values of the columns ‘Productivity Increase’, ‘Sleep Balance’, ‘New Skill’, ‘Family Connection’, ‘relaxed’, ‘Self Time’ were changed to labels. The value-label pair is listed in the following dictionary

{-1: “Strong Decrease”, -0.5: “Decrease”, 0: “Neutral”, 0.5: “Increase”, 1: “Strong Increase”
This decision was taken, after going through the metadata and understanding the purpose of the question, which revealed an inherent order (ordinal data) and also for data analysis and visualizations, labels provide more clarity than numbers for ordinal data.

## Data Analysis/Exploration
TABLES
We start first by getting the distribution of our survey participants by their age groups, occupations, and gender. This is to help us understand the perspective their responses are coming from. We also see these values in percentages for better understanding.
We move next to exploring their responses to the questions looking at them from different angles; occupation, age group, gender.
DASHBOARD
Our dashboard shows a summary view of our tables. With slicers at the left of the page, to help you filter the results according to questions you require answers to.

## Results 
GENERAL
Generally, there was a 7.4% increase in the average work hours of the respondents.
Over half of the participants didn’t find transitioning into remote work easy. 
A great percentage of the respondents were indifferent about their home environment, another large percentage disagree to liking their home environment, and a lesser percentage like their home environment.
A large percentage of respondents were able to connect more to their families, with a lesser percentage seeing a decrease in connecting to their family.
There was an almost equal balance with those agreeing that they saw an increase in productivity, and those that saw a decrease in productivity, and those that were neutral.
A little over half the participants learnt a new skill during the pandemic, while the others replied negative.
Over a quarter of respondents answered neutral to having more self-time and relaxation.
About 45% of the respondents saw a decrease in their sleep balance, and about 32% saw an increase in their sleep balance.
You can refer to the charts and tables for more information.
GENDER
Generally, males found the transition of working in the pandemic easier compared to females. This conclusion was gotten after comparing the percentages of responses by gender.
Males found it easier to work online compared to females, as only 45% of them replied in the negative, with 61% for the females.
More females than males disliked their home environment. An almost equal percentage of both genders agreed to connecting more to their families.
An almost equal percentage of both genders saw a decrease in their sleep balance, and also time they had for themselves.
Almost half the females replied in the negative to learning a new skill and positive to having an increase in productivity, while it was over a quarter for the males in both cases.
More percentage of females than males relaxed more during the pandemic.

## Conclusions
There was an increase in productivity which surprised me, because I expected a decrease. This tells much about our abilities to adapt to any situation and make the most of it. 
Males adapted the easiest to the pandemic, as a greater percentage of them answered in positive to improvement questions compared to females. We have a smaller amount of those who didn’t disclose their gender, limiting our ability to make conclusions for them.
