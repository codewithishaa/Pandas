1)Pandas_Basics.ipynb
-A Jupyter Notebook demonstrating core Pandas functions:

-Importing Pandas (import pandas as pd)

-Reading CSV (pd.read_csv)

-Inspecting DataFrames (.head(), .tail(), .info(), .describe(), .dtypes)

-Saving to CSV (df.to_csv with custom delimiter/columns/no‐header options)

-Column Selection & Series vs. DataFrame (df['col'], df[['col1','col2']])

-Reading HTML Tables (pd.read_html from a URL)

-JSON → DataFrame (parsing JSON strings or API responses)

-API Calls (e.g., GitHub Issues via requests.get, converting JSON to DataFrame)

-Writing Extracted Tables (looping over scraped/parsed DataFrames → CSV)

-String/List Columns & Broadcasting (splitting, expanding lists, adding constant columns)

-Example Data Used:

IPLData.csv (21 columns, ~150K rows of ball‐by‐ball cricket data)

-HTML tables from Basketball Reference player pages

-A simple JSON string (nested list → DataFrame)

-Live GitHub API pull (Pandas repo issues)

2)Pandas_DataManipulation.ipynb
-A Notebook on advanced data manipulation in Pandas:

-Loading Data (pd.read_csv of Titanic dataset)

-Inspecting & Summarizing (.head(), .columns, .dtypes, .describe())

-Handling Missing Values (.isnull(), .dropna(), .fillna())

-Indexing & Selection (.loc[], .iloc[], boolean masks)

-Creating/Modifying Columns (arithmetic, .assign(), mapping)

-GroupBy & Aggregation (df.groupby().sum(), .describe())

-Concatenation & Merge/Join (pd.concat, pd.merge, .join)

-Reshaping Basics (stack/unstack examples)

-Example Data Used:

Titanic passenger data (survival, class, age, fare, etc.)


