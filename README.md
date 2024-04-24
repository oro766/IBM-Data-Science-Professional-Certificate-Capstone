# IBM-Data-Science-Professional-Certificate-Capstone

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

### Lab 1: Collecting the data:
**Description:**<br> 
    - Request to the SpaceX API<br>
    - Clean the requested data<br>

**Input Data:** [Spacex API (static JSON file)](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DS0321EN-SkillsNetwork/datasets/API_call_spacex_api.json) <br>
**Output Data:** [Dataset Part 1 (CSV file)](https://github.com/oro766/IBM-Data-Science-Professional-Certificate-Capstone/blob/1b244b5e61b5fcdb754a2065f7db0235dccf2814/dataset_part_1.csv<br>)

### Lab 2: Data Collection with Web Scraping:
**Description:** 

Input Data
Output Data

### Lab 3: Data wrangling: 
**Description:**

Input Data
Output Data

### Lab 4: EDA with SQL: 
Description
Input Data
Output Data

### Lab 5: EDA with Visualization:
Description
Input Data
Output Data

### Lab 6: Interactive Visual Analytics with Folium:
Description
Input Data
Output Data

### Lab 7: Interactive Dashboard with Ploty Dash: 
Description
Input Data
Output Data

### Lab 8: Machine Learning Prediction:
Description
Input Data
Output Data

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

