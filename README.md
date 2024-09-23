# Road Traffic Accident Analysis and Prediction in Great Britain (UK)

## Overview

This project involves an in-depth analysis of road traffic accidents that occurred in Great Britain in the year 2020. The data is stored in a SQLite database and includes detailed information about each accident, the vehicles involved, and the resulting casualties. The objective of this project is to analyze the provided dataset, identify patterns and risk factors, and offer data-driven insights to government agencies for improving road safety. Additionally, predictive models are developed to assess the severity of accidents and help reduce the frequency and impact of future incidents.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Objectives](#objectives)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Modeling and Prediction](#modeling-and-prediction)
  - [Apriori Algorithm](#apriori-algorithm)
  - [Outlier Detection](#outlier-detection)
  - [RandomForestClassifier](#randomforestclassifier)
- [Findings and Results](#findings-and-results)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)
- [Requirements](#requirements)
- [How to Use](#how-to-use)
- [Contributors](#contributors)

## Introduction

In the year 2020, the Great Britain government recorded detailed traffic accident data. This project utilizes that data to identify patterns, assess accident severity, and suggest actionable improvements to road safety. The analysis focuses on identifying accident hotspots, patterns of risk during different times of the day or week, and key factors that contribute to more severe accidents.

## Dataset

The dataset consists of four tables stored in a SQLite database:

1. **Accident**: Contains details about each accident (e.g., location, time, and conditions).
2. **Casualty**: Information regarding casualties, including severity and type (pedestrian, motorist, etc.).
3. **Vehicle**: Describes vehicles involved in the accidents (e.g., type, model, and condition).
4. **Also**: Additional details related to accident conditions.

### Key Features:
- Accident occurrence time and location
- Type and severity of accidents
- Vehicles involved in accidents
- Casualty information (injuries, fatalities, etc.)

## Objectives

1. Analyze the dataset to identify patterns and trends in road traffic accidents.
2. Build predictive models to estimate the severity of accidents.
3. Use clustering to identify accident hotspots.
4. Recommend actions to government agencies to reduce road accidents and improve safety.

## Data Preprocessing

- Data cleaning: Handling missing values, correcting inconsistent entries.
- Feature extraction: Creating relevant features from the dataset (e.g., accident time, vehicle type).
- Transformation: Encoding categorical variables and normalizing numeric data.
- Splitting data: Dividing the dataset into training and testing sets for machine learning models.

## Exploratory Data Analysis (EDA)

Several exploratory techniques were used to uncover patterns in the dataset:

- **Accident frequency**: High accident rates were observed during weekdays, especially during peak business hours.
- **Motorbike vs. Pedestrian accidents**: A significant difference was observed between these two categories in terms of frequency and severity.
- **Hotspot Identification**: Clustering methods helped identify accident-prone areas.
- **Time of the Day/Week Analysis**: Analyzed the impact of time on accident severity.

## Modeling and Prediction

### Apriori Algorithm

The **Apriori algorithm** was used to discover frequent itemsets and association rules from the dataset. This helped in identifying patterns that frequently appear together, such as specific types of accidents occurring under certain weather conditions.

### Outlier Detection

Outlier detection methods were used to identify anomalies in the data that could indicate unusually severe accidents or exceptional circumstances that may need further investigation.

### RandomForestClassifier

A **RandomForestClassifier** model was developed to predict the severity of accidents (e.g., fatal, serious, or slight). The model achieved high accuracy, particularly for predicting fatal accidents, based on key features like accident location, vehicle type, and time of the day.

### Performance Metrics

- Accuracy: High accuracy in classifying severe and fatal accidents.
- F1 Score: Measured the model's ability to balance precision and recall.
- Confusion Matrix: Visualized the model's classification performance.

## Findings and Results

1. **Peak Hours**: A higher frequency of accidents was observed during peak business hours (8 AM - 9 AM and 5 PM - 7 PM).
2. **Weekdays vs. Weekends**: Accidents were more frequent on weekdays, particularly in urban areas.
3. **Motorbike and Pedestrian Accidents**: Pedestrians were more vulnerable in urban areas, while motorbike accidents were frequent on highways.
4. **Accident Hotspots**: Clustering algorithms identified accident hotspots, which are high-risk areas for future incidents.
5. **Severity Prediction**: The RandomForestClassifier achieved high accuracy, with the ability to predict fatal accidents based on a variety of features.

## Recommendations

1. **Improved Road Design**: Focus on accident-prone areas to redesign roads for better safety.
2. **Weather-responsive Plans**: Develop plans to address accident risks during poor weather conditions.
3. **Enhanced Public Awareness**: Campaigns focused on accident-prone times and locations.
4. **Traffic Regulation**: Implement stricter controls during high-risk hours.

## Conclusion

By analyzing traffic accident data from 2020, we were able to uncover important patterns and build predictive models that can help government agencies make data-driven decisions to improve road safety. Future work can include adding more data from previous years and improving the model's performance through further tuning and testing.

## Requirements

To run the project, you need the following:

- Python 3.7+
- SQLite3
- Required Python libraries:
  - Pandas
  - NumPy
  - Scikit-learn
  - Matplotlib
  - Seaborn
  - PySpark
  - Flask (for deploying models)
  
Install all dependencies using the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/road-traffic-accidents-analysis.git
   ```

2. Navigate to the project directory:
   ```bash
   cd road-traffic-accidents-analysis
   ```

3. Set up the database by importing the SQLite file provided in the repository.

4. Run the Jupyter notebooks or scripts provided for analysis and modeling.

5. Use the Flask app to deploy the predictive models.

## Contributors

- Muhammad Talha Zafar - [LinkedIn](https://www.linkedin.com/in/muhammad-talha-zafar-3117481b3/) | [GitHub](https://github.com/TalhaZafarAi)
  
---

Feel free to reach out for any suggestions or contributions to the project. Together, we can help reduce road accidents and enhance safety!

---


