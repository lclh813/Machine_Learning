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
- Tool: pandas ```cut``` ```loc```

### 3.2. Data Splitting
### 3.2.1. Independent and Dependent Variable
- Specify independent and dependent variables.
- Tool: pandas ```iloc```
### 3.2.2. Training and Validation Data
- Split data into training and validation sets.
- Tool: sklearn ```model_selection```

# 3.3. Model Selection
### 3.3.1. Model Deployment
- classification algorithm


## Part 4. Steps
Complete Code
### Step 1. Preparation
1.1. Import Library
