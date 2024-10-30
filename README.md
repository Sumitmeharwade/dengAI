# dengAI - Predicting Dengue Disease Spread

This project, **dengAI**, aims to predict the weekly spread of dengue fever based on environmental and climate-related data, designed as a submission for a competition on DrivenData. By analyzing historical climate factors and their influence on dengue cases, this project seeks to establish predictive insights for public health planning and resource allocation.

## Project Overview

The primary objective is to predict dengue cases using environmental features. The analysis workflow involves data preprocessing, exploratory data analysis (EDA), and predictive modeling to identify trends and seasonality in dengue outbreaks. The project includes feature exploration and preliminary model development to identify optimal predictive factors.

## Dataset Description

The datasets are organized into training and testing subsets, sourced from public health and climate databases. Files included are:

- **dengue_features_train.csv**: Contains weekly environmental and climate features related to dengue spread.
- **dengue_labels_train.csv**: Labels indicating weekly dengue cases for supervised learning.
- **dengue_features_test.csv**: Test dataset to generate predictions for unknown cases.
- **submission_format.csv**: Template for formatting final submissions in accordance with competition requirements.

Key features include temperature, humidity, and precipitation, which significantly impact disease prevalence.

## Project Workflow

### 1. Data Import and Preprocessing
   - **Loading and Merging**: Combining feature and label datasets to prepare a unified data structure.
   - **Handling Missing Values**: Cleaning data by imputing or handling missing values to ensure model robustness.
   - **Feature Scaling**: Scaling features for consistency, aiding model performance.

### 2. Exploratory Data Analysis (EDA)
   - **Distribution Analysis**: Examining temporal and geographical distribution of dengue cases.
   - **Climate Feature Exploration**: Analyzing temperature, humidity, and precipitation trends to uncover seasonality patterns.
   - **Visualization**: Using `matplotlib`, `seaborn`, and `plotly` to visualize feature relationships and trends.

### 3. Modeling and Prediction
   - **Feature Selection**: Using insights from EDA to select significant features.
   - **Model Building**: Testing various models to predict the number of weekly dengue cases.
   - **Evaluation**: Assessing model performance using appropriate metrics.

### 4. Submission
   - **Output Generation**: Formatting predictions according to `submission_format.csv` for competition submission.

## Requirements

- Python 3.x
- Jupyter Notebook
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `plotly`
  - `scikit-learn`
  - `geopandas` (for geographical data analysis)

## Usage

To reproduce the analysis:

1. Clone this repository:
   ```bash
   git clone https://github.com/Sumitmeharwade/dengAI.git
   cd dengAI
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook to view the analysis:
   ```bash
   jupyter notebook DengAI.ipynb
   ```
