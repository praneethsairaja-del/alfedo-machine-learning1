

Iris Species Classification Model
This project focuses on predicting the species of an Iris flower based on its sepal and petal measurements. It uses the classic Iris Dataset to train and evaluate multiple Machine Learning classification models.  
IPYNB
+ 1

## Project Overview
The notebook demonstrates an end-to-end data science workflow, including:  
IPYNB

Environment Setup: Installing and importing the necessary data science libraries.  
IPYNB

Data Loading & Exploration: Loading the dataset and examining its structure.  
IPYNB

Data Quality Checks: Verifying the data type and checking for missing values.  
IPYNB

Data Visualization: Plotting the relationships between various features.  
IPYNB

Model Training & Evaluation: Setting up multiple scikit-learn classifiers (such as KNN, Logistic Regression, and Decision Trees) to compare their predictive performance.  
IPYNB

### Prerequisites & Installation
To run the notebook successfully, you will need Python along with several standard data science packages. You can install all dependencies directly within the notebook or via your terminal:  
IPYNB
+ 1

Bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
### Dataset Structure
The notebook loads a local dataset named IRIS.csv. The dataset contains 150 observations with no missing values and consists of 5 columns:  
IPYNB
+ 1

Column Name	Data Type	Description
sepal_length	float64	
Length of the sepal in cm  
IPYNB

sepal_width	float64	
Width of the sepal in cm  
IPYNB

petal_length	float64	
Length of the petal in cm  
IPYNB

petal_width	float64	
Width of the petal in cm  
IPYNB

species	object	
Target class (e.g., Iris-setosa, Iris-versicolor, Iris-virginica)  
IPYNB

### Notebook Workflow
1. Library Imports
The project utilizes standard tools for analysis, visualization, and modeling:  
IPYNB

Data Manipulation: pandas, numpy

  
IPYNB

Visualization: matplotlib.pyplot, seaborn

  
IPYNB

Machine Learning: scikit-learn (train_test_split, KNeighborsClassifier, LogisticRegression, DecisionTreeClassifier)  
IPYNB

Model Serialization: joblib (for saving the trained model)  
IPYNB

2. Data Cleaning
Executes df.info() to verify 150 non-null rows.  
IPYNB

Runs df.isnull().sum() to confirm that the dataset requires no missing-value imputation.  
IPYNB

3. Exploratory Data Analysis (EDA)
Generates pair plots and feature correlation graphs using seaborn to understand how the target species cluster based on petal and sepal dimensions.  
IPYNB

4. Machine Learning Modeling
The notebook prepares the data for classification by splitting it into training and testing sets, then evaluates the following algorithms using accuracy scores, confusion matrices, and classification reports:  
IPYNB

K-Nearest Neighbors (KNN)

  
IPYNB

Logistic Regression

  
IPYNB

Decision Tree Classifier

  
IPYNB

### How to Use
Clone your project directory and place the IRIS.csv file in your specified local path.  
IPYNB

Open the .ipynb file in Jupyter Notebook or VS Code.  
IPYNB

Update the file path in the data loading cell if your IRIS.csv is stored in a different folder:  
IPYNB

Python
df = pd.read_csv('your_relative_or_absolute_path/IRIS.csv')

