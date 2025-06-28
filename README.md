# 🛒 Product Recommendation Engine

This repository contains a collaborative filtering-based recommendation system built on Apache Spark using the Amazon Product Reviews Dataset. The project is designed to provide personalized product recommendations using Alternating Least Squares (ALS) and optimized for large-scale data with Delta Lake.

## 📌 Overview

This engine is developed as an individual project to build a scalable and efficient recommendation system leveraging real-world customer review data from Amazon.

## 🧠 Problem Statement

Customers often struggle to find relevant products due to the overwhelming variety. This recommendation engine aims to:

- Suggest relevant products using collaborative filtering.
- Process millions of reviews efficiently.
- Handle real-time or incremental updates.
- Improve accuracy through model optimization.

## 📂 Dataset

- **Source:** Kaggle [https://www.kaggle.com/datasets/arhamrumi/amazon-product-reviews]
- **Name:** Amazon Product Reviews Dataset
- **Fields:**
  - `ProductID`
  - `UserID`
  - `Rating`
  - `ReviewText`
  - `Timestamp`

## 🚀 Project Objectives

- Clean and preprocess large-scale review data.
- Build a user-item interaction matrix.
- Implement and optimize the ALS collaborative filtering model.
- Enable scalable training and inference using Spark and Delta Lake.
- Measure performance improvements with RMSE and data optimization techniques.

## 🔧 Tech Stack

- Apache Spark with PySpark
- Databricks
- Delta Lake
- ALS (Alternating Least Squares)
- RMSE Evaluation
- Z-Ordering & Vacuum for optimization

## 📊 Pipeline Tasks

### 1. Data Preprocessing
- Convert and clean timestamps
- Remove null and irrelevant columns
- Deduplicate data

### 2. Exploratory Data Analysis
- Identify top reviewers, trending products, and review distributions
- Understand product and user-level engagement

### 3. ALS Model Building
- Build user-item matrix
- Train initial ALS model
- Evaluate with RMSE

### 4. Optimization
- Hyperparameter tuning via cross-validation
- Use Delta Lake for incremental updates
- Apply Z-Ordering and Vacuum for performance

### 5. Final Model
- Achieved RMSE: **0.26**

## ✅ Results

| Stage            | RMSE   |
|------------------|--------|
| Initial Model    | 2.30   |
| After Tuning     | 1.17   |
| Final Optimized  | 0.26   |

## 🧪 How to Use

1. Clone this repository.
2. Import the provided `.dbc` notebook into your Databricks workspace.
3. Attach to a cluster and run the notebook cells in order.
4. (Optional) Upload your own reviews dataset for testing.

## 👨‍💻 Author

Developed by **Vasu Arora**  

