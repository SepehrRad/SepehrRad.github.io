# Project Portfolio

---

## Data Science
---

### Chicago Taxi Trip Pattern Analysis

#### Final Advanced Analytics & Application Course Project - University of Cologne

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/SepehrRad/aaa21)

This study focused on the dynamics of the ride-hailing business in Chicago. The open Chicago City data of taxi trips in 2015 was used to provide analysis and recommendations for bringing value to the taxi business in Chicago. Furthermore, the result of the project can be used for the introduction and planning of electric ride-hailing services in Chicago.

The Project had four distinct parts: EDA, customer clustering and analysis, demand prediction in geo-temporal resolution, charging location optimization.

In the first part of the project, we visualized the taxi trip data, in different spatial and temporal resolutions, to get an insight into Chicago’s taxi demand patterns. The data was geographically discretized using Uber’s H3 library. This approach yielded very interesting results. E.g. 90% of all trips take place in only ten Community Areas of Chicago, which are all part of the city center or at the airport. Or the fact that the overall demand increases during the morning stays constant over the course of the day, and starts rising in the evening with a peak at 19:00.
<img src="images/AAA_starttimes.png?raw=true"/><br>
<img src="images/AAA_pickups_ca.png?raw=true"/>


The goal of the second part of the project was getting a better understanding of how the customers are using mobility services and proposing optimization suggestions for the business operations. After creating a set of relevant geo-temporal features such as airport distance and holidays, the customers were assigned into six distinct clusters, using both soft (GMM) and hard clustering (KNN) approach:

<img src="images/AAA_Customer_Clusters_Chicago.png?raw=true"/><br>
<img src="images/AAA_BoxPlot_SoftClustering.png?raw=true"/>
<img src="images/AAA_Scatter_SoftClustering.png?raw=true"/>

The third part of the project aimed at predicting demand in different geo-temporal resolutions. To get better model performance in addition to synthetic geo-temporal features, Chicago weather information was gathered and added to the model's input. Deep Artificial Neural Networks and SVMs were used for this task:

<img src="images/AAA_prediction_results.png?raw=true"/>




---

### Impact of Covid-19 on New York Cab Industry & Public Mobility

#### Final Programming Data Science Course Project - University of Cologne

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/SepehrRad/pds21)

The aim of this project was to analyze the impact of COVID-19 on the yellow cab industry in New York. Furthermore, using the open-source NYC Taxi & Limousine Commission (TLC) data in 2020 the project aimed to unfold opportunities and recommendations to the taxi industry.

The project was divided into two main parts. In the first section, the EDA part, all trips were interactively visualized using Panel and multiple visualization libraries. (E.g. Plotly, Folium)

The explanatory analysis showed the taxi hot zones as well as the impact of Covid-19 on public mobility:
<br><br>
<img src="images/PDS_Pickup_Hot_Zones_NYC.png?raw=true"/>
<br><br>
<img src="images/PDS_Corona_Impact_NYC.png?raw=true"/>


In the second section, the prediction modeling part, three models were built to predict fare amount, expected trip distance, and payment type. The apparent effect of covid-19 was taken into account by engineering an array of relevant features such as covid-19 lockdowns timeline as well as school restrictions. The Random Forest Classifier and Regressor were built using the XGBoost library and fine-tuned using grid search:

| Model | Prediction Target | Evaluation Metric |
| --- | --- | --- |
| `Random Forest Classifier` | Payment Type | 0.88 Percision - 0.81 F1 |
| `Random Forest Regressor` | Fare Amount ($) | 0.385 MAE - 1.289 RMSE |
| `Random Forest Regressor` | Trip Distance (KM) | 0.407 MAE - 0.665 RMSE |

---

### Sustainable Mobility in Heidelberg & Marburg

#### Final Analytics & Application Course Project - University of Cologne

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](/https://github.com/SepehrRad/analyticsAndapps)

**Project Description:** Description

<img src="images/dummy_thumbnail.jpg?raw=true"/>

---

## Business Intelligence

---

### Creating an ETL Pipeline for an Enterprise Web Application

Final Bachelor project in cooperation with Innovas GmbH

**Project Description:** Delivering Encrypted Data to

---

### Development of Business Intelligence Strategies for Small and Medium-sized Companies in the Health Care Industry

Bachelor thesis in cooperation with Innovas GmbH

**Project Description:** Description

---




