# Identifying Mental Health in the Tech Industry Project
Date: February 2024

Welcome to the Identifying Mental Health in the Tech Industry Project. This repository holds the
dataset and accompanying Python analysis scripts for a survey conducted to explore features relative
to mental health treatment.

The goal of this project is to predict if an employee should seek treatment based on the selected
features from the survey.

## Repository Contents
- `survey.csv`: This is the raw dataset file. It includes all the responses collected from the survey. Each
row represents a single respondent's answers, and the columns represent individual questions or data
points collected.
- `code_file.ipynb`: A Jupyter notebook that contains the data analysis code. It includes data cleaning,
exploratory analysis, and statistical testing to derive insights from the survey data.
- `BAIT 509 Final Project Report.pdf`: This file contains the final report based on data and code.

## Data

Here is a breakdown of the key columns in `survey.csv`:
- `Timestamp`: Time the survey was submitted.
- `Age`: The age of the respondent.
- `Gender`: The gender of the respondent.
- `Country`: The country where the respondent belongs.
- `State`: If the respondent lives in the United States, which state or territory does the respondent live
in?
- `self_employed`: Are you self-employed?
- `family_history`: Do you have a family history of mental illness?
- `treatment`: Have you sought treatment for a mental health condition?
- `work_interfere`: If you have a mental health condition, do you feel that it interferes with your work?
- `no_employees`: How many employees does your company or organization have?
- `remote_work`: Do you work remotely (outside of an office) at least 50% of the time?
- `tech_company`: Is your employer primarily a tech company/organization?
- `benefits`: Does your employer provide mental health benefits?
- `care_options`: Do you know the options for mental health care your employer provides?
- `wellness_program`: Has your employer ever discussed mental health as part of an employee
wellness program?
- `seek_help`: Does your employer provide resources to learn more about mental health issues and how
to seek help?
- `anonymity`: Is your anonymity protected if you choose to take advantage of mental health or
substance abuse treatment resources?
- `leave`: How easy is it for you to take medical leave for a mental health condition?
- `mental_health_consequence`: Do you think that discussing a mental health issue with your employer
would have negative consequences?
- `phys_health_consequence`: Do you think that discussing a physical health issue with your employer
would have negative consequences?
- `coworkers`: Would you be willing to discuss a mental health issue with your coworkers?
- `supervisor`: Would you be willing to discuss a mental health issue with your direct supervisor(s)?
- `mental_health_interview`: Would you bring up a mental health issue with a potential employer in an
interview?
- `phys_health_interview`: Would you bring up a physical health issue with a potential employer in an
interview?
- `mental_vs_physical`: Do you feel that your employer takes mental health as seriously as physical
health?
- `obs_consequence`: Have you heard of or observed negative consequences for coworkers with
mental health conditions in your workplace?
- `comments`: Any additional notes or comments

## Getting Started

To reproduce the analysis, follow these steps:
1. Install Python on your system. The code is written for Python 3.x.
2. Open the `code_file.ipynb` notebook in Jupyter Lab or Jupyter Notebook.
3. Run the cells in the notebook from top to bottom to perform the data analysis.

## Process Explained
1. Perform basic data analysis
   - Review the summary of data
   - Data cleaning (fix typo in gender column)
   - Identify numeric and categorical objects
2. Data preprocessing:
   - Split data into training and test set
   - Identify the target column and include the key features to predict the target
3. Build pipeline
   - Make a pipeline to transform numeric and categorical objects
   - For numeric columns: Perform data imputation and standard scaling
   - For categorical objects: Perform data imputation and one-hot encoding
4. Create a dummy model as our baseline model for comparison.
5. Perform cross-validation with hyperparameter search for various models:
   - Decision Tree
   - SVC
   - Logistic Regression
   - Random Forest Regression
6. Model evaluation & selection
   - Create a confusion matrix to compare the accuracy & precision of each model
   - Select the best model

Data License

The dataset used in our analysis is available under the CC BY-SA 4.0 license.
Source: https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey

Questions and Comments

Should you have any questions or require further clarification, feel free to contact project group
member at carazhou0322@gmail.com, kqz0808@gmail.com, yifeiw07@student.ubc.ca,
and linyoung9198@gmail.com.
