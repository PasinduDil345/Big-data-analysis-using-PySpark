# PySpark Social Media Engagement Analysis 📊

This project demonstrates the use of PySpark to analyze a social media engagement dataset. The notebook explores various data manipulation and analysis techniques available in the Spark ecosystem to process data and extract meaningful insights.

## 📋 Project Overview

The main goal of this project is to perform an exploratory data analysis (EDA) on social media data. It showcases fundamental PySpark operations, including:
* Loading data into a Spark DataFrame.
* Performing data transformations and aggregations.
* Joining different datasets.
* Visualizing results to understand data distributions.

## 💾 Dataset

The analysis is performed on the `social_media_engagement.csv` dataset. Key columns in this dataset include:
* `platform` (e.g., Facebook, Instagram, Twitter)
* `post_type` (e.g., image, video, poll)
* `likes`, `comments`, `shares`
* `sentiment_score` (e.g., positive, neutral, negative)

## 🛠️ Technologies Used

* **Python**
* **Apache Spark (PySpark)**
* **Pandas** (for converting Spark DataFrame for visualization)
* **Matplotlib & Seaborn** (for plotting)


## ✨ Features & Analysis Performed

* **Data Loading and Schema Inspection**: The dataset is loaded into a Spark DataFrame, and its schema is programmatically inspected.
* **Data Selection & Filtering**: The notebook demonstrates how to select specific columns and filter rows based on conditions (e.g., posts with more than 500 likes).
* **Aggregation**: `groupBy()` is used to perform aggregations and calculate key metrics, such as the average and maximum number of likes for each social media platform.
* **Joins**: Two separate DataFrames are created and then joined on a common key (`post_id`) to demonstrate join operations.
* **Feature Engineering**: A new column (`double_likes`) is created using the `withColumn()` function to showcase data transformation.
* **Data Visualization**: The distribution of 'likes' is visualized using a histogram after converting a subset of the Spark DataFrame to a Pandas DataFrame.
