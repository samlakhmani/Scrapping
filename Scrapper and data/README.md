# Selenium Tutorial: Scraping Glassdoor.co.in

The motivation for the scrapper is to be able to develop a Data Science project from the data that is aquired. Glassdoor ,a href='https://www.glassdoor.com/about/terms.htm'>Terms of Use</a> states that they do not alow scraping and your account can be banned for using a scraper.

*This project is purely for educational purposes, and if Glassdoor aproaches me to remove this repository, I will oblige*

The Data Science project is a analysis project aim to replicate the daily functioning of a 'Data Anlytist' job profile. 
Further elaboration on the project details will be available in the respective <a href=https://github.com/samlakhmani/DS_salary>directory/repository</a>.(click to redirect you to the repository)

Using this scraper we will be extracting Company details, the job details and the salary details for further analysis


# Literary Review

Exsisting scrappers were searched to get basic architecture and functioning 
Found no scraper with handling updated glassdoor notification 
Job opening in india do not display an estimated/expected salary  

# Methodology

We used selenium library to go throught the JS web app portion of the job listing to select one job offer at a time

Job
 |_ Company Details
 |_ About Job
 |_ Salary
 
After building a basic scraper tool with the help from the resources, modifications were made to help handle the various pop-ups that would disturb the process of the scraper, such as jobalert and sign-up forms
The company details and job profile details were stored in a data frame
Since no estimated salary was given we extracted top 5 related salaries and made a dataframe for it for further analysis. For every job listing in the Job dataframe there are 5 rows in the salary dataframe 


## This results in two DataFrame 
1. The job list with details about the company in 1st DataFrame
1. Salary Details in 2nd DataFrame

## Pre-requisites
1. Understanding of python
1. python 3
1. Anaconda Environment 
1. Website Architechture basics
1. Knowledge of XPath. (Shared a very good resource below)
1. selenium library  

## Resources :
1. https://github.com/MatthewChatham/glassdoor-review-scraper
1. https://devhints.io/xpath
1. https://github.com/MatthewChatham/glassdoor-review-scraper 
1. https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905
1. https://github.com/arapfaik/scraping-glassdoor-selenium
