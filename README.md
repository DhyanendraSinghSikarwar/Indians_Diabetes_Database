# Pima_Indians_Diabetes_Database
This is the code "To analyze & check dependencies between features" on Diabetes dataset (offered by Kaggle.com) by Dhyanendra Singh.
## Context

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to analyze the features and check the dependencies of features. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.


## Diabetes
Diabetes is a disease that occurs when your blood glucose, 
also called blood sugar, is too high. Blood glucose is your main
 source of energy and comes from the food you eat. Insulin, 
a hormone made by the pancreas, helps glucose from food get
 into your cells to be used for energy.

## Different parameters Descriptions:

### BMI:
BMI is a person’s weight in kilograms divided by the square of
 height in meters. A high BMI can indicate high body fatness.

### Glucose:
A blood sugar level less than 140 mg/dL (7.8 mmol/L) is 
considered normal.A blood sugar level from 140 to 199 mg/dL 
(7.8 to 11.0 mmol/L) is considered prediabetes. This is sometimes
 referred to as impaired glucose tolerance. A blood sugar level 
 of 200 mg/dL (11.1 mmol/L) or higher indicates type 2 diabetes.

### Insulin:
Insulin is a hormone (a chemical substance that acts 
as a messenger in the human body) that is secreted by an
 abdominal organ called the pancreas. It controls the breakdown 
 of carbohydrates, fats and proteins in the body. It also guides
  the liver and muscles to store glucose and fat that can be 
  used during periods of increased energy requirements and
   fasting. Insulin is a “key” that unlocks the cell gates 
   so that glucose from the blood enters the cells. The cells
    of the muscle and fat tissue are dependent solely on
     insulin for glucose uptake and use.

### Pregnancies:
Diabetes can cause problems during pregnancy for women and 
their developing babies. Poor control of diabetes during 
pregnancy increases the chances for birth defects and other 
problems for the pregnancy. It can also cause serious 
complications for the woman. Proper health care before and
 during pregnancy can help prevent birth defects and other 
 health problems.

### Skin Thickness:
Skin thickness is primarily determined by collagen content and 
is increased in insulin-dependent diabetes mellitus (IDDM). We
 measured skin thickness in 66 IDDM patients aged 24–38 yr and
  investigated whether it correlated with long-term glycae-mic
   control and the presence of certain diabetic complications.
 
 
### Age:
Older adults are at high risk for the development of type 2 
diabetes due to the combined effects of increasing insulin
 resistance and impaired pancreatic islet function with aging.

### Blood pressure:
Over time, diabetes damages the small blood vessels in your body, causing the walls of the blood vessels to stiffen. This increases pressure, which leads to high blood pressure.” The combination of high blood pressure and type 2 diabetes can greatly increase your risk of having a heart attack or stroke.

Diabetes pedigree function:
A function which scores likelihood of diabetes based on family history.

## Dependencies:

### Pymongo
   PyMongo is the official MongoDB Python driver for MongoDB and it is used to work with MongoDB from Python.
### Pandas
  Pandas is mainly used for data analysis. Pandas allows importing data from various file formats such as comma-separated values, JSON, SQL, and Microsoft Excel. Pandas allows various data manipulation operations such as merging, reshaping, selecting, as well as data cleaning, and data wrangling features.

### Numpy
 NumPy, which stands for Numerical Python, is a library consisting of multidimensional array objects and a collection of routines for processing those arrays. Using NumPy, mathematical and logical operations on arrays can be performed.

### Matplotlib.pyplot
matplotlib.pyplot is a collection of functions that make matplotlib work like MATLAB. Each pyplot function makes some change to a figure: e.g., creates a figure, creates a plotting area in a figure, plots some lines in a plotting area, decorates the plot with labels, etc.

### Seaborn
Seaborn is an open-source Python library built on top of matplotlib. It is used for data visualization and exploratory data analysis. Seaborn works easily with dataframes and the Pandas library. The graphs created can also be customized easily.



## MongoDB
MongoDB is a document database used to build highly available and scalable internet applications. With its flexible schema approach, it’s popular with development teams using agile methodologies. Offering drivers for all major programming languages, MongoDB allows you to immediately start building your application without spending time configuring a database.

## Use of MongoDB
MongoDB is built on a scale-out architecture that has become popular with developers of all kinds for developing scalable applications with evolving data schemas.
As a document database, MongoDB makes it easy for developers to store structured or unstructured data. It uses a JSON-like format to store documents. This format directly maps to native objects in most modern programming languages, making it a natural choice for developers, as they don’t need to think about normalizing data. MongoDB can also handle high volume and can scale both vertically or horizontally to accommodate large data loads.



