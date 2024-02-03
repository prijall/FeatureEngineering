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

    **Note:** Since, All other types aren't used as MInMax Scaling, I just focused on MinMaxScaler in practical Implementation. I will assure to do other in forthcoming future.

![code photo](Code_Snippet.png) 

![visual](MinMax_Matplot.png) ![Visual](MinMax_Seaborn.png)

# Day 4
Today, I learned the concept of Encoding which is widely used in categorical variables in classofication. We convert alphabetic value to numeric values in machine learning which helps model to perform better. There are Two kinds of Encoding, they are:
- Nominal Encoding
- Ordinal Encoding
 Today , I studied about Ordinal Encoding only. 
 ## Ordinal Encoding 
Ordinal Encoding are those encoding in which there is order in the different categorical values.
For example: If there are three categorizes i.e. 'Poor', 'Average' and 'Excellent' in grading system then the intuition is that "Excellent > Average > Poor". 
In this case, we will be using Ordinal Encoding.
**Note:** We can assign values in order in Ordinal Encoding i.e. {'Poor': 0, 'Average':1, 'Excellent':2}

![Code Photo](OrdinalEncodingPhoto-2-1-1.png)
![Result](NumericValue.png)

# Day 5
Today, I deep dive into the concept of One Hot Encoding which is very useful in machine learning. One Hot Encoding is used in Nominal dataset i.e. those dataset that has no order. For example; If we have 4 columns of colors that are Red, Blue, Green and Black then we use One Hot Encoding in this dataset as there is no order to any color. 

### Concept of Dummy Variable Trap
 When we do OneHotEncoding, we divide categories into different columns. But when all the columns are formed, we remove one column i.e if there are 'n' columns after categorical division then er make it 'n-1' to avoid **MultiColinearity**. 

### OHE using Frequent Variables
When Separating categories, there may be as many columns due to which it becomes difficult to handle and manage data due to which this concept is introduce that if we have many categories then we will make columns of only those which have more frequency and we make common columns for rest of the categories which makes our data more clean. The assumption here is that the categories in common column should be in less frequency.

![code](OHE_photo.png)