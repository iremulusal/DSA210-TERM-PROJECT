# **DSA210-TERM PROJECT**

## **Project Overview**
Over the next three months, I will systematically examine how daily habits including total caloric intake, macronutrient distribution (protein, carbohydrates, and fats), sleep duration, and exercise time affect my body composition, specifically focusing on changes in body fat percentage and overall weight. The ultimate goal is to identify and quantify which habits play the most pivotal role in shaping my physical outcomes, while also gaining deeper insight into how my body responds to these factors, thereby streamlining my weight loss and fat reduction journey.

## **Objectives**
1. **Identify Key Influencing Factors**  
   - Determine which daily habits (e.g., calorie intake, macronutrient ratios, sleep duration, exercise time) most significantly drive reductions in body weight and body fat percentage.  

2. **Develop Data-Driven Strategies**  
   - Use the findings to create or refine daily habits (e.g., adjusting protein intake, prioritizing sleep quality, or increasing exercise duration) to achieve measurable health and fitness improvements.  

3. **Apply Data Science Concepts**  
   - Implement Python-based tools for data cleaning, exploratory data analysis (EDA), and advanced techniques such as regression modeling or time-series analysis in accordance with the DSA210 course requirements.  

4. **Long-Term Practical Application**  
   - Translate data-driven insights into actionable and sustainable habits that continue to promote healthy weight management beyond the study period.  

## **Motivation**
- **Personal Goals**  
  Focus on reducing overall weight and body fat while examining how each lifestyle factor (e.g., calorie intake, sleep quality, exercise time) uniquely affects my body, enabling a more targeted and efficient weight-loss strategy.  

- **Real World Data Application**  
  Gain hands-on experience in collecting, cleaning, and analyzing personal health data using Python and related libraries, bridging theory with everyday practice.  

- **Skill Integration & Enhancement**  
  Develop practical proficiency in data visualization, model evaluation, and decision-making processes that directly inform effective weight loss strategies, thereby enriching both personal and professional growth.  

## **Dataset**
The dataset will consist of three months of daily records, each including the following variables:

- **Date**: The specific day of each record.  
- **Total Calories (kcal)**: Daily caloric intake.  
- **Macronutrients (g)**:  
  - Protein  
  - Carbohydrates  
  - Fats  
- **Water Intake (L)**: Daily water intake.  
- **Body Fat Percentage (%)**: Daily measurement to track fat loss.  
- **Body Weight (kg)**: Daily measurement to monitor overall weight changes.  
- **Sleep Duration (hours)**: Total hours of sleep each night.  
- **Sleep Quality (1–5)**: Self-rated measure of sleep quality.  
- **Exercise Time (minutes)**: Duration of physical activity, including fitness and pilates.  
- **Calorie Deficit (kcal)**: Computed as 2300 – (Daily Caloric Intake – Calories Burned during Exercise).  
  - Here, 2300 kcal represents the estimated daily maintenance calorie requirement determined using the Mifflin-St Jeor formula.  

All data will be logged daily at the same time in an Excel file. Any outliers resulting from unusual circumstances such as illness, injuries, or deviations from routine will be flagged for further review during analysis.  

## **Analysis Plan**
### **1. Data Collection & Preprocessing**
- **Import & Consolidation**: Load the three-month daily Excel log into a Pandas Data Frame.  
- **Cleaning**:  
  - Address missing or inconsistent values.  
  - Standardize units (calories in kcal, macronutrients in grams, weight in kg).  
  - Convert date columns to a consistent datetime format.  
- **Minimal Feature Engineering**:  
  - Compute daily changes in body weight and fat percentage.  
  - Categorize sleep quality and exercise time into defined groups (e.g., low, moderate, high) as needed.  
  - Calculate the "Calorie Deficit" using the formula: 2300 - (Daily Caloric Intake - Calories Burned during Exercise).  

### **2. Exploratory Data Analysis (EDA)**
#### **Descriptive Analysis**
- Calculate key statistics (mean, median, standard deviation) for total calories, macronutrients, water intake, sleep metrics, exercise time, weight, and fat percentage.  

#### **Visualization**
- Use histograms and density plots to examine the distribution of individual variables.  
- Generate time series plots to observe trends in body weight and fat percentage over the three months.  
- Create a correlation heatmap to visualize relationships among daily calories, macronutrient ratios, sleep, exercise, weight, and fat percentage.  
- Employ scatter and box plots to explore bivariate relationships, such as between protein intake and fat percentage or sleep quality and weight changes.  

## **Hypothesis Testing**
### **1) Total Caloric Intake & Body Weight**
- **H₀**: Total daily caloric intake has no significant relationship with overall body weight.  
- **H₁**: Higher total caloric intake is significantly associated with increased body weight.  
- **Approach**: Use correlation analysis and regression modeling to evaluate the relationship.  

### **2) Caloric Deficit & Fat Percentage Reduction**
- **H₀**: A daily caloric deficit does not significantly influence reductions in body fat percentage.  
- **H₁**: Consistent caloric deficits are significantly associated with reductions in body fat percentage.  
- **Approach**: Compare days with deficits versus surpluses using t-tests and regression.  

### **3) Protein Intake & Fat Loss**
- **H₀**: The proportion of protein intake (relative to total calories) has no significant effect on body fat percentage reduction.  
- **H₁**: A higher proportion of protein intake is significantly associated with greater reductions in body fat percentage.  
- **Approach**: Use multiple regression analysis while controlling for total caloric intake.  

### **4) Sleep Duration & Quality vs. Body Composition**
- **H₀**: Sleep duration and sleep quality have no significant influence on overall body weight or body fat percentage.  
- **H₁**: Longer sleep duration is significantly associated with lower overall body weight, and better sleep quality is significantly associated with greater reductions in body fat percentage.  
- **Approach**:  
  - Analyze correlations and perform regression between sleep duration and weight changes.  
  - Compare groups based on sleep quality ratings using t-tests to evaluate differences in body fat percentage.  

## **Conclusion**
This project aims to provide clear, data-driven answers to the following key questions:

- **Which daily habits most significantly influence body weight and body fat percentage?**  
  Identify the impact of total calories, macronutrient ratios, sleep duration/quality, and exercise time on body composition.  

- **How do nutritional intake and lifestyle factors interact?**  
  Explore whether factors such as protein intake and exercise have synergistic effects on reducing body fat.  

- **Can targeted adjustments lead to measurable improvements?**  
  Evaluate if improvements in specific areas like increased protein, better sleep, or extended exercise time result in greater fat loss and weight reduction.  

- **What actionable insights can guide sustainable weight management?**  
  Translate statistical findings into practical, long term strategies for effective weight and fat reduction.  

By addressing these questions, the project will not only enhance our understanding of how daily habits shape physical outcomes but also provide a scalable framework for making informed, sustainable lifestyle changes.

