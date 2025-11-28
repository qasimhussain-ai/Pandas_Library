# Pandas_Library
pandas is a powerful Python library for working with structured data. It provides flexible data structures, tools for cleaning and transforming datasets, and high-level functionality for analysis and exploration. Built on top of NumPy, pandas makes it easy to load data from many formats, manipulate it efficiently, and perform common operations used in data science and analytics.

Features

DataFrame and Series structures
Intuitive, labeled data containers designed for tabular and time-series data.

Data loading utilities
Read and write data in CSV, Excel, JSON, SQL databases, Parquet, and more.

Data cleaning tools
Handle missing values, duplicates, type conversions, and reshaping.

Powerful indexing & selection
Label-based, position-based, and boolean indexing for flexible data access.

Grouping & aggregation
Group-by operations for summarization and statistical analysis.

Time-series functionality
Date indexing, resampling, rolling windows, and easy time-based slicing.

Integration-friendly
Works smoothly with NumPy, Matplotlib, scikit-learn, and other data libraries.

Installation
pip install pandas


or with conda:

conda install pandas

Basic Usage
import pandas as pd

# Creating a DataFrame
df = pd.DataFrame({
    "name": ["Alice", "Bob", "Charlie"],
    "age": [24, 30, 29]
})

# Inspecting data
print(df.head())
print(df.info())

# Selecting columns
ages = df["age"]

# Filtering
adults = df[df["age"] >= 25]

# Adding a column
df["is_adult"] = df["age"] >= 18

# Grouping
avg_age = df.groupby("is_adult")["age"].mean()

Common Tasks & Functions
Purpose	Functions
Load data	read_csv, read_json, read_excel, read_sql, read_parquet
Inspect data	head, tail, info, describe, shape
Clean data	dropna, fillna, drop_duplicates, astype
Select data	loc, iloc, boolean filters
Transform	apply, map, assign, rename, merge, concat
Time series	to_datetime, resample, rolling, shift
Project Links

Official site: https://pandas.pydata.org

Source code: https://github.com/pandas-dev/pandas

License

pandas is released under the BSD 3-Clause License.
