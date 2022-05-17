# Google-Data-Analytics-Professional-Certificate-bellabeat_case_study

![índice](https://user-images.githubusercontent.com/98779367/168304972-6ef68f87-f6e4-47ba-a97c-9716af2a0530.png)


## Scenario
In this case, I'm a junior data analyst working on the marketing analyst team at <b>Bellabeat, a high-tech manufacturer of women's health-focused products</b>.
Bellabeat is a successful small, but high-tech, company that makes smart health-focused products. With their products they intend to become a more larger player in the
global market for smart devices.
Collecting data on activity, sleep, stress, and reproductive health has allowed Bellabeat to empower women with
knowledge about their own health and habits. Since it was founded in 2013, Bellabeat has grown rapidly and quickly
positioned itself as a tech-driven wellness company for women.
By 2016, Bellabeat had opened offices around the world and launched multiple products. Bellabeat products became available
through a growing number of online retailers in addition to their own e-commerce channel on their website. The company
has invested in traditional advertising media, such as radio, out-of-home billboards, print, and television, but focuses on digital
marketing extensively. Bellabeat invests year-round in Google Search, maintaining active Facebook and Instagram pages, and
consistently engages consumers on Twitter. Additionally, Bellabeat runs video ads on Youtube and display ads on the Google
Display Network to support campaigns around key marketing dates.

To answer the key business questions, I will follow the steps of the
data analysis process proposed by Google: <b>ask, prepare, process, analyze, share and act.</b>

## Ask
This first step focuses on having a clear understanding of the business task and key stakeholders.
We ask ourselves questions?. What we are trying to understand?. How we can use available information to make informed business decisions?.

<b>Business task and key stakeholders:</b>
* Urška Sršen: Bellabeat’s cofounder and Chief Creative Officer.
* Sando Mur: Mathematician and Bellabeat’s cofounder; key member of the Bellabeat executive team.
* Bellabeat marketing analytics team: A team of data analysts responsible for collecting, analyzing, and
reporting data that helps guide Bellabeat’s marketing strategy.

Sršen asks you to analyze smart device usage data in order to gain insight into how consumers use non-Bellabeat smart
devices. To do that she encourages you to use public data that explores smart device users’ daily habits and then apply those findings in one bellabeat product in particular.

## Prepare
The Prepare step is where we analyze the data we're working with? How is it organized? Where does it come from? Is it reliable?, etc.
The Kaggle dataset, [FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit), is found under de license (CC0: Public Domain, dataset made available through [Mobius](https://www.kaggle.com/arashnic). 
<br>This dataset consists of 18 csv files and is generated by respondents to a distributed survey via Amazon Mechanical Turk between 03/12/2016 and 05/12/2016. Thirty-three eligible Fitbit users consented to the submission of personal tracker data, including minute-level output for physical activity, heart rate, and sleep monitoring.

The ideal data source should be <b>ROCCC</b>, which stands for Reliable, Original, Comprehensive, Current, and Cited. In this particular case:
* It is <b>not Reliable</b>, because the sample size is small and it is not representative of the population.
* It is <b>not Original</b> because it is provided by a third party. In this case Amazon Mechanical Turk.
* It <b>is Comprehensive</b> because it includes the right information and parameters to understand smart watch users. 
* It <b>is not Current</b>. The survey ranges from 03/12/2016 to 05/12/2016, which makes it out of date.
* It's <b>not well Cited</b>. Missing key information about data providers, how they do the survey, etc.

Sršen have told us that this data set might have some limitations, and encourages us to consider adding another data to help
address those limitations as we begin to work more with this data.

## Process
This step focuses on formatting, cleaning, and preparing the data for proper analysis. We try to reduce data redundancy to minimize future analytic errors and ensure integrity.
* The tools chosen for this case are "Microsoft SQL Server", "Excel" and "Tableau".
* Data has been sorted, filtered, and formated for analysis. I have focus on remove, duplicates and unnecesary information, check data types, remove outliers, find and fix structurals errors, handle missing data, and data validation.

<b>1.</b> First of all, we create a new database and import all the files into SQL Server.
<b>2.</b> We do a quick SELECT statement to inspect tables.

`
SELECT *
FROM dailyActivity_merged
`
