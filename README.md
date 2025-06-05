File 1. Pandas_Basics.ipynb
A Jupyter Notebook that walks through fundamental Pandas operations step by step.
2. Topics Covered
2.1. Importing Pandas
    • How to import the Pandas library into your Python environment (import pandas as pd).
2.2. Reading CSV Data into a DataFrame
    • Using pd.read_csv() to load data from CSV files.
    • Handling delimiters, headers, and encoding when reading CSVs.
2.3. Displaying and Inspecting DataFrame Contents
    • .head() and .tail() – viewing the first or last N rows.
    • .info() – summary of column data types and non-null counts.
    • .describe() – statistical summary (mean, std, min, max, quartiles).
    • .dtypes – checking each column’s data type.
2.4. Saving a DataFrame to CSV
    • df.to_csv() – exporting a DataFrame to a CSV file.
    • Custom delimiters (e.g., sep='|').
    • Selecting specific columns to write.
    • Disabling headers or index in the output CSV.
2.5. Selecting Columns & Working with Series vs. DataFrame
    • Accessing single columns as a Series (df['column_name']).
    • Slicing multiple columns to form a smaller DataFrame.
    • Understanding differences between Series (1D) and DataFrame (2D).
2.6. Reading HTML Tables from a URL
    • pd.read_html(url) – scraping all tables from a webpage into a list of DataFrames.
    • Example: loading NBA player statistics from “Basketball Reference.”
2.7. Converting JSON‐Formatted Strings or Web API Responses
    • Using Python’s built-in json module to parse JSON into Python dictionaries/lists.
    • pd.json_normalize() (or pd.DataFrame()) to convert nested JSON to a flat DataFrame.
    • Example: converting a simple JSON string of user details (name, phone, company list) into a DataFrame.
2.8. Fetching Data from a Public API and Parsing JSON
    • Using requests.get() to call a REST API (e.g., GitHub Issues API).
    • Parsing the returned JSON and converting it into a DataFrame.
    • Example: fetching open issues from the Pandas GitHub repository.
2.9. Writing Extracted Tables to CSV Files
    • Looping over scraped/parsed DataFrames and writing each to a separate CSV with df.to_csv().
    • Naming conventions and file organization.
2.10. Working with String Columns, List‐Based JSON, & Broadcasting Scalars
    • Manipulating string data in columns (e.g., splitting, stripping, case conversion).
    • Expanding list‐type columns into separate rows or columns.
    • Broadcasting a scalar value across a new column for all rows.
3. Example Datasets Used in the Notebook
3.1. IPLData.csv
    • Ball-by-ball match data covering 21 columns and approximately 150,460 rows.
    • Used to demonstrate reading large CSVs, inspecting data, and basic cleaning steps.
3.2. HTML Tables from “Basketball Reference”
    • Example: loading player statistics tables via pd.read_html().
    • Demonstrates web scraping of tabular data without manual copy-paste.
3.3. Simple JSON String
    • A contrived JSON example, e.g.:
    ```json
{
"name": "Isha",
"phone_no": 45454545,
"comp": ["Google", "EY", "Unilever"]
}
