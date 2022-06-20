# Project Portfolio

---
I am an Information Systems graduate student (M.Sc.) with experience and passion for machine learning, cloud-native web development, cloud computing & digital transformations.

This portfolio page shows an overview of some of my projects during my professional work as well as my academic studies. These projects cover following topics:
- Data Science & Business Intelligence
- IT Governance & Consulting

---

## Data Science & Business Intelligence
---

### Big Data Analytics (~35 Million Data Points) - Chicago Taxi Trip Pattern 

#### Final Advanced Analytics & Application Course Project (M.Sc.) - University of Cologne

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/SepehrRad/aaa21)

This study focused on the dynamics of the ride-hailing business in Chicago. The open Chicago City data of taxi trips in 2015 was used to provide analysis and recommendations for bringing value to the taxi business in Chicago. Furthermore, the result of the project can be used for the introduction and planning of electric ride-hailing services in Chicago.

The Project had four distinct parts: EDA, customer clustering and analysis, demand prediction in geo-temporal resolution, charging location optimization.

In the first part of the project, we visualized the taxi trip data, in different spatial and temporal resolutions, to get an insight into Chicago’s taxi demand patterns. The data was geographically discretized using Uber’s H3 library. This approach yielded very interesting results. E.g. 90% of all trips take place in only ten Community Areas of Chicago, which are all part of the city center or at the airport. Or the fact that the overall demand increases during the morning stays constant over the course of the day, and starts rising in the evening with a peak at 19:00.

<div class="row">
  <div class="column">
    <img src="images/AAA_pickups_ca.png?raw=true" style="width:100%"/>
  </div>
  <div class="column">
    <img src="images/AAA_starttimes.png?raw=true" style="width:100%"/>
  </div>
</div>


The goal of the second part of the project was getting a better understanding of how the customers are using mobility services and proposing optimization suggestions for the business operations. After creating a set of relevant geo-temporal features such as airport distance and holidays, the customers were assigned into six distinct clusters, using both soft (GMM) and hard clustering (KNN) approach:

| Cluster | Label | Trip Start Hour | Trip Kilometers | Trip Minutes | Trips(%) |
| 0 | `After Party Customers` | 0-2 | 1 - 4 | 5 - 10 | 9.8 |
| 1 | `Urban Evening Customers` | 19-22 | 1 - 3 | 5 - 9 | 21.9 |
| 2 | `Suburban Evening Customers` | 18-22 | 4 - 7 |  4 - 18 | 14.7 |
| 3 | `Daytime Short-Distance Customers` | 10-15 | 1 - 2 | 4 - 7 | 19.0 |
| 4 | `Long Distance Customers` | 5 - 14 | 4 - 10 | 16 - 22 | 9.9 |
| 5 | `Daytime Medium Distance Customers` | 9 -15 | 2 - 4 | 10 - 13 | 19.0 |

<div class="row">
  <div class="column">
    <img src="images/AAA_BoxPlot_SoftClustering.png?raw=true" style="width:100%"/>
  </div>
  <div class="column">
    <img src="images/AAA_Scatter_SoftClustering.png?raw=true" style="width:100%"/>
  </div>
</div>

The third part of the project aimed at predicting demand in different geo-temporal resolutions. To get better model performance in addition to synthetic geo-temporal features, Chicago weather information was gathered and added to the model's input. Deep Artificial Neural Networks and SVMs were used for this task:

<img src="images/AAA_prediction_results.png?raw=true"/>

Finally, in the fourth section of the project, the charging stations allocation problem for electric taxi vehicles was tackled. This was first formulated mathematically as a linear programming problem under constraints and then solved using the Python PuLP library:

<img src="images/AAA_charging_locs.png?raw=true"/>


---

### Big Data Analytics (~20 Million Data Points) - Impact of Covid-19 on New York Cab Industry & Public Mobility

#### Final Programming Data Science Course Project (M.Sc.) - University of Cologne

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/SepehrRad/pds21)

The aim of this project was to analyze the impact of COVID-19 on the yellow cab industry in New York. Furthermore, using the open-source NYC Taxi & Limousine Commission (TLC) data in 2020 the project aimed to unfold opportunities and recommendations to the taxi industry.

The project was divided into two main parts. In the first section, the EDA part, all trips were interactively visualized using Panel and multiple visualization libraries. (E.g. Plotly, Folium)

The explanatory analysis showed the taxi hot zones as well as the impact of Covid-19 on public mobility:

<img src="images/PDS_Pickup_Hot_Zones_NYC.png?raw=true"/>
<img src="images/PDS_Corona_Impact_NYC.png?raw=true"/>


In the second section, the prediction modeling part, three models were built to predict fare amount, expected trip distance, and payment type. The apparent effect of covid-19 was taken into account by engineering an array of relevant features such as covid-19 lockdowns timeline as well as school restrictions. The Random Forest Classifier and Regressor were built using the XGBoost library and fine-tuned using grid search:

