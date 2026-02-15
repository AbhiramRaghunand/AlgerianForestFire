# Algerian Forest Fire Prediction

## End-to-End Machine Learning Implementation

📌 Project Overview
  - This project implements a complete end-to-end Machine Learning pipeline to predict the likelihood of forest fires using the Algerian Forest Fire Dataset.
  - The system analyzes meteorological and environmental parameters such as temperature, humidity, wind speed, rainfall, and fire weather indices to classify whether a fire     will occur.
  - The objective is to demonstrate practical ML workflow implementation — from data preprocessing to model deployment.

📊 Dataset Information
  The dataset contains meteorological records collected from two regions of Algeria:
  
    - Bejaia region
    - Sidi Bel-Abbes region

🔎 Features Include:
    - Temperature
    
    - Relative Humidity (RH)
    
    - Wind Speed (Ws)
    
    - Rain
    
    - FFMC
    
    - DMC
    
    - DC
    
    - ISI
    
    - BUI
    
    - FWI
    
    - Class (Fire / Not Fire)

🧠 Machine Learning Pipeline
  
  This project covers the full ML lifecycle:
  
  1️. Data Cleaning
  
    - Handled missing values
  
    - Removed inconsistencies
    
    - Converted categorical labels
  
  2️. Exploratory Data Analysis (EDA)
    
    - Correlation analysis
    
    - Feature distribution visualization
    
    - Class imbalance analysis
  
  3️. Feature Engineering
    
    - Feature scaling (Standardization)
    
    - Label encoding
  
  4️. Model Training
    
    - Implemented and compared multiple models:
    
    - Linear Regression
    
    - Ridge Regression
    
    - Lasso Regression
  
  5️. Model Evaluation
    
    Evaluated using:
    
      - Mean Absolute Error
      
      - R2 Score
  
  6️. Deployment
    
    - Model saved using Pickle
    
    - Flask backend created for prediction API
    
    - User inputs environmental data
    
    - System returns Fire / Not Fire prediction

🏗 System Architecture

User Input → Data Preprocessing → Trained ML Model → Prediction Output

🛠 Tech Stack

  👨‍💻 Backend
  
    - Python
    
    - Flask

  📊 ML & Data Processing
    
    - Pandas
    
    - NumPy
    
    - Scikit-learn
    
    - Matplotlib
    
    - Seaborn
    
 🧰 Tools
    
    - Git
    
    - VS Code
    
    - Postman

🔍 Performance Comparison

      Model	            Mean Absolute Error (MAE)	  R² Score
      
      Linear Regression	    0.5170	                 0.9831
      
      Ridge Regression	    0.5293	                 0.9824
      
      Lasso Regression	    1.1258	                 0.9499
      
      Elastic Net	          1.7704	                 0.8888
      
🏆 Best Performing Model

    Linear Regression achieved the best performance, with:
    
    - Lowest MAE (0.5170)
    
    - Highest R² Score (0.9831)
    
    This indicates that the model explains approximately 98.3% of the variance in the target variable and has very low prediction error.


📊 Key Observations

  - Linear and Ridge regression performed similarly, indicating low multicollinearity impact.
  
  - Lasso and Elastic Net showed higher error, likely due to stronger regularization penalizing important features.
  
  - The dataset demonstrates strong linear relationships between features and target variable.
 
🎯 Conclusion

   The final deployed model was Ridge Regression, as it provided accurate and stable predictions.

🚀 How to Run

  - Clone the repository: 
    git clone https://github.com/yourusername/algerian-forest-fire.git
    
  - Navigate into project:
    cd algerian-forest-fire

  - Install dependencies:
    pip install -r requirements.txt
    
  - Run Flask app
    python app.py

🎯 Key Learnings
  
    - End-to-end ML workflow implementation
    
    - Importance of feature scaling
    
    - Model comparison and selection
    - Deployment of ML model using Flask
    - Handling real-world tabular datasets
