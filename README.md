
# Project: I+D Cancer investigation in California

__Made by__:
* Darwin Diaz
* Ignacio Irace

## 1. Objectives

* __Main Objective__: Cancer investigation focused on medical advances for early identification in California.

    * __Secundary Objective 1__: Analize total cases in California for insights
    * __Secundary Objective 2__: Find which types of cancer can reduce mortaility rate with early detections.
    * __Secundary Objective 3__: Simulate a timeline between 2013 and 2018 with the count of cases per year and per type.



## 2. Question

__Question__: does cancer cases can be reduce with early detection?

__Secundary Questions__:

* Everyone of you have heard about cancer?
* How many of you know someone that has any cancer?
* Do you know anyone that has pass away because of cancer?
* Do feel this last question in sometime will be __no__ ?


## 3. How the market investigation was structured

Kindly consider this investigation was not made for business purposes, the main purpose of this investigation is looking for areas where the investigation needs to go further to save lives.

The main country for this investigation is the United States a country with more than 326 millions of population, we look at statistics from each state looking for the one with more cancer cases, Colifonia is the state with more cancer cases registered between 2015 and 2019, the count rises to 871 thousand, almost 1 million. California is the right target for the big number of cancer detected.

The dataset was taken from data world, there are more than 11k registers of cancer surgeries made in California between 2013 and 2017, to make a deeper investigation we look for complementary data like per-capita income, population for every county (the population used in this investigation was 2018 and we used as reference), new detection, mean detection and late detection. The Center for Desease Control and Prevention (CDC) was also a useful site for our investigation, from here we get data like prevention, death, new cases, etc... Wikipedia was also helpful to extract general data like population and per-capita income.

 


### 3.1. Libraries used

The data was threated using python to apply cleanning and web scrapping models until the data was prepared, further the data is going to be presented into Power BI.

* __Pandas__ : Used for data manipulation and data wrangling.
* __Requests & Beautifulsoup__ : Used for web scrapping.
* __Matplotlyb.pyplot__: For sampling visualizations.
* __Pandas Profiling__ : For sampling visualizations.
* __Plotly__: Interactive maps.



### 3.2. Data cleanning process

First, from the 11k lines from California surgeries basic cleanning and ordering data techniques were applied like changing the names, strips and unifying the data as much as posible, for example; # of Cases (ICD 9) and # of Cases (ICD 10) were concatenated into one column because the difference between both is the year were they were applied.

The NA values for county were filled out with "Sacramento" because the Statewide Hospital is in this hospital has the most NA values. Investigating through google we also look for the averge cost of a surgery depending on the cancer type, then applying two different web scrapping scripts to get data from wikipedia, after the web scrapping the county names were adapted to the one from the first dataset.



## 3.3. Power BI

Power BI is one of the most used tools for visualizations. The dashboard is more focused into the amount of cancer cases and surgeries, basically looking for the hospitals that makes more surgeries per each type of cancer, also some sheets are about demografic data like the counties with mores cancer surgeries and comparissons from costs vs per-capita income per county.

One important data considerated in this dashboard is the detection, a sooner detection depending on the cancer can lower the death probbility which is the main purpose of the software. Area maps were applied to identify the survival probabilities and detection probabilities for then comparing this probabilities per detection (sooner, meand and late) to find the relationship between detection and survival per cancer type.



## 4. Insights and answer to the main question

### 4.1 Answer
Basically the question was answer when we structured the market investigation, but why? the answer to this question is the amount of surgeries made in California compared to the rest of states in the US. The amount of surgeries will mark a clear tendency and accurate data.

### 4.2 Insights
* Breats and Prostate cancer are the most advanced in detection.
* Most late cancer detections have a lower survivial rate.
* New cases and mortality rate have a positive correlation.










