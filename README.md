# Confused EEG Analysis

This project aims to analyze EEG (Electroencephalogram) data to identify patterns and correlations related to confusion levels. It utilizes various data analysis techniques and machine learning models to gain insights into the dataset.

## Dataset

The dataset used in this project can be found at [Kaggle](https://www.kaggle.com/datasets/wanghaohan/confused-eeg). It consists of EEG recordings in separate CSV files and demographic information about the subjects.

To prepare the data for analysis, we concatenate the CSV files into a single Pandas DataFrame and perform data cleaning tasks, such as handling misspellings and style inconsistencies.

## Exploratory Data Analysis

### Pandas Profiling Report

To gain a comprehensive overview of the dataset, we generate a Pandas Profiling Report. This report provides detailed statistical information, visualizations, and correlations for each feature in the dataset. It helps us understand the distribution, missing values, and potential relationships between variables.

### Univariate Analysis

We perform visual analysis of the dataset's categorical and continuous features. This analysis allows us to examine the distribution and characteristics of each feature individually.

### Multivariate Analysis

Utilizing visualizations, we examine the relationships and correlations among the continuous features in the dataset. These visualizations offer valuable insights into the connections and dependencies between the continuous variables, shedding light on potential associations within the data.

## Data Preprocessing

Before training our models, we perform data preprocessing steps, including renaming columns, assigning time stamps to each video trial, merging demographic information, and performing one-hot encoding on categorical variables.

## Model Training

We utilize TensorFlow Keras to build our neural network model. The model is trained using the prepared dataset for 100 epochs, with a learning rate of 0.001 and a batch size of 20.

## SHAP (SHapley Additive exPlanations)

To interpret the predictions made by our trained model, we employ the SHAP library. SHAP provides explanations for individual predictions, highlighting the features that contribute the most to the model's decision-making process.

## Results and Insights

By analyzing the SHAP values, we gain insights into the significant features influencing the confusion levels. These insights can help in understanding the underlying patterns and factors contributing to confusion.

## Conclusion

This project demonstrates the application of data analysis and machine learning techniques to EEG data to understand confusion levels. By exploring the dataset, training a neural network model, and interpreting the results using SHAP, we uncover valuable insights that contribute to our understanding of the relationship between EEG signals and confusion levels.

Feel free to explore the code and adapt it to your specific needs. If you have any questions or suggestions, please feel free to reach out.
