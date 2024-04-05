# Pymaceuticals Data Analysis
 Applied Matplotlib data and library knowledge to a real-world situation and dataset.

# Repo Direction 
- Created a new repository for this project called #Matplotlib-Data-Visualization, Cloned the new repository(remote) to local by terminal.

- Inside my local Git repository, created a folder for "Pymaceuticals"

- Added Jupyter notebook "(pymaceuticals_starter_Roshni.ipynb)" to this folder. This is the main script to run this analysis.

- A Data folder that contains the CSV files(Raw Data) i have used. 

- Also this folder that contains "pdf" file that has the results from the conducted analysis.

- Pushed these changes to GitHub profile by bash terminal.

# Background 
Pymaceuticals, Inc., 
A new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company,have been given access to the complete data from their most recent animal study. 
In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

# Analysis Instructions
Task was broken down into the following tasks:

1. Data Prepration

2. Generating summary statistics.

3. Creation of bar charts and pie charts.

4. Calculation for quartiles, find outliers, and creation of a box plot.

5. Creation for a line plot and a scatter plot.

6. Calculation for correlation and regression.

7. Final analysis.

# 1.  Data Prepration
- Ran the required package dependency and data imports, and then merged the mouse_metadata and study_results DataFrames into a single DataFrame.

- Displaied the number of unique mice IDs in the data, and then checked for any mouse ID with duplicate time points. Displaied the data associated with that mouse ID, and then created a new DataFrame where this data is removed. Used this cleaned DataFrame for the remaining steps.

- Displaied the updated number of unique mice IDs.

# 2.  Generating summary statistics.
Created a DataFrame of summary statistics. There Was more than one method to produce the results after.

Summary statistics are included:

A row for each drug regimen. These regimen names have contained in the index column.

A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

# 3. Creation of bar charts and pie charts.
Generated two bar charts. 
Both charts have identicals and the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

Created the first bar chart with the Pandas DataFrame.plot() method.

Created the second bar chart with Matplotlib's pyplot methods.

Generated two pie charts. Both charts have identical and shown the distribution of female versus male mice in the study.

Created the first pie chart with the Pandas DataFrame.plot() method.

Created the second pie chart with Matplotlib's pyplot methods.

# 4.Calculation for quartiles, find outliers, and creation of a box plot.
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.
