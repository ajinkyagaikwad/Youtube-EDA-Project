# Youtube-EDA-Project
Analysis of my own YouTube watch history

**Introduction**

This repository contains code and documentation for the Exploratory Data Analysis (EDA) project using YouTube dataset sourced from (https://takeout.google.com/)

**Objective**

Clean and enhance the dataset, perform EDA which provides information about watching patterns in the YouTube activity.

**Dataset overview**

'MyActivity.json' contains 100k+ records of YouTube activity. Each record represents a unique information (identified by titleurl) and includes various attributes such as Title, subtitles, time and more

**How to source data**

Visit https://takeout.google.com/ -> My Activity -> Deselect all -> Select YouTube -> from file format select json -> export via email

**Issues found in the data**

Missing values- there were some records without channel name in the 'subtitles' column. As this would prove a hindrance while creating a new column 'Channel Name', I deleted such rows

Removed videos- there were 300+ entries with videos removed from the YouTube. I filtered them out for analysis.

Record of ads - many rows were the records of ads watched on YouTube. Based on the 'details' column, I filtered them out as well.

Datatype of 'date' column - it was string earlier; to work with the time, I changed it to datetime

**Tools used**

For the EDA project, following tools were used

Python for data cleaning tasks

Pandas was instrumental in data manipulation, cleaning and handling missing values

NumPy was utilized for mathematical operations and array handling during the cleaning process

Google Colab provides an interactive Jupyter notebook environment for code development, exploration and documentation

Seaborn and matplotlib for plotting the data

**Data Cleaning Process**

The data cleaning process involved the following steps:

Data Understanding - The dataset was thoroughly examined to understand the structure, columns and their meanings. Being familiar with the YouTube helped me get a grasp of the data quickly.

Data Exploration - Exploratory Data Analysis was performed to gain insights into the data, identify patterns and uncover anomalies.


**EDA**

EDA process involved following steps:

Getting the insights into the data using pandas, numpy framework

Plotting the analysis of columns to reveal their corelation, trend, comparisons

**Documentation**

For detailed information about the EDA process, please refer to the Jupyter notebook provided in the repository
