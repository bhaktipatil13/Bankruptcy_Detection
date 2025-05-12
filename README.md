# Bankruptcy_Detection

The objective of this project is to develop a classification model that predicts the likelihood of a company going bankrupt based on key financial and operational risk factors.

By analyzing features such as industrial risk, management risk, financial flexibility, credibility, competitiveness, and operating risk, the model aims to identify patterns and warning signs associated with financial distress.

The insights derived from this analysis can assist businesses, investors, and financial institutions in making informed decisions to mitigate risks and improve financial stability.

## 📊 Problem Statement

The objective is to build a binary classification model that predicts whether a company is likely to go bankrupt based on features like:
- Industrial Risk
- Management Risk
- Financial Flexibility
- Credibility
- Competitiveness
- Operating Risk

## 📁 Dataset

This dataset contains information on various risk factors, such as industrial, management, and operating risks, along with other characteristics that influence a company's performance during stressful situations.

### Features:
- `IR` - Industrial Risk  
- `MR` - Management Risk  
- `FF` - Financial Flexibility  
- `CR` - Credibility  
- `CO` - Competitiveness  
- `OR` - Operating Risk  
- `D` - Target variable (1: Bankrupt, 0: Non-Bankrupt)

## 🛠️ Project Workflow

1. **Data Loading & Exploration**
    -Used exploration techniques to
   1.understand shape and size of the dataset, checked missing , null duplicated values by doing basic analysis
   2.Data typs overview
   3.Vizualizations to understand the distrribution of variables

   **Conclusion**
   Our exploratory data analysis (EDA) revealed key patterns in the dataset, highlighting how different risk factors influence
   the classification outcome. it is observed that some features, such as **financial flexibility and competitiveness**, show strong
   separation between classes, while others, like **industrial risk and management risk**, exhibit more gradual changes in class proportions.
   The dataset also presents potential class imbalances and correlations among certain risk factors, which need to be carefully addressed.  

2. **Data Preprocessing**  
   -This section outlines the key preprocessing steps applied to the dataset before model training. The data is first split into features (X)
   and target labels (y), with categorical variables encoded using ordinal encoding. A structured 70-15-15 split is used to separate training,
   validation, and test sets.

   -During model development, we will experiment with removing duplicates and applying SMOTE to address class imbalance, assessing their impact on
   model performance. The training set undergoes feature selection, while the validation and test sets receive the same transformations to ensure consistency. 
   These preprocessing steps establish a solid foundation for effective model building and evaluation.

   -Used ordinal encoding for the categorical variables and did PCA vizualization to reduce dimentionallity and determine optimal number of components by doing
   feature selection.

4. **Model Building**  
   Trained and evaluated below five models using a train-validation-test split:  

   1. Logistic Regression 
   2. Decision Tree  
   3.Random Forest & Naive Byas   
   4.Gradient Boosting (XGBoost)
   5.Neural Networks   


5. **Model Evaluation**
   Used below steps to evaluate the model

 1. Train-Validation-Test Split  
   - Train models on training data and evaluate on the validation set.  
   - Tune hyperparameters using GridSearchCV on the validation set.  
   - Train the best configuration on the full training set.  

2. Test Set Evaluation  
   - Evaluate final models on the test set.  
   - Compare accuracy scores and confusion matrices.  
   - Identify overfitting/underfitting trends.  

3. Select Best Model & Improve* 
   - Apply k-fold cross-validation to handle overfitting.    
   - Train on the full dataset and report final accuracy and confusion matrix.  
  
   Evaluated using:
   - Accuracy Score
   - Confusion Matrix
   - Classification Report
   - ROC-AUC Curve

7. **Insights**  
   - Visualizations of performance.
   - Model comparison based on metrics.


## 👩‍💻 Authors

- **Bhakti Patil**  
  

