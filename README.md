# Predicting-Hazardous-Near-Earth-Objects-NEOs
<b>Overview</b> </br>
<p>This project focuses on predicting whether a Near-Earth Object (NEO) is hazardous using a dataset provided by NASA. The dataset contains observations of NEOs from 1910 to 2024, with features such as absolute_magnitude, relative_velocity, miss_distance, and average_diameter. The goal is to build a machine learning model that can accurately classify NEOs as hazardous or non-hazardous.</p>
<b>Project Description</b> </p>
<p>In this project, we use machine learning to predict whether a Near-Earth Object (NEO) is hazardous. The dataset contains 338,199 records, each representing an object in space that has been monitored for its proximity to Earth. Some of these objects are classified by NASA as "is_hazardous," indicating that they pose a potential danger to our planet.

The project involves:

- Data cleaning and preprocessing.

- Exploratory Data Analysis (EDA) to understand the dataset.

- Handling imbalanced data using SMOTE (Synthetic Minority Over-sampling Technique).

- Training and evaluating Decision Tree and Random Forest models.

- Feature selection to improve model performance.</p>
 <br> 
<b> Steps</b></br>
<br>
<b> Data Cleaning </b></br>

- Handled missing values by dropping rows with null values.

- Created a new feature, average_diameter, by averaging estimated_diameter_min and estimated_diameter_max.

- Dropped redundant columns (estimated_diameter_min, estimated_diameter_max, orbiting_body).

<b>Exploratory Data Analysis (EDA)</b></br>
- Visualized the distribution of the target variable (is_hazardous).

- Analyzed the relationship between features and the target variable using boxplots and pie charts.

- Identified class imbalance in the dataset (12% hazardous NEOs vs. 88% non-hazardous NEOs).

<b> Data Preprocessing </b></br>
- Encoded the is_hazardous column from True/False to 1/0.

- Addressed class imbalance using SMOTE to oversample the minority class.

- Split the data into training and testing sets.

<b> Model Training and Evaluation </b></pr> 

- Trained a Decision Tree Classifier and evaluated its performance.

- Trained a Random Forest Classifier and compared its performance with the Decision Tree.

- Performed feature selection using SelectFromModel and RFE to identify the most important features.

- Retrained the models using selected features and evaluated their performance.

  <br>

<b> Results </b></br>
</br>
<b> Decision Tree Classifier </b><br>
- Accuracy: 93.97%

- Confusion Matrix:


  [[55541  3499] <br>
 [ 3611 55353]]
<br>

<b> Random Forest Classifier </b><br>
- Accuracy: 95%

- Confusion Matrix:


    [[56091  2949] <br>
 [ 2865 56099]] 
<br>
