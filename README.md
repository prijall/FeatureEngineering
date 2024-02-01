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
   
   ![Graph Photo](StandardizedGraph-1.png)


# Day 3
  After learning the basic concpets of Standaradization, today i studied about Normalization in feature scaling. **Normalization** is a technique often applied with goal to change the values of numeric columns in the dataste to use a common scale, without distorting differences in the ranges of values or losing informations.There are various types of Normalization, they are;
  - MinMax Scaling
  - Mean Normalization
  - Max Absolute 
  - Robust Scaling

  ## MinMax Scaling 
     The formula for MinMax Scaling is:
         X'= (X-Xmin)/(Xmax-Xmin)
         
      The range of new distribution will be in [0, 1]. In 2D graph, it means squashing all the datas into unit square and In 3D graph, it is cubic.

  ## Mean Normalization
   The formula of Mean Normalization is:
     X'= (X-Xmean)/(Xmax-Xmin)

    It is generally mean centering like that of Standaradization.

    **Note:** Since, All other types aren't used as MInMax Scaling, I just focused on MinMaxScaler in practical Implementation. I will assure to do other in coming future.

![code photo](Code_Snippet.png) 

![visual](MinMax_Matplot.png) ![Visual](MinMax_Seaborn.png)