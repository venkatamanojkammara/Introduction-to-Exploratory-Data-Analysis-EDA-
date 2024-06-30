# Exploratory Data Analysis EDA
## 1. Introduction
Exploratory Data Analysis (EDA) is a process to analyze the data and summarize their main characteristics, often with visual methods. EDA is crucial before applying any Machine Learning algorithum as it helps understand the data, detect patterns, spot anomalies, and check assumptions.
## 2. Python Libraries Required for EDA
  
  - Pandas: For data manipulation and analysis.
  
  - NumPy: For numerical operations.
  
  - Matplotlib: For basic plotting and visualization.
  
  - Seaborn: For more advanced statistical visualizations.

### 2.1 Installing Libraries :

  - `pip install pandas`
    
  - `pip install numpy`

  - `pip install matplotlib`
    
  - `pip install seaborn`

## 3. Steps in Exploratory Data Analysis 
### 3.1 Data Collection
Collect data from various sources (CSV, excel, databases, web scraping, APIs).
  
  - `read_csv(filename)`
  - `read_excel(filename)`
    
### 3.2 Data Cleaning
  - **Handling Missing Values :** Identify and handle missing values (e.g., fill, drop).
  - **Removing Duplicates :** Identify and remove duplicate rows.
  - **Data Type Conversion :** Convert data to appropriate types.

### 3.3 Understanding the Data
  - **Descriptive Statistics :** Use methods like `.describe()` to get a summary of the data.
  - **Data Shape and Types :** Check the shape and data types using `.shape` and `.dtypes.`

### 3.3 Visualize the Data 
  - **Histograms :** For understanding the distribution of numeric data.
  - **Box Plots :** For detecting outliers.
  - **Scatter Plots :** For visualizing relationships between two variables.
  - **Correlation Matrix :** For understanding correlations between variables.

### 3.4 Data Transformation
  - **Feature Engineering :** Create new features from existing ones.
  - **Normalization and Scaling :** Normalize or scale numerical data for better performance of models.

## 4. Exploratory Data Analysis with Python
### 4.1 Importing Libraries
    import numpy as np
    import matplotlib.pyplot as plt
    import pandas as pd
    import seaborn as sns
### 4.2 Reading the Data
  For CSV files
  
   `df=pd.read_csv('filename.csv')`

   For Excel files
   
   `df=pd.read_excel('filename.xlsx')`

### 4.3. Data Cleaning
   **Handling missing values**
   
   Fill missing values with mean
     
   `df.fillna(df.mean(), inplace=True)`

  Drop rows with missing values

   `df.dropna(inplace=True)`

   **Removing duplicates**
 
   `df.drop_duplicates(inplace=True)`

   **Data type conversion**

   `df['column_name'] = df['column_name'].astype('int')`

### 4.4 Understanding Data
   **Descriptive statistics**

   `print(df.describe())`

   **Data shape and types**

    print(df.shape)
    print(df.dtypes)

### 4.5 Data Visualization

   **Histogram**

    plt.hist(df['column_name'], bins=30)
    plt.xlabel('Column Name')
    plt.ylabel('Frequency')
    plt.title('Histogram of Column Name')
    plt.show()

   **Box plot**
   
    sns.boxplot(x=df['column_name'])
    plt.title('Box Plot of Column Name')
    plt.show()

   **Scatter plot**

    plt.scatter(df['column1'], df['column2'])
    plt.xlabel('Column 1')
    plt.ylabel('Column 2')
    plt.title('Scatter Plot of Column 1 vs Column 2')
    plt.show()

   **Correlation matrix**
   
    correlation_matrix = df.corr()
    sns.heatmap(correlation_matrix, annot=True)
    plt.title('Correlation Matrix')
    plt.show()

## 5. Conclusion
Exploratory Data Analysis is an iterative process that helps understand the data, which is crucial for making the decisions before building any Machine Learning models. Regular practice and exploration of different datasets will enhance your EDA skills.



  
   
