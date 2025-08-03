# Course 10: Applied Data Science Capstone

This folder contains my final project for **Course 10** of the IBM Data Science Professional Certificate:  
**Applied Data Science Capstone**.

---

## Course Overview

This capstone project brought together everything I've learned in the previous 9 courses of the IBM Data Science track. It emphasized applying data science methodology in a real-world context, particularly focused on **predictive analytics and geospatial analysis**.

Key skills and tools used:
- Data acquisition via APIs and web scraping
- Data wrangling and exploratory data analysis  
- Machine learning classification models
- Interactive visualizations with **Folium** and **Plotly Dash**
- SQL data analysis
- Geospatial mapping and analysis

---

## Final Capstone Project: SpaceX Falcon 9 First Stage Landing Prediction

### Project Description

In this project, I developed a comprehensive data science solution to predict the success of SpaceX Falcon 9 first-stage landings. This analysis is crucial for determining launch costs, as SpaceX's competitive advantage comes from reusing the first stage, which accounts for approximately 60% of total launch costs.

**Business Problem:** An alternate space company needs to predict Falcon 9 first-stage landing success to determine competitive launch pricing and make informed bids against SpaceX.

**Key Findings:**
- SpaceX's landing success rate improved dramatically from 0% (flights 1-9) to 70%+ (flights 20-49)
- KSC LC-39A achieved the highest success rate at 76.9% among launch sites
- Block 5 boosters demonstrate 100% success rate with advanced technology
- SpaceX's reusability reduces launch costs by up to 70%, from $165M to $67M per launch

---

## Methodology & Workflow

### 1. **Data Collection**
   - **SpaceX REST API:** Retrieved launch data from `/v4/launches/past` endpoint
   - **Wikipedia Web Scraping:** Used BeautifulSoup to extract additional launch records
   - **Features Collected:** Flight Number, Date, Booster Version, Payload Mass, Orbit, Launch Site, Landing Outcome, etc.

### 2. **Data Wrangling & Preprocessing**
   - Created binary classification labels (1=successful landing, 0=failed landing)
   - Outcome mapping: `True ASDS/RTLS/Ocean` → 1, `False/None` outcomes → 0
   - Handled missing values using mean imputation for payload mass
   - Feature engineering and data type conversions

### 3. **Exploratory Data Analysis (EDA)**
   - **Tools:** Pandas, Matplotlib, Seaborn
   - **Analysis:** Success rates by flight number, launch site, payload mass, and orbit type
   - **Key Insights:** Identified improvement trends over time and optimal launch conditions
   - **Feature Engineering:** One-hot encoding for categorical variables

### 4. **SQL Data Analysis**
   - Database queries for aggregated statistics
   - Launch site performance comparisons
   - Payload mass analysis by booster version
   - Mission outcome distributions

### 5. **Geospatial Analysis**
   - **Interactive Folium Maps:** Visualized all launch sites with success/failure markers
   - **Proximity Analysis:** Analyzed launch sites' proximity to railways, highways, and coastlines
   - **Color-coded Markers:** Green for successful landings, red for failures
   - **Strategic Insights:** All launch sites are strategically located near oceans for safety

### 6. **Interactive Dashboard Development**
   - **Plotly Dash Application:** Built interactive web dashboard
   - **Features:**
     - Pie charts showing success rates by launch site
     - Scatter plots analyzing payload mass vs. success rate
     - Real-time filtering by launch site and payload range
     - Booster version analysis with color coding

### 7. **Machine Learning Classification**
   - **Models Implemented:** Logistic Regression, Support Vector Machine (SVM), Decision Tree, K-Nearest Neighbors (KNN)
   - **Data Preprocessing:** StandardScaler for feature normalization
   - **Hyperparameter Tuning:** GridSearchCV with 10-fold cross-validation
   - **Train/Test Split:** 80/20 ratio
   - **Best Performance:** Logistic Regression, SVM, and KNN achieved **83.3% prediction accuracy**

---

## Key Results & Insights

### Technical Results
- **Model Accuracy:** 83.3% prediction accuracy using optimized models
- **Best Performing Models:** Logistic Regression, SVM, KNN (tied)
- **Feature Importance:** Flight number, booster version, and launch site were key predictors

### Business Insights
- **Cost Impact:** Successful landings save up to $98M per launch ($165M → $67M)
- **Launch Site Performance:** KSC LC-39A shows highest success rate (76.9%)
- **Technology Evolution:** Block 5 boosters demonstrate 100% reliability
- **Temporal Trends:** Clear improvement in success rates after flight 20

### Strategic Recommendations
- **Competitive Pricing:** Use 83.3% accuracy model for bid calculations
- **Launch Site Selection:** Prioritize KSC LC-39A for critical missions
- **Technology Investment:** Focus on Block 5 booster technology
- **Risk Assessment:** Consider payload mass and orbit type in pricing models

---

## Technologies & Libraries Used

**Data Collection & Processing:**
- `requests` - API calls and web scraping
- `BeautifulSoup` - HTML parsing
- `pandas` - Data manipulation and analysis
- `numpy` - Numerical computations

**Visualization & Mapping:**
- `matplotlib` & `seaborn` - Statistical visualizations
- `folium` - Interactive geospatial mapping
- `plotly` & `dash` - Interactive dashboard development

**Machine Learning:**
- `scikit-learn` - Classification algorithms and model evaluation
- `GridSearchCV` - Hyperparameter optimization
- `StandardScaler` - Feature normalization

**Database Analysis:**
- Magic SQL queries for data aggregation and analysis

---

## What I Learned

- **End-to-End Data Science Workflow:** From data collection to model deployment
- **API Integration:** Working with RESTful APIs and handling JSON responses
- **Web Scraping:** Extracting structured data from HTML tables
- **Geospatial Analysis:** Creating interactive maps and analyzing location-based patterns
- **Machine Learning Pipeline:** Feature engineering, model selection, and hyperparameter tuning
- **Dashboard Development:** Building interactive web applications for data exploration
- **Business Analytics:** Translating technical findings into actionable business insights
- **Data Storytelling:** Presenting complex analysis through clear visualizations and narratives

---

## Project Achievements

This capstone project successfully demonstrates:
- **Technical Proficiency:** Applied multiple data science techniques in a cohesive workflow
- **Business Acumen:** Addressed real-world business problem with actionable insights
- **Data Visualization:** Created compelling visual narratives for stakeholder communication
- **Model Performance:** Achieved 83.3% accuracy in predicting mission-critical outcomes
- **Industry Relevance:** Provided competitive intelligence for space industry applications

---

## About

This project was created as the capstone for the **IBM Data Science Professional Certificate** and represents the culmination of comprehensive data science training covering the entire analytics lifecycle.

**Author:** Wasiq Amir 
