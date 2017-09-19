# EDA_BRFSS
Exploratory Data Analysis on Behavioural Risk Factor Surveillance System (BRFSS) and Short Sleep.

## Whats is BRFSS: 

[**BRFSS**](https://www.cdc.gov/brfss/index.html) ia a large phone anonymous survey conduceted **every year** through a state and federal collaboration and with [**NHANES**](https://www.cdc.gov/nchs/nhanes/index.htm) represents the main US risk factor Surveillance. 

BRFSS is conducted by the CDC (Centers for Diseases Control and Prevention, the U.S federal agency) and it's composed by "Core" questions and "modules". The "core" datasets are public and used by both governmental and independent researches.

The objective of the BRFSS is to collect uniform, state-specific data on preventive health practices and risk behaviors that are linked to chronic diseases, injuries, and preventable infectious diseases in the adult population. Factors assessed by the BRFSS include tobacco use, health care coverage, HIV/AIDS knowledge or prevention, physical activity, and fruit and vegetable consumption. Data are collected from a random sample of adults (one per household) through a telephone survey.

## Sufficient sleep

Adults need 7 or more hours of sleep per night for the best health and wellbeing. Short sleep duration is defined as less than 7 hours of sleep per 24-hour period.

Notably, insufficient sleep has been linked to the development and management of a number of chronic diseases and conditions, including diabetes, cardiovascular disease, obesity,and depression.

- *On average, how many hours of sleep do you get in a 24-hour period?*

(BRFSS variable :SLEPTIM1) 

Starting from 2013 this new question about sleeping has been tested and so we can analyse data at least for three years (2013-2014-2016, no present in the 2015 survey)

I wuold like to investigate how short sleep duration varies by social/demographic factors by (sex, age, race/ethnicity, education level, income, employment status) and if risk factors (BMI, smokers, Physical activity) are more common among adults who sleep <7 hours compared to those who sleep ≥7 hours and display and propose KPIs.

In order to do this I've downloaded the three datasets available (they are very huge, see below) and tried to figure out the structure and the useful data/variables.

Data Pipeline: 

 - [Data Preparation](1_BRFSS_DataPreparation.ipynb)
 
 - [Data Exploration](2_BRFSS_DataExploration.ipynb)


## BRFSS resources: 


* Dataset:
 - [**BRFSS Dataset 2016**](https://www.cdc.gov/brfss/annual_data/2016/files/LLCP2016XPT.zip)
 - [**BRFSS Dateset 2014**](http://www.cdc.gov/brfss/annual_data/2014/files/LLCP2014XPT.ZIP)
 - [**BRFSS Dateset 2013**](http://www.cdc.gov/brfss/annual_data/2013/files/LLCP2013XPT.ZIP)

* General info and mapping and summary statistics about each variable:
 - [**2016 Info and Codebook report**](https://www.cdc.gov/brfss/annual_data/annual_2016.html): 
 - [**2014 Info and Codebook report**](https://www.cdc.gov/brfss/annual_data/annual_2014.html)
 - [**2013 Info and Codebook report**](https://www.cdc.gov/brfss/annual_data/annual_2013.html)


* [**Historical questions database**](https://chronicdata.cdc.gov/Behavioral-Risk-Factors/Behavioral-Risk-Factor-Surveillance-System-BRFSS-H/iuq5-y9ct): questions/variable per year

Note: In the BRSFSS Dataset 2015 the question "On average, how many hours of sleep do you get in a 24-hour period?" was not included.