| Model | Prediction Target | Evaluation Score |
| --- | --- | --- |
| `Random Forest Classifier` | Payment Type | 0.88 Percision - 0.81 F1 |
| `Random Forest Regressor` | Fare Amount ($) | 0.385 MAE - 1.289 RMSE |
| `Random Forest Regressor` | Trip Distance (KM) | 0.407 MAE - 0.665 RMSE |

---

### Sustainable Mobility in Heidelberg & Marburg

#### Final Analytics & Application Course Project (M.Sc.) - University of Cologne

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](/https://github.com/SepehrRad/analyticsAndapps)

Showing how fleet operators can make use of increasingly ubiquitous real-time data streams in order to optimize their bike supply management and thus boost customer satisfaction and revenue, was the focus of this project. The underlying hypothesis was that hourly, daily, seasonal, and weather-related trends influence and positively correlate with the demand of the bike-sharing system. In order to factor in weather-related demand fluctuations, the weather information was gathered and added to the NexBike data sets.

Five key performance indicators (KPIs) were developed to track and improve the business service level. These provided indications of the current operations and how well the fleet is doing in terms of utilization, revenue, coverage, and activations:

<div class="row">
  <div class="column">
    <img src="images/aa_violin_plots.png?raw=true" style="width:100%"/>
  </div>
  <div class="column">
    <img src="images/aa_utilization.png?raw=true" style="width:100%"/>
  </div>
</div>

<div class="row">
  <div class="column">
    <img src="images/aa_seasonalities.png?raw=true" style="width:100%"/>
  </div>
  <div class="column">
    <img src="images/aa_heidelberg_pickups.png?raw=true" style="width:100%"/>
  </div>
</div>


Furthermore, three different prediction models were built using two heterogeneous data sets of Nextbike users in Heidelberg and Marburg from 2019. The customer demand was modeled in daily and hourly resolution using Time Series Analysis (Facebook Prophet), Ridge & Lasso Regression, and Random Forest Regressor (XGBoost). Based on the daily result we chose XGBoost model for final deployment.

| City | Model | MAE | MAPE |
| --- | --- | --- | --- |
| Marburg | `FBProphet` | 110.69 | 28.77 % |
| Marburg | `Polynomial Regression` | 89.6 | 32.96 % |
| Marburg | `Ridge Regression` | 89.5 | 33.68 % |
| Marburg | `Random Forest Regressor` | 76.26 | 33.38 % |
| Heidelberg | `FBProphet` | 68.88 | 28.59 % |
| Heidelberg|  `Polynomial Regression` | 53.19 | 40.84 % |
| Heidelberg | `Ridge Regression` | 53.11 | 87.69 % |
| Heidelberg | `Random Forest Regressor` | 47.35 | 26.31 % |


Finally, the customers were clustered based on their demand patterns. Thus, enabling NextBike to identify trip types as well customer types:

<div class="row">
  <div class="column">
    <img src="images/aa_heidelberg_clusters.png?raw=true" style="width:100%"/>
  </div>
  <div class="column">
    <img src="images/aa_marburg_clusters.png?raw=true" style="width:100%"/>
  </div>
</div>

---

---

### Creating & Implementing a Business Intelligence (BI) Concept for an Enterprise Web Application

#### Final B.Sc. Practical Project in Cooperation with innovas GmbH (.MSG Group) - Cologne University of Applied Sciences

As part of my final practical project work at the Cologne University of Applied Sciences, I developed and implemented a BI concept for an online platform of the innovas GmbH delivering data to different health insurance companies.

In the first phase of the project, I carried out a requirements analysis for insurance companies involved based on a goal-oriented approach using i*-framework.

After defining the use cases as well as the organizational and technical constraints, the implementation concept was introduced which included an ETL process written both in Java and Python that transferred the data from the operational database into multidimensional data lakes. Furthermore, PowerBI was used for analysis, reporting, and interactive visualizations.

Finally, since the data was highly sensitive according to the General Data Protection Regulation (DSGVO in German) various security measures were taken to ensure the security of data storage and transport. E.g. asymmetric encryption and secure data vaults.

The work product was successfully deployed and is in use since 2020.


---

## IT Governance & Consulting

---

### Development of Business Intelligence Strategies for Small and Medium-sized Companies in the Health Care Industry

#### Bachelor Thesis in Cooperation with innovas GmbH (.MSG Group) - Cologne University of Applied Sciences

The aim of my bachelor thesis was to define guidelines for the development of BI strategies for
Small- and Medium-sized Enterprises (SMEs) in the healthcare industry.

To achieve this goal, I developed an ontology of BI strategy, with the help of which the BI strategy is semantically defined and its most important fields of action are introduced. By applying this methodology one can ensure consistent use of language that facilitates the representation of complex relationships between terms in this domain. E.g. BI Strategy, IT Strategy, Business Strategy, IT Governance. Thus, helping SMEs orienting themselves in the complex BI landscape.

Finally, based on the developed ontology and extensive literature review, I presented _eight guidelines_ according to the TOGAF-Format (Statement, Rationale, Implications), which facilitates the development of a BI strategy for any SME in the healthcare industry.

---




