# Uber-Data-Analysis
Exploratory Data Analysis of Uber ride requests using Python, Pandas, NumPy, Matplotlib and Seaborn.

# 🚕 Uber Data Analysis

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on Uber ride request data to understand ride demand patterns, trip statuses, pickup locations, and time-based trends.

The analysis focuses on identifying patterns in completed trips, driver cancellations, and cases where no cars were available. The project was developed as a hands-on implementation during a data analytics workshop.

---

## 🎯 Objectives

The main objectives of this project are:

- Analyze Uber ride request data using Python.
- Understand the distribution of different ride statuses.
- Identify the number of ride requests across different hours of the day.
- Analyze ride status based on pickup location.
- Identify time periods with higher cancellations or unavailable cars.
- Understand potential demand and supply-related patterns.

---

## 📊 Dataset

The dataset contains **6,745 Uber ride requests** with the following attributes:

| Column | Description |
|--------|-------------|
| `Request id` | Unique identifier for each ride request |
| `Pickup point` | Pickup location of the ride (City/Airport) |
| `Driver id` | Identifier of the assigned driver |
| `Status` | Status of the ride request |
| `Request timestamp` | Date and time when the ride was requested |
| `Drop timestamp` | Date and time when the ride was completed/dropped |

### Ride Status Distribution

The dataset contains three ride statuses:

- **Trip Completed:** 2,831
- **No Cars Available:** 2,650
- **Cancelled:** 1,264

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab / Jupyter Notebook

---

## 🔍 Analysis Performed

### 1. Data Loading and Inspection

The dataset was loaded using Pandas and examined using:

- `head()`
- `shape`
- `info()`
- `value_counts()`

### 2. Data Preprocessing

The request and drop timestamps were converted into datetime format.

A new feature called `RequestHour` was created from the request timestamp to analyze ride demand by hour.

### 3. Ride Status Analysis

The distribution of:

- Trip Completed
- Cancelled
- No Cars Available

was analyzed to understand the overall outcome of ride requests.

### 4. Hourly Ride Demand

The number of ride requests was analyzed across different hours of the day to identify periods of higher ride demand.

### 5. Pickup Point Analysis

Ride requests were analyzed based on two pickup locations:

- City
- Airport

The relationship between pickup point and ride status was visualized.

### 6. Hourly Status Analysis

Ride status was analyzed across different hours using grouped and stacked bar charts.

Separate analyses were also performed for:

- City pickups
- Airport pickups

---

## 📈 Visualizations

The project includes visualizations such as:

- Number of rides requested per hour
- Ride status distribution by pickup point
- Trip status distribution by hour
- City pickup status distribution by hour
- Airport pickup status distribution by hour

---

## 💡 Key Insights

The analysis helps identify:

- The overall distribution of completed, cancelled, and unavailable rides.
- Hours with higher numbers of ride requests.
- Differences in ride outcomes between City and Airport pickup points.
- Time periods where cancellations and unavailable cars become more prominent.
- Potential demand and supply gaps that can be further investigated.
