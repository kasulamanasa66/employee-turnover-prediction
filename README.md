# employee-turnover-prediction
Machine Learning project to predict employee attrition using classification algorithms and HR analytics data.


Project Overview

    Employee turnover is a major challenge for organizations. This project aims to predict employee attrition and uncover the key factors influencing employees to     leave, while also providing data-driven retention strategies.

The solution combines:

  Handling Imbalacing using SMOTE Technique
  
  Machine Learning (classification)
  
  Clustering (employee segmentation)
  
  Business insights for HR decision-making

Objectives

    Predict whether an employee will leave the company
    
    Identify key factors contributing to attrition
    
    Handle class imbalance effectively
    
    Compare multiple machine learning models
    
    Segment employees who left using clustering
    
    Recommend targeted retention strategies

Dataset
    HR Analytics dataset
    
        Contains features like:
        
            Satisfaction level
            
            Last evaluation
            
            Number of projects
            
            Average monthly hours
            
            Time spent in company
            
            Promotion history
            
            Salary level
            
            Department

Tech Stack

    Python
    
    Pandas, NumPy
    
    Matplotlib, Seaborn
    
    Scikit-learn
    
    XGBoost
    
    Imbalanced-learn (SMOTE)

Exploratory Data Analysis (EDA)

    Key insights discovered:
    
        Employees with low satisfaction are more likely to leave
        
        High working hours indicate burnout → higher attrition
        
        Employees with no promotion in last 5 years tend to leave
        
        Both low performers and high performers can leave (different reasons)


Visualizations
🔹 Correlation Heatmap

        ![HeatMap](images/heatmap.png)

    Finding the number of clusters using Elbow Method:
        ![Elbow](images/Elbow_Graph.png)

   Clustering Visulaization:
         ![ScatterPlot](images/Clusters.png)
         


  Purpose:

    Understand feature relationships
    
    Identify important variables influencing attrition


Data Preprocessing

  Removed duplicate records
  
  One-hot encoded categorical variables (salary, department)
  
  Train-test split
  
  Handled class imbalance using SMOTE


Machine Learning Models

    The following models were trained and evaluated:
    
       1)Logistic Regression
       
       2)Naive Bayes
       
       3)K-Nearest Neighbors (KNN)
       
       4)Support Vector Machine (SVM)
       
       5)Decision Tree
       
       6)Random Forest
       
       7)AdaBoost
       
       8)Gradient Boosting
       
       9)XGBoost

Model Evaluation

    Used 5-Fold Cross Validation
    
    Evaluation Metric: F1-Score (due to class imbalance)

                        | Classification Model       | F1-Score          | 
                        | -----------------          | ------------ -----| 
                        | Logistic Regression        | 0.8425216686188239|       
                        | Naive Bayes | 0.5721       | 0.760508887050977 |
                        | K-Nearest Neighbours(KNN)  | 0.9551733662607429|      
                        | Support Vector Machine SVM)| 0.9583910497635838|      
                        | Decision Tree              | 0.9587162711018923|       
                        | Random Forest              | 0.977622849973565 |     
                        | AdaBoost                   | 0.9271460149997945|
                        | Gradient Boosting          | 0.971988849207932 |
                        | XGboost                    | 0.9806758565708419|

   
        
    👉 Ensemble models like Random Forest, Gradient Boosting, and XGBoost performed best.

Clustering Analysis

    Performed KMeans clustering on employees who left to identify behavioral patterns.

    Identified Segments:
    
    🔴 Disengaged Employees (Low satisfaction, low performance)
    
    🟡 High-performing but dissatisfied employees 
    
    🟢 Moderately engaged employees

Retention Strategies


   * Improve engagement for low-satisfaction employees
     
   * Reward and promote high performers
    
   * Strengthen employee involvement programs
    
   * Reduce excessive workload (burnout prevention)
    
   * Provide career growth opportunities
    
    *Improve compensation structure
    
    
Key Takeaways

    *Attrition is driven by multiple factors, not just performance
    
    *Combining ML + clustering provides deeper insights
    
    *Data-driven HR strategies can significantly reduce employee turnover

