# Absenteeism-Preprocessed
cleaned and preprocessed the dataset  for further predictive analysis
# Absenteeism Data Analysis and Preprocessing Project

## Project Overview

This project focuses on the cleaning, preprocessing, and exploratory analysis of the "Absenteeism at work" dataset. The primary goal is to transform the raw data into a clean, well-structured format suitable for data analysis and ready for future machine learning applications.

The key tasks performed in this project include handling categorical data, feature engineering from date-time columns, and preparing the dataset for analytical queries.

---

## Data Preprocessing Steps

The Jupyter Notebook (`Absenteeism (1).ipynb`) in this repository details the following preprocessing steps:

1.  **Categorical Data Handling (`Reason for Absence`):**
    * The 'Reason for Absence' column, containing 28 different numerical codes, was transformed into a more manageable format.
    * **Dummy variables** were created from the original codes to convert them into a numerical format suitable for analysis.
    * To simplify and create more powerful features, these dummy variables were then grouped into four main meaningful categories:
        1.  **Diseases:** Absences due to various diagnosed diseases.
        2.  **Pregnancy:** Absences related to pregnancy or childbirth.
        3.  **Symptoms:** Absences due to non-specific medical symptoms.
        4.  **Appointments:** Absences for medical, dental, or other appointments.

2.  **Date and Time Feature Engineering (`Date`):**
    * The 'Date' column was converted from a string to a proper datetime object.
    * New features were extracted from the date:
        * **Month of Absence:** To analyze monthly trends.
        * **Day of the Week:** To analyze weekly patterns in absenteeism.

3.  **Categorical Data Handling (`Education`):**
    * The 'Education' column was converted into dummy variables to properly represent the different educational levels as distinct categories.

4.  **Final Cleanup:**
    * All original and intermediate columns (like the original 'Reason for Absence' and 'Date' columns) were dropped to avoid data redundancy, leaving a final, clean dataset.
    * The final preprocessed data was saved to `absenteeism-data-preprocessed.csv`.

---

## How to Use This Repository

1.  **Clone the repository:**
    ```bash
    ```git clone https://github.com/SahilPatel010/Absenteeism-Preprocessed.git
2.  **Open the Jupyter Notebook:**
    * Navigate to the project folder and open `Absenteeism (1).ipynb` using Jupyter Notebook or JupyterLab to see the full code and step-by-step process.
3.  **View the Data:**
    * `Absenteeism-data.csv` is the original, raw data.
    * `absenteeism-data-preprocessed.csv` is the final, clean dataset ready for analysis.

---

## Tools and Libraries

* **Python 3**
* **Pandas:** For data manipulation and analysis.
* **Jupyter Notebook:** For interactive code development and documentation.
