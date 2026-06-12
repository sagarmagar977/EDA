# EDA Project 1

## Data Preparation

- Load the given dataset into a Pandas DataFrame.
- Provide a brief overview of the dataset, including:
  - Total number of rows.
  - Total number of columns.
- List all column names and identify their data types:
  - Numerical
  - Categorical
  - Datetime
- Identify the target variable, if one exists in the dataset.
- Explain what the dataset represents in 2-3 sentences.
- Describe why the dataset is suitable for an Exploratory Data Analysis (EDA) project.
- Summarize any notable characteristics of the dataset that may be useful for further analysis.

## Data Cleaning

### Identify Missing Values

- Check every column in the dataset for missing or null values.
- Calculate and report the percentage of missing data in each affected column.
- Select an appropriate treatment method for each column and justify your choice:
  - Drop rows if only a small number of records are affected.
  - Replace missing numerical values with the mean or median, depending on the data distribution.
  - Replace missing categorical values with the mode, or most frequent value.
- Explain why the chosen method is suitable for preserving data quality.

### Detect and Remove Duplicate Records

- Identify any duplicate rows in the dataset.
- Remove all duplicate entries.
- Report:
  - Number of duplicate rows found.
  - Number of duplicate rows removed.
  - New dataset shape, in rows x columns, after duplicate removal.

### Detect and Handle Outliers

- Select at least two numerical columns for outlier analysis.
- Use the Interquartile Range (IQR) method to detect outliers.
- For each selected numerical column:
  - Report the lower and upper bounds.
  - State the number of outliers detected.
  - Explain the chosen treatment:
    - Remove the outliers.
    - Cap the extreme values.
    - Retain them if they represent legitimate observations.
  - Justify the decision based on the dataset context.

### Summary of Data Cleaning

- Provide a short paragraph summarizing all preprocessing activities, including:
  - How missing values were handled.
  - Number of duplicate records removed.
  - How outliers were treated.

## Analysis and Insights

### Single Column Analysis

- Pick one numerical column from the cleaned dataset.
- Create a histogram or box plot to show how the values are distributed.
- Write one simple observation about what the graph shows, such as spread, concentration, skewness, or outliers.
- Pick one categorical column from the dataset.
- Create a bar chart showing how often each category appears.
- Write one observation about which category is most common and which is least common.

### Relationship Between Two Columns

- Create a correlation heatmap for all numerical columns using Seaborn.
- Find the two columns that are most strongly related, ignoring self-correlation.
- Report:
  - The names of both columns.
  - The correlation value.
  - A simple explanation of what this relationship means in real terms.
- Choose any two columns and show their relationship using:
  - A scatter plot.
  - A grouped box plot.
  - A table, or crosstab.
- Write one observation about the pattern or trend you notice.

### Looking at Multiple Columns Together

- Create a pair plot using at least three columns.
- Look at how the columns behave together in different combinations.
- Describe one interesting pattern or grouping that only becomes visible when looking at all selected columns together.
- Explain why this insight is useful for understanding the dataset.

### Summary of Findings

- Write a short paragraph summarizing:
  - What you noticed in the single-column analysis.
  - The strongest relationship between two columns.
  - The key pattern found when looking at multiple columns together.
  - What these results tell you about the dataset overall.

## Conclusion

### Key Findings

- The distribution of the selected numerical variable showed some extreme values, as seen in the histogram or other diagram, indicating the presence of outliers.
- The correlation heatmap revealed a strong relationship between two numerical variables, suggesting one could help predict the other in a modelling context.
- The categorical bar chart showed an uneven distribution, where one category was significantly more frequent than others, indicating possible class imbalance.

### Data Quality Assessment

- Some assumptions were made while handling missing values using mean, median, or mode, which may slightly affect accuracy.
- Decisions made during outlier handling, such as removing or capping values, could influence future model performance.
- Overall, the dataset is cleaner but still carries minor risks from imputation and imbalance.

### Possible Machine Learning Questions

- Can the target variable be predicted using the most strongly correlated features?
  - Strong correlations suggest useful predictive relationships between variables.
- Can the dataset be used to classify records into categories based on numerical patterns?
  - Visible patterns in distributions suggest separable groups.

### Final Verdict

- The dataset is mostly ready for modelling, but additional steps like feature scaling, handling class imbalance, and validating preprocessing assumptions are recommended before building a machine learning model.

# EDA Project 2

Choose any dataset of your interest from a public source such as Kaggle or another free source. It must have at least 500 rows and a mix of numerical and categorical columns.

Perform a complete Exploratory Data Analysis covering data preparation, cleaning, analysis, and conclusion, following the same structure and requirements from the previous assignment. Justify every decision you make.
