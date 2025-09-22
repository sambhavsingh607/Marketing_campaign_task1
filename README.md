Marketing Campaign Data Analysis
This project focuses on cleaning, preprocessing, and analyzing a marketing campaign dataset. The goal is to prepare the raw data for further exploratory data analysis (EDA) and machine learning modeling.

Project Structure
marketing_campaign.csv: The original raw dataset containing customer information and campaign performance.

Task_1.ipynb: A Jupyter Notebook detailing the data cleaning and preprocessing steps.

cleaned_marketing_campaign.csv: The output of the data cleaning process, a tidy dataset ready for analysis.

Task 1: Data Cleaning and Preprocessing
The primary objective of this task was to clean and prepare the raw marketing_campaign.csv dataset. The following steps were performed in the Task_1.ipynb notebook:

Data Loading: The dataset was loaded into a Pandas DataFrame using the correct tab (\t) delimiter.


Handling Missing Values: The Income column, which contained 24 missing values, was imputed with the median value to maintain data integrity and avoid data loss.


Removing Duplicates: All duplicate rows were identified and removed using the df.drop_duplicates() function to ensure each record is unique and to prevent skewed analysis.

Standardizing Data:

Text values in the Education and Marital_Status columns were converted to a consistent title case format.

All column headers were standardized to be lowercase with underscores (e.g., 

Year_Birth became year_birth).

Data Type Conversion:

The 

Dt_Customer column was converted to a datetime object for proper time-based analysis.

The 

Year_Birth and Income columns were converted to the appropriate numeric data types.

Feature Engineering: A new column, age, was created by calculating the difference between the current year and the year_birth to provide a more direct measure for analysis.

How to Use
Clone this repository.

Navigate to the project directory.

Open and run the Task_1.ipynb notebook to see the data cleaning process in action.

The cleaned_marketing_campaign.csv file is ready for your further analysis or modeling tasks.
