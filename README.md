IBM-APPLIED-DATA-SCIENCE-CAPSTONE-PROJECT

OUTLINE
1. Executive Summary
2. Introduction
3. Methodology
4. Results
5. Conclusion
6. Appendix 

OVERVIEW

This project adopts a comprehensive approach to predicting the successful landing of the SpaceX Falcon 9 first stage. Data was collected from Wikipedia through web scraping and supplemented with detailed launch records from the SpaceX API. The dataset was cleaned and formatted through handling missing values, encoding categorical variables, standardization, and removal of irrelevant features. Exploratory data analysis was performed using SQL to extract insights, supported by visualizations such as scatter plots and bar charts created with Matplotlib and Seaborn. Interactive geographic analysis was conducted using Folium maps, and a Plotly Dash application was developed to explore launch success rates dynamically.
The prepared data was split into training and testing sets, normalized, and used to train predictive models. Hyperparameter tuning was applied to optimize model performance, followed by evaluation of the models to assess their accuracy.

Data Collection Methodology:
Web Scraping
Data was sourced from Wikipedia, providing historical information about the SpaceX Falcon 9 launch vehicle.
SpaceX API: Additional data was sourced through the SpaceX API which supplied detailed records of launches, including launch dates, boosters informations and launch site locations.
Perform Data Wrangling: Data cleaning includes handling missing values, hot encoding, standardization, maintenance of consistency, removing irrelevant columns.
Perform exploratory data analysis (EDA) using visualization and SQL: EDA with SQL to derive insights and answer questions regarding data sets.
Visualizations of launch success rate, launch sites, payloads through scatter graphs , bar charts using Seaborn and Matplotlib 
Perform interactive visual analytics using Folium and Plotly Dash: Use of Folium in generating interactive maps. 
Development of plotly dash application to analyze launch success rates.
Perform predictive analysis using classification models: Machine Learning Predictive Analysis, Train data, test and split data
and data normalization. Hyperparameter tuning to maximize accuracy of predictive models
Evaluation of Models

INTERACTIVE MAP WITH FOLIUM

An interactive map was created using Folium to visualize SpaceX Falcon 9 launch sites and their outcomes. All launch locations were plotted and enhanced with markers, circles, and lines to distinguish between successful and failed launches. Launch outcomes were encoded as binary classes, where 0 indicates failure and 1 indicates success. Color-coded marker clusters were used to compare success rates across launch sites and identify locations with higher mission success. Distance calculations were also performed to analyze the proximity of launch sites to surrounding features such as coastlines, railways, highways, and cities, helping assess whether launch sites are strategically positioned away from populated areas while remaining close to key infrastructure.

DASHBOARD APP WITH PLOTLY DASH
An interactive dashboard was developed using Plotly Dash to analyze launch performance. Pie charts were used to display the distribution of total launches by site, while scatter plots illustrated the relationship between payload mass (kg) and launch outcome across different booster versions.

CONCLUSION

From the analysis of the datasets, several key insights were identified. Launch sites with a higher number of flights tend to have higher success rates, and overall launch success increased steadily from 2013 to 2020. Among the orbits analyzed, ES-L1, GEO, HEO, and SSO recorded the highest success rates, while KSC LC-39A emerged as the most successful launch site.
Geospatial analysis using interactive maps and dashboards highlighted the influence of launch site location and payload mass on Falcon 9 first-stage landing success. In the predictive analysis, multiple classification models were evaluated. The Decision Tree classifier achieved the highest accuracy (0.8750), outperforming Logistic Regression, SVM, and KNN (each with an accuracy of 0.8333), making it the most effective model for predicting Falcon 9 landing success in this study.

