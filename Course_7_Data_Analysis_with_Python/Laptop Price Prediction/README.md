# Module-by-Module Labs: Data Analysis with Python

This folder contains 5 Jupyter notebooks that progressively build skills in data analysis using Python. Each notebook focuses on a specific stage of the data analysis pipeline, using a laptop pricing dataset throughout.

## Dataset
- **Source**: IBM laptop pricing dataset
- **Purpose**: Predict laptop prices based on various features
- **Features**: Manufacturer, Category, GPU, OS, CPU cores, Screen size, CPU frequency, RAM, Storage, Weight, Price

## Notebooks Overview

### 1. Data-Importing.ipynb
**Objective**: Learn to import and explore datasets
- Load CSV data using pandas
- Explore dataset structure with `.head()`, `.info()`, `.describe()`
- Basic data inspection and understanding

### 2. Data-Wrangling.ipynb
**Objective**: Clean and preprocess data for analysis
- Handle missing data using various strategies
- Correct data types and format conversions
- Standardize and normalize numerical features
- Create binned categories for visualization
- Convert categorical variables to numerical indicators
- Data transformation techniques

### 3. EDA.ipynb (Exploratory Data Analysis)
**Objective**: Analyze data patterns and relationships
- Visualize individual feature distributions
- Statistical summary analysis
- Group analysis and pivot tables
- Correlation analysis using Pearson correlation
- Data visualization with matplotlib and seaborn
- Identify key features affecting laptop prices

### 4. Model-Development.ipynb
**Objective**: Build and compare regression models
- Simple linear regression (single variable)
- Multiple linear regression
- Polynomial regression for non-linear relationships
- Create scikit-learn pipelines
- Model comparison using MSE and R² metrics
- Feature selection and engineering

### 5. Model-Evaluation.ipynb
**Objective**: Validate and improve model performance
- Train/test split strategies
- Cross-validation techniques
- Identify overfitting in models
- Ridge regression for regularization
- Grid search for hyperparameter tuning
- Model performance optimization

## Skills Demonstrated

### Technical Skills
- **Data Import**: Loading datasets from various sources
- **Data Cleaning**: Handling missing values, data type corrections
- **Data Transformation**: Normalization, standardization, feature engineering
- **Statistical Analysis**: Descriptive statistics, correlation analysis
- **Visualization**: Creating informative plots and charts
- **Machine Learning**: Building, evaluating, and tuning regression models

### Tools & Libraries
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical operations
- **matplotlib & seaborn**: Data visualization
- **scikit-learn**: Machine learning algorithms
- **scipy**: Statistical functions

## Learning Progression

Each notebook builds upon the previous one:
1. **Import** → Basic data loading and exploration
2. **Wrangle** → Clean and prepare data for analysis
3. **Explore** → Understand patterns and relationships
4. **Model** → Build predictive models
5. **Evaluate** → Validate and improve models

## Key Achievements
- Comprehensive understanding of the data analysis workflow
- Hands-on experience with real-world data challenges
- Practical application of machine learning techniques
- Professional-quality code with clear documentation
- Reproducible analysis methods

This series of notebooks provides a complete foundation in data analysis using Python, from initial data exploration to final model evaluation.
