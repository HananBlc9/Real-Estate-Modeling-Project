# Real Estate: Data Integration, Cleaning API & Modeling Project

## Objectives

This project simulates a real-world data science task. The goal is to:

- Collect property data from two real estate APIs.
- Clean and integrate the raw datasets.
- Build a robust predictive model to estimate property prices.

The final deliverable is a well-structured GitHub repository containing all project components.

---

## APIs Used for Data Collection

- **API 1:** [Datafiniti Property Data API](https://www.datafiniti.co/data/property-data)
- **API 2:** Local(LLM-generated dummy data)

---

## Steps Taken in Data Collection and Cleaning

1. **API Integration**  
   - Pulled real estate listings from **Datafiniti API**.
   - Generated dummy property data using **LLM** for the second data source.

2. **Data Processing**  
   - Merged data from both sources into a unified dataset.
   - Removed duplicate entries and handled missing/null values.
   - Standardized formatting, column names, and data types.
   - Filled or removed incomplete columns.
   - Exported the final cleaned dataset as a CSV.

3. **Data Cleaning API (Challenge)**  
   - Built a RESTful API using **FastAPI** for data cleaning.
   - Endpoint accepts raw CSV and returns cleaned data.
   - Source code: a cell in the notebook

---

## Modeling Approach and Results

1. **Objective**: Predict property prices based on attributes.

2. **Models Used**:
   - Linear Regression *(Best performing)*
   - Random Forest
   - Decision Tree
   - Lasso Regression
   - Ridge Regression

3. **Results**:
   - **Linear Regression** achieved the best R² score and overall performance.
   - Evaluation metrics are provided in the notebook.

---

## Repository Structure

├── data/
│ ├── 967941_1.csv
│ ├── generated_property_data.csv
│ └── cleaned_data.csv
|
├── notebooks/
│ └── exploration_and_modeling.ipynb
│
└── README.md
