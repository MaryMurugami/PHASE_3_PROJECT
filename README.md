# PHASE_3_PROJECT
TANZANIA WATER WELLS CLASSIFICATION

## BUSINESS UNDERSTANDING

Tanzania is an East African developing country known for its vast wilderness areas and an estimated population of 63 Million in East Africa. One of the key challenges faced by most developing countries in the region is access & provision of clean water; this problem is exacerbated during the dry seasons when majority of existing wells run dry. Despite the establishment of many water points in the country, some are in need of repair while others have failed altogether.

### Objective

1.1.0- Main Objective
To predict the condition of water wells in Tanzania using information about the pumps, installation dates and location. The information gathered will be used to provide insights to the Tanzanian government and decision makers on how to plan in future for the installation, repair and maintenace of wells.

1.1.1 
To identify wells that are in need of repair or have failed completely, which could help the government or NGOs to plan and prioritize the maintenance and repair work.

1.1.2
To analyze the data, then identify patterns and trends to enable the Tanzanian government make informed decisions on where new wells can be built and ideal locations.

1.1.3 
To Develop a machine learning classifier model to predict the status of water wells in Tanzania.

1.1.4
The model shoud be able to predict which pumps are functional, which need some repairs, and which don't work at all.

## Data Understanding

Data Sets complied an provided by Taarifa and Tanzanian Ministry of Water as below:

- *Test set values*: The independent variables that need predictions
- *Training set labels*: The dependent variable (status_group) for each of the rows in Training set values
- *Trainig set values*: The independent variables for the training set

Our goal is to predict the operating condition of a waterpoint for each record in the dataset. We are provided the following set of information about the waterpoints. We shall proceed to preprocess both the traiing and testing data sets before we subject them to our model.




## Data Cleaning, exploration and visualization 
We Imported the necessary Libraries, Loaded & Inspected the Datasets, then converted the counts of each category into percentages. This is important in our dataset because it will help us understand the distribution and balance of the different categories in our data. 
 
-Here we needed to understand the prevalence and percentage of functional wells, those that need repair and the non-functioning ones.
- This will help us prioritize maintenance, those that require repair and where resources can be allocated.
- With time, the Tanzanian Government can monitor and track changes in the wells over time by comparing the percentages throughout the different periods and any shifts in the condition of the water wells.

## Data Modelling
We tested the different models and basedn on the accuracy score we settled on the KNN classifier 
![image](https://github.com/MaryMurugami/PHASE_3_PROJECT/assets/122040156/098e474c-7d9d-446a-b81e-c2ae2208237e)

## Recommendations
For large complex datasets like the Tanzania wells data, which had 59,400 observations, simple data analysis using Excel would be difficult, so Machine Learning is ideal because it is used for large complex datasets allowing the visualization of patterns and relationships that would ideally be missed by simple data analysis methods.The Tanzania well dataset has both categorical and numerical datasets, so ML was able to provide algorithms to identify patterns and relationships in the data such as in places where wells in a sparse population, the wells was rarely used and needed repair. Such wells need to be identified if there is need for repair or maintenance

For large dataset, data cleaning is key to ensure data quality prior to applying ML algorithms, in this data we dropped variables like latitude, longitude, district codes etc. which were not necessary for our model. The characteristic of the dataset is determined by the data type and goal of analysis, e.g. For the Tanzania wells data set we used Decision tress KNN was the best model it had 73.9%  accuracy score meaning the model correctly predicted the classification levels
The analysis showed that data collected should highlight more on non-functional pumps or those in need of repair so that they can plan resource allocation for repairs and maintenance 

CONCLUSION/SUGGESTIONS
Areas requiring improvement to further increase our preffered models' predictive power:

- Further Tuning: More fine tuning to improve model accuracy
- Try More Classifiers & Consider using more complex ensemble models (Bagging, Stacking)
- Consider using more features provided in Original dataset






