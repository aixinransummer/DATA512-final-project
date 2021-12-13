# DATA512-final-project

This repository contains all the relevant files for the final project in Data 512. The write-ups for Assignment 4 to Assignment 7 are included with a jupyter notebook documenting all the code that has been used throughout my study on the correlation between unemployment rate and infection rate in Denver, Colorado. 

## Data Used
There are three data sources used in this project. 

The first one is the [COVID-19](https://www.kaggle.com/antgoldbloom/covid19-data-from-john-hopkins-university?select=RAW_us_confirmed_cases.csv) data from John Hopkins University, which documents cumulative confirmed cases per county in the U.S since January 22nd, 2020. By the proejct was created, data until October 15th, 2021 was used for the study. The original dataset contains attritbues listed below

| Attributes | Description |
| --- | --- |
| Province_State | Name of the state|
| Admin2| Name of the county |
| UID | A unique identifier for each county|
| iso2| Two-letter country codes defined in ISO 3166-1|
| iso3 | Three-letter country codes defined in ISO 3166-1|
| code3| Standard country or region code for statistical use |
| FIPS | Federal Information Processing Standards code for the county |
| Country_Region| Name of the country for the region |
| Lat | Latitude of the region |
| Long| Longtitude of the region |
| Combined_Key| Indicate county, state, country |
| Dates| Cumulative number of confirmed cases for specific date |

After selecting the data about Denver, CO from this dataset, only the attributes of dates and cumulative cases were used for analysis. 

The second dataset is the [mask mandates](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i) data from CDC.The attributes and their description is listed below

| Attributes | Description |
| --- | --- |
| State_Tribe | Abbreviation of the state or the tribe|
| County_Name| Name of the county |
| FIPS_State | Federal Information Processing Standards for the state|
| FIPS_County| Federal Information Processing Standards for the county|
| date | Dates in the format of mm/dd/yy|
| order_code| Indicate if there is a order for mask policy|
| Face_Masks_Required_in_Public | A requirement for individuals operating in a personal capacity to wear masks 1) anywhere outside their homes or 2) both in retail businesses and in restaurants/food establishments. |
| Source_of_Action| Source where order was found |
| URL| URL of order language used to complete dataset|
| Citation|Citation for the order|

After selecting the data about Denver, CO from this dataset, only the attributes of dates and Face_Masks_Required_in_Public were used for analysis.

The thrid data is the [unemployment rate](https://beta.bls.gov/dataViewer/view/timeseries/LAUCN080310000000003) data about Denver, which is from the U.S Bureau of Labor Statistics. There are five attributes in the dataset, as explained below

| Attributes | Description |
| --- | --- |
| Series ID| Unique id that indicates which location the series is about|
| Year| Year of the data |
| Period | Month of the data|
| Label| In the format of year-month to indicate time|
| Value | Monthly unemployment rate in percentage|

Only the attributes label and value were used for the analysis. 

## Explanation of Each File
[A4-visualization.docx](A4-visualization.docx) is the assignment turned in for Assignment 4, which include a visualizaiton and a reflection report about the graph. The assignment aims to explain how masking policy affects the progression of confirmed COVID cases through the visualization. 

[A5-plan.docx](A5-plan.docx) is the assignment turned in for Assignment 5, which documents my plan about carrying out analysis for the project. 

[A6-presentation.pptx](A6-presentation.pptx) is the powerpoint I used for the in-class presentation. 

[A7-final-report.docx](A7-final-report.docx) is the final report turned in for Assignment 7. 

[DATA-512-Project.ipynb](DATA-512-Project.ipynb) is a jupyter notebook that documents all the code that has been used from Assignment 4-7. 

## Code Attribution
I would like to thank Jin Hyun Cheong on his [post](https://towardsdatascience.com/four-ways-to-quantify-synchrony-between-time-series-data-b99136c4a9c9) about cross correlation. The code of drawing cross correltion graph was adapted from the code he shared in the post. 
## Licenses
Datasets used for this project is licensed under [MIT](LICENSE).

The COVID-19 data is licensed under [Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode), which means I am allowed to share and adapt the data without specific permission. 

As per [Q&A section](https://www.cdc.gov/Other/policies.html) in CDC, the second dataset is in the public domain and may be freely used or reproduced without obtaining copyright permission. 

According to the [linking and copyright information](https://www.bls.gov/bls/linksite.htm), the third dataset is in the public domain and is free to be used without specific permission but required to cite the U.S. Bureau of Labor Statistics as a source.
