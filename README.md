# Data-Visualization-Challenge
Data Visualization Challenge

Overview

This analysis examines data from a Pymaceuticals study on the effectiveness of various drug treatments for squamous cell carcinoma (SCC). The study involved 249 mice and tracked their tumor development over 45 days. The analysis focuses on summarizing the data, generating plots, and calculating key statistics to support the clinical study report.

Files Used

	•	mouse_metadata.csv: Contains metadata about the mice, including mouse ID, gender, and age.
	•	study_results.csv: Includes tumor measurement data for each mouse across different time points and drug treatments.

Data Preparation

	1.	Data Merging: Combined mouse_metadata and study_results DataFrames into a single DataFrame.
	2.	Duplicate Handling: Identified and removed duplicate time points for any mouse ID, resulting in a cleaned DataFrame.
	3.	Unique Mice Count: Displayed the number of unique mice IDs before and after removing duplicates.

Summary Statistics

	•	Statistics Calculated: Mean, median, variance, standard deviation, and SEM of tumor volume for each drug regimen.
	•	Method: Generated the summary statistics DataFrame using groupby and summary methods.

Bar and Pie Charts

	1.	Bar Charts:
	•	Pandas: Generated a bar chart showing the number of rows (Mouse ID/Timepoints) for each drug regimen.
	•	Matplotlib: Created a similar bar chart using Matplotlib’s pyplot.
	2.	Pie Charts:
	•	Pandas: Created a pie chart to visualize the distribution of female versus male mice.
	•	Matplotlib: Produced a similar pie chart using Matplotlib’s pyplot.

Quartiles, Outliers, and Box Plot

	1.	Final Tumor Volume: Calculated the final tumor volume for mice across four drug regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.
	2.	Outlier Detection: Determined potential outliers using quartiles and IQR.
	3.	Box Plot: Generated a box plot to show the distribution of final tumor volumes, highlighting outliers.

Line Plot and Scatter Plot

	1.	Line Plot: Created a line plot of tumor volume versus time point for mouse ID I509, treated with Capomulin.
	2.	Scatter Plot: Generated a scatter plot of mouse weight versus average tumor volume for the Capomulin regimen.

Correlation and Regression

	1.	Correlation Coefficient: Calculated the Pearson correlation coefficient between mouse weight and average tumor volume.
	2.	Linear Regression: Computed the linear regression model and plotted the regression line on the scatter plot.
