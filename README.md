# 📊 DSA210 Term Project: Data-Driven Weight & Fat Loss Analysis

## Project Overview  
Over the next three months, I will systematically examine how daily habits—including total caloric intake, macronutrient distribution (protein, carbohydrates, and fats), sleep duration, and exercise time—affect my body composition. The primary focus will be on **body fat percentage reduction** and **overall weight changes**.  

The goal is to **identify and quantify** which habits play the most pivotal role in shaping my physical outcomes while streamlining my weight loss and fat reduction strategy.

---

## Objectives  

### 1️⃣ Identify Key Influencing Factors  
- Determine which daily habits (e.g., calorie intake, macronutrient ratios, sleep duration, exercise time) most significantly impact weight and body fat percentage.  

### 2️⃣ Develop Data-Driven Strategies  
- Use the findings to **adjust daily habits**, such as modifying protein intake, prioritizing sleep quality, or increasing exercise duration to optimize fitness results.  

### 3️⃣ Apply Data Science Concepts  
- Implement **Python-based data analysis** tools, including:  
  - Data cleaning  
  - Exploratory Data Analysis (EDA)  
  - Regression modeling & time-series analysis (as per DSA210 course requirements)  

### 4️⃣ Long-Term Practical Application  
- Translate **data-driven insights** into **sustainable** and actionable habits for long-term weight management.  

---

## Motivation  

### Personal Goals  
- Optimize weight loss by analyzing how **calories, sleep, and exercise** impact body fat percentage.  
- Develop a **more effective, targeted weight-loss strategy** based on data-driven insights.  

### Real-World Data Application  
- Gain hands-on experience in **data collection, cleaning, and analysis** using Python.  
- Apply theoretical concepts to **real-life fitness tracking**.  

### Skill Integration & Enhancement  
- Strengthen expertise in:  
  - **Data visualization** (histograms, scatter plots, heatmaps)  
  - **Model evaluation** (correlation, regression)  
  - **Decision-making** based on statistical analysis  

---

##Dataset  

The dataset will contain **three months of daily records**, stored in an **Excel file**, including:  

### **Recorded Features**  
| Feature | Description |
|---------|-------------|
| **Date** | Specific day of each record |
| **Total Calories (kcal)** | Daily caloric intake |
| **Macronutrients (g)** | Protein, Carbohydrates, Fats |
| **Water Intake (L)** | Daily water consumption |
| **Body Fat Percentage (%)** | Measurement of fat loss |
| **Body Weight (kg)** | Tracking overall weight changes |
| **Sleep Duration (hours)** | Total sleep time each night |
| **Sleep Quality (1–5)** | Self-rated sleep quality |
| **Exercise Time (minutes)** | Duration of physical activity (gym, Pilates, etc.) |
| **Calorie Deficit (kcal)** | Computed as: `2300 - (Daily Caloric Intake - Calories Burned)` |

**Note:** Any **outliers** (due to illness, injuries, or deviations from routine) will be flagged and reviewed before analysis.  

---

##Analysis Plan  

### **Data Collection & Preprocessing**  
-  **Import & Consolidation**: Load daily records into a **Pandas DataFrame**.  
-  **Data Cleaning**:  
  - Handle missing/inconsistent values  
  - Standardize units (calories in kcal, macronutrients in grams, weight in kg)  
  - Convert date columns to `datetime` format  
-  **Feature Engineering**:  
  - Compute **daily changes in body weight & fat percentage**  
  - Categorize **sleep quality** and **exercise time** into groups (low, moderate, high)  
  - Calculate **calorie deficit**  

###  **Exp
