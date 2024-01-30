![Feature Engineering](<feature engineering.png>)

# Day 1
  Today, I started learning Feature engineering which is very important in machine learning. According to Wikipedia, Feature Engineering is the process of using domain knowledge to extract features from any raw data.
  There are 4 kinds in feature engineering, they are;

## Feature Transformation
   There are mainly four types of feature transformation;
- Missing value Imputation
- Handling Categorical Features
- Outlier Detection
- Feature Scaling

## Feature Construction
   Sometimes, we need to construct features manually in dataset to make our data more cleaner and effective to use for machine learning algorithms.

## Feature Selection 
   It is one of the important part of feature engineering as it helps us to focus on real data. For example, while working in MNIST dataset, we only need to use the column that has figure and discard that are empty.

## Feature Extaction
   It helps to reduce the no of independent variables and makes our machine learning model more efficient.
   
![photo](F_Engineering.png)


# Day 2
  There are basically two types of feature scaling and they are: **Standardization** and **Normalization** .Today, I learned the concept of Standardization in feature scaling which is very important in machine learning. Standardization is the process of standardizing the values so that they wont create imbalance and biased dataset during development of machine learning models. This is also very important to those algorithms which uses Euclidean distance. Standardization is also called **Z-Score Normalization**.
   The formula that is used to get Standardization is Actual value subtracted to Mean value which is divided by Standard Deviation i.e.
  
   - Standardization = (Actual Value)- (Mean Value)/(Standard Deviation)

   ![Code Photo](Standardization_code_png.png) 
   
   ![Graph Photo](StandardizedGraph.png)