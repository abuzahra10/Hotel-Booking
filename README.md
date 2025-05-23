# 🚖 NYC Taxi Trip Tip Prediction using Apache Spark

This project utilizes Apache Spark and MLlib to analyze NYC taxi trip data and build a predictive model to estimate taxi tips based on trip and fare features.

> Developed as part of **Big Data & NoSQL Databases – Spring 2025** at the German International University.

---

## 📊 Objective

To preprocess a large-scale NYC taxi dataset, perform exploratory data analysis, and train a machine learning model to predict the **tip amount** using features like trip distance, fare, payment type, and pickup/dropoff locations.

---

## 🔍 Dataset

- **Source:** NYC TLC Trip Record Data  
- **Files Used:**
  - `taxi_trip_data.csv`: Includes trip/fare details
  - `taxi_zone_geo.csv`: Mapping for pickup/dropoff zones

### Key Features:

| Column              | Description                           |
|---------------------|---------------------------------------|
| pickup_datetime     | Timestamp when the trip began         |
| dropoff_datetime    | Timestamp when the trip ended         |
| trip_distance       | Total distance of the trip            |
| fare_amount         | Base fare for the trip                |
| tip_amount          | Tip given by passenger                |
| payment_type        | Payment method (cash, credit, etc.)   |
| PULocationID        | Pickup zone ID                        |
| DOLocationID        | Dropoff zone ID                       |

---

## 🛠️ Tools & Technologies

- **Apache Spark**
- **PySpark**
- **Spark SQL / DataFrame API**
- **Spark MLlib**
- **Python**
- **Jupyter Notebook**

---

## 📈 Workflow

1. **Data Ingestion**
   - Load raw CSV files into Spark DataFrames
   - Clean nulls, drop invalid trips

2. **Feature Engineering**
   - Calculate trip duration
   - Extract time-based features
   - Map zones using `taxi_zone_geo.csv`

3. **Exploratory Data Analysis**
   - Visualize correlations between tips and features
   - Detect outliers and skewed distributions

4. **Modeling (Tip Prediction)**
   - Use Spark ML pipelines
   - Train/test split
   - Feature assembler + VectorIndexer
   - Algorithms: Linear Regression, Random Forest Regressor

5. **Evaluation**
   - Metrics: RMSE, MAE, R²
   - Feature importance analysis

---


