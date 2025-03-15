# PyMaceuticals Clinical Study Analysis

## Background
PyMaceuticals, Inc. is a pharmaceutical company specializing in anti-cancer medications. The company recently conducted a clinical study to test potential treatments for squamous cell carcinoma (SCC), a common form of skin cancer. The study involved 249 mice, each diagnosed with SCC tumors, and tested the efficacy of different drug regimens, including the company's drug of interest, Capomulin. Tumor development was monitored over 45 days to compare the performance of Capomulin against other treatments.

## Objective
The purpose of this analysis is to generate all necessary tables and figures for the technical report on the clinical study. Additionally, a top-level summary of the study results is provided for the executive team.

## Dataset
The dataset includes:
- Mouse metadata ("Mouse ID","Drug Regimen","Sex","Age_months","Weight (g)")
- Tumor volume measurements over time
- Timepoints for tumor progression

## Requirements
To run the notebook successfully, you need the following:
- Python 3.x
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- NumPy

Install the required libraries using:
```bash
pip install pandas matplotlib seaborn numpy
```

## Analysis Steps
### 1. Prepare the Data
- Merge mouse metadata and study results into a single DataFrame.
- Identify and remove duplicate time points for any mouse.
- Display the number of unique mice before and after data cleaning.

### 2. Generate Summary Statistics
- Create a DataFrame with summary statistics for each drug regimen, including:
  - Mean, median, variance, standard deviation, and standard error of the tumor volume.

### 3. Create Bar Charts and Pie Charts
- Bar charts:
  - Display the total number of time points per drug regimen using both Pandas' `plot()` and Matplotlib's `pyplot`.
- Pie charts:
  - Show the distribution of male and female mice using both Pandas' `plot()` and Matplotlib's `pyplot`.

### 4. Quartiles, Outliers, and Box Plot
- Identify the final tumor volume for each mouse in the four most promising drug regimens (Capomulin, Ramicane, Infubinol, Ceftamin).
- Calculate quartiles, interquartile range (IQR), and determine potential outliers.
- Generate a box plot to visualize the tumor volume distribution, highlighting outliers.

### 5. Line and Scatter Plots
- Line plot:
  - Show tumor volume changes over time for a mouse treated with Capomulin.
- Scatter plot:
  - Compare average tumor volume vs. mouse weight for Capomulin-treated mice.

### 6. Correlation and Regression
- Calculate and visualize correlation between mouse weight and tumor volume.
- Perform linear regression to analyze this relationship.

## Results
This analysis provides key insights into:
- The effectiveness of Capomulin compared to other drug regimens.
- Tumor volume trends over time for different treatments.
- Statistical significance of drug effects.


