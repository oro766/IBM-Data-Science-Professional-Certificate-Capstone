# IBM-Data-Science-Professional-Certificate-Capstone
![687474~1](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/assets/131335559/87812876-ae8f-4a42-8351-63cacf266f1e)


## Executive Summary

### Summary of Methodologies:
- **Data Collection:** Utilized SpaceX REST API calls and Wikipedia web scraping.
- **Data Wrangling:** Preprocessed data via one-hot encoding for ML readiness.
- **Exploratory Data Analysis:** Utilized visualization and SQL for insights.
- **Interactive Visual Analytics:** Employed Folium and Plotly Dash for dynamic exploration.
- **Predictive Analysis:** Utilized LR, SVM, KNN, and DT classification models for predictions.

### Summary of All Results
- **Dataset:** Consisted of 90 rows × 83 columns, influencing ML model selection.
- **Best Predictive Models:** Logistic Regression, Support Vector Machine, K Nearest Neighbors.
- **Model Accuracy:** Achieved 0.85 on training and 0.83 on test data.
- **Key Insights:**
    - Payload mass between 1,952kg and 5,300kg yielded most positive outcomes.
    - Booster version "FT" was most successful, while "v1.1" was least successful.
    - Launch site KSC LC-39A generated the highest successful outcomes.


## Introduction

### Project Background and Context:
- SpaceX's Falcon 9 rocket stands out for its ability to significantly reduce launch costs by reusing its first stage. Based on its website SpaceX's Falcon 9 rocket launch  has a price tag of 62 million USD compared to upwards of 165 million USD from other providers.
- Determining whether the first stage will land, helps calculating the cost of a launch. This information can be used if an alternate company intends to bid against space X for a rocket launch.

### Key Questions to Address:
- Which launch site exhibits the highest success rate in terms of successful Falcon 9 first stage landings? 
- What factors (payload, orbit type, flight no, etc.) contribute to the highest and lowest outcome success rates? 
- Which machine learning models best predict if the first stage will land given the available data?


## Methodology
![SpaceX REST calls](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/assets/131335559/d03ea6f3-64f0-4b8d-9db3-ee0adb5f9078)

### Lab 1: Collecting the data:
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/jupyter-labs-spacex-data-collection-api_oo.ipynb)<br> 
- Request to the SpaceX API
- Clean the requested data

**Input Data:** [Spacex API (static JSON file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/API_call_spacex_api.json) <br>
**Output Data:** [Dataset Part 1 (CSV file)](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/1b244b5e61b5fcdb754a2065f7db0235dccf2814/dataset_part_1.csv<br>)

### Lab 2: Data Collection with Web Scraping:
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/jupyter-labs-webscraping_oo.ipynb)<br> 
- Extract a Falcon 9 launch records HTML table from Wikipedia
- Parse the table and convert it into a Pandas data frame

**Input Data:** [Wikipedia (static HTML file)](https://en.wikipedia.org/w/index.php?title=List_of_Falcon_9_and_Falcon_Heavy_launches&oldid=1027686922") <br>
**Output Data:** [Dataset - SpaceX Webscraping (CSV file)](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/spacex_web_scraped.csv)

### Lab 3: Data wrangling: 
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/labs-jupyter-spacex-Data%20wrangling_oo.ipynb)<br> 
- Exploratory Data Analysis
- Determine Training Labels

**Input Data:** [Dataset Part 1 (CSV file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/dataset_part_1.csv")) <br>
**Output Data:** [Dataset Part 2 (CSV file)](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/dataset_part_2.csv)

### Lab 4: EDA with SQL: 
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/jupyter-labs-eda-sql-coursera_sqllite_oo.ipynb)<br> 
- Understand the Spacex DataSet
- Load the dataset into the corresponding table in a Db2 database
- Execute SQL queries to answer assignment questions

**Input Data:** [Spacex (CSV file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/labs/module_2/data/Spacex.csv") <br>

### Lab 5: EDA with Visualization:
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/jupyter-labs-eda-dataviz.ipynb.jupyterlite_oo.ipynb)<br> 
- Exploratory Data Analysis
- Preparing Data Feature Engineering

**Input Data:** [Dataset Part 2 (CSV file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/dataset_part_2.csv") <br>
**Output Data:** [Dataset Part 3 (CSV file)](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/6565629ebf0c663fd25a4322425d0e816a27a794/dataset_part_3.csv)

### Lab 6: Interactive Visual Analytics with Folium:
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/8f61965396d0c8e0c5c3830123da43eec7a0467a/lab_jupyter_launch_site_location.jupyterlite_oo.ipynb)<br> 
- Mark all launch sites on a map
- Mark the success/failed launches for each site on the map
- Calculate the distances between a launch site to its proximities

**Input Data:** [Spacex Launch Geo Data Set (CSV file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/spacex_launch_geo.csv') <br>

### Lab 7: Interactive Dashboard with Ploty Dash: 
**Description:** [Python Code](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/8f61965396d0c8e0c5c3830123da43eec7a0467a/spacex_dash_app.py)<br> 
- Launch Site Drop-down Input Component
- Callback function to render success-pie-chart based on selected site dropdown
- Range Slider to Select Payload
- Callback function to render the success-payload-scatter-chartscatter plot

**Input Data:** [Spacex Launch Dash Data Set (CSV file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/spacex_launch_dash.csv) <br>

### Lab 8: Machine Learning Prediction:
**Description:** [Jupyter Notbook](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/8f61965396d0c8e0c5c3830123da43eec7a0467a/SpaceX_Machine_Learning_Prediction_Part_5.jupyterlite_oo.ipynb)<br> 
Perform exploratory Data Analysis and determine Training Labels<br>
- create a column for the class
- Standardize the data
- Split into training data and test data

Find best Hyperparameter for SVM, Classification Trees and Logistic Regression<br>
- Find the method performs best using test data


**Input Data:** [Dataset Part 2 (CSV file](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/dataset_part_2.csv") & [Dataset Part 3 (CSV file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/dataset_part_3.csv')<br>


## Conclusion
- The data set 90 rows × 83 columns is rather small which was considered by the selection of machine learning (ML) models.
- The ML models with the best predictive outcomes are:
    - Logistic Regression (logreg_cv)
    - Support Vector Machine (SVM_cv)
    - K Nearest Neighbors (KNN_cv)
- The accuracy of the previously mentioned models are at 0.85 on the training and 0.83 on the test data.
- Further considerations:
    - Payload mass between 1,952kg and 5,300kg have the most positive outcomes.
    - FT is the most successful booster version and v1.1 is the least successful one. 
    - The launch site Kennedy Space Center Launch Complex 39A (KSC LC-39A) generated the highest numbers of successful          outcomes.

## Appendix
PowerPoint Presentation as PDF file: [ds-capstone-template-coursera - oo.pdf](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/files/15089650/ds-capstone-template-coursera.-.oo.pdf)
