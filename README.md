# Freemind-Insurance-Analysis
This project involves analyzing an insurance dataset to understand the factors influencing insurance charges considering individuals age, sex, BMI, number of children, smoking status and region. The picture below is gotten from [freepiks website](https://www.freepik.com/free-photo/life-health-insurance-policy-concept-idea_1211580.htm#query=insurance%20policy&position=1&from_view=search&track=ais&uuid=f7c443cf-b85d-493d-ae15-5ae21b30f038)


![](life-health-insurance-policy-concept-idea.jpg)

## Introduction
This report presents a comprehensive analysis of an insurance dataset, aiming to understand the factors influencing insurance charges. This dashboard is user-friendly and interactive. It makes use of slicer to select results by region. The dataset consists of information on individuals, including their age, sex, BMI, number of children, smoking status, region, and insurance charges

## Problem Statement
The goal of this analysis is to address these questions:
* What is the distribution of insured individuals based on age, and how does it impact insurance charges?
* What is the average BMI of insured individuals, and is there a relationship between BMI and insurance charges?
* How does the number of children influence insurance charges?
* What proportion of the insured population are smokers, and how does smoking status correlate with insurance charges?
* Are there any specific regions where insurance charges are consistently higher or lower?
* What are the primary factors contributing to higher insurance charges in the dataset?
* How do these customer segments based on age, BMI differ in terms of insurance charges and other characteristics?
* Highlight any trends, outliers, or patterns that you observe.

## Skills and Concepts Demonstrated
The following are skills and concepts demonstrated when working on this project
* Data Exploration
* Filtering and Slicing
* Correlation and Analysis
* Customer and BMI Segmentation
* 
## Data Source



## Data Transformation
Data preparation and cleaning was done on Power Query Editor and the following are the steps taken to prepare the data for further analysis:
•	Changed all fields to the appropriate data types

•	Removed duplicates (1338 was the original number of rows but after this step, we are left with 1337  rows)

•	Added new column using ‘conditional column’ to create age distribution between age 18 to 64 

•	Added another column to create a standard BMI (Body Mass Index) distribution from 15.96 to 53.13

•	The ‘index column - from 1’ was created to give all individuals it unique ID 

•	The newly added columns were renamed and reordered to their appropriate place

* Data Cleaning
![](Cleaning.PNG)


## Data Analysis
To detect outliers, Z-score and scatter plots were used. In the case of Z score, Z-Score was calculated on numeric column and outliers were identified. The following are report of outliers found in numeric columns;
•	No outliers detected on age column 
•	4 records were identified as outliers on BMI column.
•	No outliers detected on children column 
•	No outliers detected on charges column.

Treatment of Outliers
BMI Outliers: Outliers in the BMI variable are 4. These 4 outliers in BMI column are replaced with the mean value of the column using DAX

* DAX
![](DAXInsurance.PNG)

* Z Score
![](ZScore.PNG)

Insights from scatter plot
•	With scatter plot, outliers were identified in charges variable and it shows 8 outliers. These outliers were transformed and replaced with IQ3
•	The results shows that there’s a positive relationship between age and insurance charges. 
•	It indicate that age has a significant impact on insurance charges meaning the older you get the higher the charges, while the number of children has a minimal effect.
•	It shows that age and BMI values are great determinant of charges

## Data Visualization
This dashboard is user-friendly and interactive. It makes use of slicer to show results by region. The dashboard shows all information of insured individuals and how it influence the insurance charges.

![](Dashboard.PNG)
