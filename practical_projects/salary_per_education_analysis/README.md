# ⚠️ Project in progress...

# **Preparation for the project**

## **Objectives**

The main objective of this analytics project is to establish a correlation between education level and salary. Subsequently, the goal is to elaborate a comprehensive report, including a dashboard and the key insights derived from all the analysis.

## **Data Sources**

The dataset was obtained from multiple sources, including surveys, job posting sites, and other publicly available resources. All the data pertains to India.

## **Dataset**

A total of 6704 data points were collected. The dataset included five variables: age, experience_years, job role, education level, and salary.
Last update: 2023

Here is the link to the dataset page on Kaggle:
https://www.kaggle.com/datasets/mohithsairamreddy/salary-data/data

# **The project**

## **Cleaning and Manipulating Data**

The first step was to download and import the dataset into Excel, then use the "Text to Columns" feature to read the CSV file and convert its type to .xlsx. Subsequently, I removed the blank rows and converted the data into a table format. I was unable to remove duplicates because there was no primary key (PK) in the original dataset.

I converted the Salary values from INR (Indian Rupees) to USD (United States Dollars) and filtered the data to remove rows containing blank cells, as well as some inconsistent salary entries (e.g., $6 a month). I also removed non-integer values from the "Years of Experience" column.

I corrected the spelling within the "Education Level" column, resulting in four distinct categories: High School, Bachelor's Degree, Master's Degree, and PhD. Additionally, I created a new field, named "Knowledge Area," which indicates the worker's field of expertise (this was achieved using AI).

## **Descriptive Analysis**

For this stage, I utilized conditional formulas to calculate the mean, Coefficient of Variation (CV), and Median for each Education Level. I also generated a box plot displaying salary distribution per education level.

## **Data Enrichment**

Some data points were synthetically generated to complete the pivot tables, using the mean proportion relative to existing data points. These generated data points can be identified by searching for "generated datapoint" in the "Job Title" column.

## **Pivot Tables and Charts**

1. Salary per education and experience years, presented with an area chart (generated data was primarily used for the "High School" category).
2. Salary per gender and age, displayed with a line chart (some generated data was used here).
3. Salary per field of work, visualized with a column chart.
