# Phase 1 Project Description - Qi, Olu and Scotty

## Project Overview

For this project, we utilized data cleaning, imputation, analysis, and visualization to generate insights for a business stakeholder.

### Business Problem

This company is expanding into new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for private enterprises. but do not know anything about the potential risks of aircraft. The company will cater to individual clients, corporations, or groups who require exclusive and personalized air transportation, for business, convenience, luxury, or efficiency reasons.


## Business Understanding

The company is interested in purchasing and operating jets for business, executive, corporate and private clients.

Our company had several key questions regarding their new business endeavor:

* What are the most reliable types of engines that we can purchase for our aircraft?
* Which aircraft would have the most optimal cost of maintenance and operation?
* Which aircraft have the best outcomes in case of accidents in terms of injuries and aircraft damage?
* What is the financially optimal number of engines per aircraft?
* Which aircraft has features that would best help us serve our clients?



## Data Understanding and Analysis

### Source of Data

In the `data` folder is a [dataset](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses) from the National Transportation Safety Board that includes aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters.

### Description of Data
The dataset consists of 90,000+ rows; each row represents an accident. 
The dataset has 31 columns including: 

* Event.Id	
* Investigation.Type	
* Accident.Number	
* Event.Date	
* Location	
* Country	
* Latitude	
* Longitude	
* Airport.Code	
* Airport.Name	
* Injury.Severity	
* Aircraft.damage	
* Aircraft.Category	
* Registration.Number	
* Make	
* Model	
* Amateur.Built	
* Number.of.Engines	
* Engine.Type	
* FAR.Description	
* Schedule	
* Purpose.of.flight	
* Air.carrier	
* Total.Fatal.Injuries	
* Total.Serious.Injuries	
* Total.Minor.Injuries	
* Total.Uninjured	Weather.Condition	
* Broad.phase.of.flight	
* Report.Status	
* Publication.Date

The datatypes of these columns are strings and floats.

#### Interactive Dashboard
By analyzing the dataset, we were able to create a dashboard with several interesting insights.

[Link to interactive dashboard of visualizations from the data](https://public.tableau.com/app/profile/qi.cai/viz/AvationBusinessDashboard/Dashboard1?publish=yes)

See below dashboard:

![tableau dashboard for aviation accidents](https://i.imgur.com/iZtcwnZ.png)


## Conclusion
After thorough analysis of the dataset, we have several conclusions for the company that wants to purchase and operate airplanes for private enterprises:

* The 3 best aircraft for the company would be the Bombardier CL-600, Rockwell NA-265-80 and Raytheon 400A jets.
![Bombardier CL-600, Rockwell NA-265-80 and Raytheon 400A jets.](https://i.imgur.com/iTLGP3A.png)

* Aircraft with turbo engines are much more safer than aircraft with reciprocating engines. The data shows that there is a much lower risk of crashes with aircraft-powered turbo fan engines.
* There has been a overall downward trend in the number of aircraft crashes per year starting from 1985.