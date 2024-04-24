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

## Executive Summary

### Project Background and Context:
- SpaceX's Falcon 9 rocket stands out for its ability to significantly reduce launch costs by reusing its first stage.      Based on its website SpaceX's Falcon 9 rocket launch  has a price tag of 62 million USD compared to upwards of 165        million USD from other providers.
- Determining whether the first stage will land, helps calculating the cost of a launch. This information can be used if    an alternate company intends to bid against space X for a rocket launch.

### Key Questions to Address:
- Which launch site exhibits the highest success rate in terms of successful Falcon 9 first stage landings? 
- What factors (payload, orbit type, flight no, etc.) contribute to the highest and lowest outcome success rates? 
- Which machine learning models best predict if the first stage will land given the available data?



