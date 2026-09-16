# Veda-Technology
# Task 9 
Internship task for Veda Technology (Data Analytics track, Level 1, Day 9).

## About

This task is about calculating and understanding basic descriptive statistics - mean, median, mode, standard deviation, and percentiles - for a dataset. The goal was to see what these numbers actually tell us about a dataset, not just calculate them.

## Dataset

Used the Iris dataset. It has 150 rows and 5 columns:
- sepal_length
- sepal_width
- petal_length
- petal_width
- species (setosa, versicolor, virginica)

## Tools Used

- Python
- Pandas
- Google Colab

## What I Did

1. Loaded the dataset and checked for missing values using `df.info()`
2. Calculated summary statistics (mean, median, std, percentiles) for the 4 numeric columns using `df.describe()`
3. Calculated mode separately using `df.mode()`
4. Grouped the data by species using `groupby()` to compare the three flower types
5. Wrote up what the numbers showed about skew and spread

## What I Found

Sepal length and sepal width had mean, median and mode values close to each other, so their distribution is fairly symmetric.

Petal length and petal width showed a bigger gap between mean, median and mode. At first this looked like skewed data, but after grouping by species it turned out the gap was because the three species (setosa, versicolor, virginica) have very different petal sizes. So it wasn't really skew, it was three different groups mixed into one column.

Main takeaway: if mean, median and mode look very different for a column, check if there are hidden categories in the data before assuming the data is skewed.

## Files

- `iris.csv` - dataset used
- `Veda_Technology_Task9.ipynb` - Colab notebook with all the code and outputs
- `Task9_Descriptive_Statistics_Akshat_Srivastava.pdf` - final report submitted for the task
