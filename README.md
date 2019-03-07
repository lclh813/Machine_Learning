# Machine Learning
## Notice
It is possible that GitHub fails to display Jupyter Notebooks. Should such circumstances arise, please refer to ***Part 4. Steps*** listed below for code samples.

## Part 1. Objective
To estimate the ***Sales Rank*** of a specific fruit based on its ***Sales Volume, Turnover, Cost, Gross Profit, and Gross Margin.***

## Part 2. Data

| Rank  | Fruit_Type | Fruit_Name_ID | Fruit_Name        | Sales Volume | Turnover | Cost  | Gross Profit | Gross Margin | Supplier | 
| :---: | :---:      | :---:         | :---              | :---:        | :---:    | :---: | :---:        | :---:        | :---:    |
| 1     | Apple      | APPL001       | Red Delicious     | 100          | 2,000    | 1,200 | 800          | 0.40         | Farm 4   |
| 2     | Kiwifruit  | KIWI001       | Sungold Kiwifruit | 96           | 3,500    | 2,800 | 700          | 0.20         | Farm 1   |
| ...   | ...        | ...           | ...               | ...          | ...      | ...   | ...          | ...          | ...      |
| 49    | Apple      | APPL002       | Royal Gala        | 18           | 500      | 450   | 50           | 0.10         | Farm 2   |
| 50    | Grape      | GRAP001       | Golden Muscat     | 15           | 480      | 360   | 120          | 0.25         | Farm 4   |

## Part 3. Outline
### 3.1. Data Transformation
- Create separate bins for different sales ranks.
### 3.1.1. Option 1: Categorization
- Databins are classified as ***categorical*** data.
- Tool: Python pandas ```cut``` 
### 3.1.2. Option 2: Category Labeling
- Databins are classified as ***numerical*** data.
- Tool: Python pandas ```loc```

### 3.2. Data Splitting
### 3.2.1. Independent and Dependent Variable
- Specify independent and dependent variables.
- Tool: Python pandas ```iloc```
### 3.2.2. Training and Validation Data
- Split data into training and validation sets.
- Tool: Python sklearn ```model_selection```

### 3.3. Model Selection
### 3.3.1. Data Transformation
### 3.3.1.1. Option 1: Categorical data
- Categorical data cannot be used for further analysis and therefore should be transformed into ***object*** property.
- Tool: Python pandas ```astype```
### 3.3.1.2. Option 2: Numerical data
-  Data transformation will not be necessary.

### 3.3.2. Model Deployment
- Implement classification algorithms.
- Tool: Python sklearn ```LogisticRegression``` ```LinearDiscriminantAnalysis``` ```KNeighborsClassifier``` ```DecisionTreeClassifier``` ```GaussianNB``` ```SVC```

### 3.3.3. Model Evaluation
- Evaluate model fits by focusing on ***predictive accuracy.***
- Tool: Python sklearn ```model_selection.cross_val_score```

### 3.3.4. Data Training
- Fit the model to training data.
- Tool: Python sklearn ```fit``` 

### 3.3.5. Data Validation
- Compare the prediction with the actual results.
- Tool: Python sklearn ```predict``` ```accuracy_score``` 

### 3.4. Prediction
- Put numbers into independent variables and get the dependent variable ***Sales Rank*** as the result.
- Tool: Python pandas```DataFrame``` sklearn ```predict```

## Part 4. Steps
### Overview of Machine Learning
- The machine learning process adopted by this analysis will be following the flow of ***blue arrows.*** 

<br>
<div align=center><img src="https://github.com/lclh813/Machine_Learning/blob/master/Pic/4_MachineLearningOverview.png"/></div>
<br>

> [***Complete Code***](https://nbviewer.jupyter.org/github/lclh813/Machine_Learning/blob/master/6_CompleteCode.ipynb) 
#### [Step 1. Preparation](https://nbviewer.jupyter.org/github/lclh813/Machine_Learning/blob/master/1_Preparation.ipynb)
#### [Step 2. Data Transformation](https://nbviewer.jupyter.org/github/lclh813/Machine_Learning/blob/master/2_DataTransformation.ipynb)
#### [Step 3. Data Splitting](https://nbviewer.jupyter.org/github/lclh813/Machine_Learning/blob/master/3_DataSplitting.ipynb)
#### [Step 4. Model Selection](https://nbviewer.jupyter.org/github/lclh813/Machine_Learning/blob/master/4_ModelSelection.ipynb)
#### [Step 5. Prediction](https://nbviewer.jupyter.org/github/lclh813/Machine_Learning/blob/master/5_Prediction.ipynb)
