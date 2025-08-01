🚢 Titanic Survival Prediction  
This project uses Decision Tree and Random Forest models to predict whether a passenger survived the Titanic disaster. Based on demographic and fare data, we explore how passenger class, sex, age, family size, and ticket price influence survival.

📁 Dataset  
Source: Titanic.csv  
Imported From: Local machine or Google Colab  
Expected Columns:  
- Pclass (Passenger class)  
- Male (1 = male, 0 = female)  
- Age  
- SibSp (Siblings/Spouses aboard)  
- Parch (Parents/Children aboard)  
- Fare  
- Survived (Target variable: 0 = No, 1 = Yes)  

🧼 Data Preparation  
- Assumed dataset has no missing values (e.g., Age should be filled in if null)  
- Categorical variable 'Sex' was encoded as binary 'Male'  
- No additional feature engineering applied  

🧠 Models Used  
🌳 Decision Tree Classifier (Entropy criterion)  
- Model 1: max_depth=10  
- Model 2: max_depth=100  
- Evaluated accuracy on both training and test sets  
- Saved plots as `treeplot.png` and `treeplot2.png`  

🌲 Random Forest Classifier  
- n_estimators=10  
- Evaluated accuracy on test set  

📈 Evaluation Metrics  
- Accuracy Score for all models  
- Example output:


Accuracy of train dataset (max_depth=10): 0.9238
Accuracy of test dataset (max_depth=10): 0.7674

Accuracy of train dataset (max_depth=100): 0.976
Accuracy of test dataset (max_depth=100): 0.772

Random Forest Accuracy: 0.76

🖼️ Visuals  
- Full decision tree plots for both tree depths  
- Saved as PNG files for easy inspection  

📦 Packages Used  
- pandas: Data manipulation  
- scikit-learn: Modeling (DecisionTree, RandomForest, accuracy metrics)  
- matplotlib: Tree plotting  
- Google Colab: File upload support (optional)  

🔧 How to Run  
1. Ensure Titanic.csv is in the working directory  
2. Run script in Python (Google Colab or local IDE)  
3. View output in console and saved tree images  
