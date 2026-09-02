# Netflix Data Science Analysis

A practical Data Science project completed as part of the **Auspify Technologies Data Science Internship**. The project analyzes a Netflix Movies and TV Shows dataset using data preprocessing, exploratory data analysis, content-based recommendation techniques, and machine learning.

## Project Overview

This project demonstrates an end-to-end Data Science workflow, from cleaning and preparing raw data to extracting insights and building machine learning and recommendation models.

The analysis was performed using **Python and Google Colab**, with libraries including Pandas, NumPy, Matplotlib, and Scikit-learn.

## Completed Tasks

### 1. Data Cleaning & Preprocessing

The Netflix dataset was cleaned and prepared for analysis by:

* Inspecting the dataset structure and data types
* Identifying missing values
* Checking for duplicate records
* Converting date fields into a proper datetime format
* Handling placeholder values in the `country` column
* Extracting numerical duration features
* Creating a cleaned dataset for further analysis

**Dataset size after preprocessing:** 8,790 records and 12 columns.

### 2. Exploratory Data Analysis

Exploratory analysis was performed to identify patterns and trends in Netflix content.

Key areas analyzed:

* Movies vs. TV Shows
* Top countries producing Netflix content
* Most common content categories
* Distribution of release years
* Content trends over time

#### Key Findings

* **Movies:** 6,126 titles
* **TV Shows:** 2,664 titles
* The **United States** had the largest number of titles in the dataset.
* **International Movies** and **Dramas** were among the most common categories.
* Content was heavily concentrated in releases from approximately **2017–2021**.
* **2018** had the highest number of titles by release year.

Visualizations were created using Matplotlib to communicate these findings.

## Visualizations

### Content Type Distribution

![Content Type Distribution](screenshots/content_type.png)

### Top Countries

![Top Countries](screenshots/top_countries.png)

### Top Categories

![Top Categories](screenshots/top_categories.png)

### Release Year Trend

![Release Year Trend](screenshots/release_year_trend.png)

### Classification Model Accuracy

![Classification Model Accuracy](screenshots/model_accuracy.png)

### 3. Content-Based Recommendation System

A content-based recommendation system was developed to recommend Netflix titles with similar characteristics.

The system uses:

* Content type
* Rating
* Categories/genres
* Text preprocessing
* **TF-IDF vectorization**
* **Cosine similarity**

The system compares the feature representation of titles and returns recommendations with the highest similarity scores.

Example titles tested include:

* *The Starling*
* *Midnight Mass*
* *The Perks of Being a Wallflower*

The results demonstrated that the system could identify titles with similar content characteristics.

### 4. Machine Learning Classification

Machine learning models were trained to classify Netflix content as either **Movie** or **TV Show**.

#### Features

The classification models used:

* `release_year`
* `rating`

Categorical rating values were converted into numerical features using one-hot encoding.

#### Models

Two classification algorithms were evaluated:

| Model               |   Accuracy |
| ------------------- | ---------: |
| Logistic Regression | **70.65%** |
| Decision Tree       | **71.79%** |

The **Decision Tree** achieved the highest accuracy at **71.79%** and performed better at identifying TV Shows compared with Logistic Regression.

## Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**
* **Google Colab**
* **Jupyter Notebook**
* **GitHub**

## Project Structure

```text
auspify-netflix-data-science/
│
├── Auspify_Data_Science_Internship_Netflix_Analysis.ipynb
├── cleaned_dataset.csv
└── README.md
```

## Methodology

The project follows a practical Data Science workflow:

```text
Raw Dataset
     ↓
Data Cleaning & Preprocessing
     ↓
Exploratory Data Analysis
     ↓
Feature Engineering
     ↓
Recommendation System
     ↓
Machine Learning Classification
     ↓
Model Evaluation & Findings
```

## Key Learning Outcomes

Through this project, I gained practical experience in:

* Data cleaning and preprocessing with Pandas
* Handling missing and inconsistent data
* Exploratory Data Analysis
* Data visualization
* Feature engineering
* Text vectorization using TF-IDF
* Similarity analysis using cosine similarity
* Machine learning classification
* Model evaluation and comparison
* Organizing and documenting a Data Science project

## Dataset

The project uses a Netflix Movies and TV Shows dataset containing information such as titles, content type, directors, cast, countries, release years, ratings, durations, and categories.

The processed dataset included in this repository is the cleaned version used throughout the analysis.

## Internship

**Program:** Data Science Internship
**Organization:** Auspify Technologies
**Project:** Netflix Data Science Analysis

This repository contains the work completed for the selected internship tasks.

## Conclusion

This project demonstrates the application of practical Data Science techniques to a real-world-style entertainment dataset. The workflow covers data preprocessing, exploratory analysis, recommendation systems, and machine learning classification.

The project also demonstrates how analytical findings and machine learning results can be communicated through structured analysis, visualizations, and documented results.