## MongoDB database
   Dataset is taken from Kaggle problem and is stored in MongoDB database. The name of database is ‘healthdb’ and the name of collection is ‘diabetes_data’ which is created inside the healthdb database.

## Dataset statistics								
Number of variables           -            10

Number of observations      -            768

Missing cells                       -            0

Duplicate rows                    -            0

## Variable types
Categorical                          -             2

Numeric                              -             8

## Variables

### _id :     (Categorical variable)

| Properties | Value       |  
| :-------- | :-------      | 
| Distinct values    | 768   | 
|Missing values       |  0    | 

### Pregnancies:     (Real number) 

| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |17       | 
|Missing values      |  0      | 
|     Mean value     |   3.84  |
| Std	             |  2.98   |
|Minimum value       |1        |
|   Maximum value    |     17  |



### Glucose:       (Real number)

| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |136     | 
|Missing values      |  0      | 
|     Mean value     |   121.11  |
| Std	             |  30.43   |
|Minimum value       |  44     |
|   Maximum value    |     199  |






### Blood Pressure:     (Real number)

| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |47    | 
|Missing values      |  0      | 
|     Mean value     |   72.25  |
| Std	             |  12.11   |
|Minimum value       |  24    |
|   Maximum value    |     122  |



### Skin Thickness:     (Real number)
| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |51   | 
|Missing values      |  0      | 
|     Mean value     |  26.51  |
| Std	             | 9.26  |
|Minimum value       |  7   |
|   Maximum value    |     63  |



### Insulin:     (Real number)
| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |186   | 
|Missing values      |  0      | 
|     Mean value     |  94.65  |
| Std	             | 105.54 |
|Minimum value       | 14  |
|   Maximum value    |     846 |



### Diabetes Pedigree Function:     (Real number)
| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |517  | 
|Missing values      |  0      | 
|     Mean value     |  .471  |
| Std	             | .331 |
|Minimum value       | .078 |
|   Maximum value    |     2.42|




### BMI:     (Real number)
| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |248  | 
|Missing values      |  0      | 
|     Mean value     |  32.45  |
| Std	             | 6.87|
|Minimum value       | 18.2 |
|   Maximum value    |     67.1|


	

### AGE:     (Real number)
| Properties | Value           |  
| :-------- | :-------         | 
| Distinct values    |52  | 
|Missing values      |  0      | 
|     Mean value     |  32.24  |
| Std	             | 11.76|
|Minimum value       | 21 |
|   Maximum value    |    81|

## Missing values
![1](https://user-images.githubusercontent.com/87273551/138477697-e411f5fa-7933-46f3-a58f-9bc06d9cf512.png)
## Unique values
![3](https://user-images.githubusercontent.com/87273551/138477917-d7c0f717-0f45-49f8-a835-a93a809ab937.png)
## Correlations
![2](https://user-images.githubusercontent.com/87273551/138478002-29aab8a4-6d67-4f9e-9915-beb1a4b864cf.png)

From the graph, we can observe that some features are highly correlated to others while some are very less correlate. Our aim is to find those features which are highly correlated and also how are these correlated.

| features | pearson correlation coefficient        |  
| :-------- | :-------         | 
| BMI & SkinThickness   |0.55 | 
|Age & Pregnancies      |  0.53     | 
|    Glucose & Outcome    |  0.49	 |
| Insulin & Glucose             | 0.36|
| Age & Bloodressure       | 0.33 |
|   BMI & Outcome     |   0.31|
|Insulin & SkinThickness|  0.29|
|BMI & BloodPressure|   0.28    |


## Conclusions: 

1. As the number of pregnancies increases, patients have more chances to be diabatic.

2. if the glucose content is more then there is a high chance of diabetes.

3. Chances of having diabetes increase with age. Tillage 30, the number of diabetes patients are less in caparison to the non-diabetic patients but after 30 number of diabetic patients increases.

4. There are some features which are linearly corelated

    a. BMI & SkinThickness	
  
    b. Age & Pregnancies 

    c. Glucose & Outcome	

    d. Insulin & Glucose	

    e. Age & Bloodressure 	

    f. BMI & Outcome 	

    g. Insulin & SkinThickness	

    h. BMI & BloodPressure
