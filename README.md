# Assignment
The code imports necessary libraries such as NumPy, Pandas, SQLAlchemy, and PyMySQL.
The 'read_csv' function is used to read a CSV file named 'youtube_dataset.csv' into a Pandas DataFrame called 'df_youtube'.
The 'head' function is used to preview the first 5 rows of the 'df_youtube' DataFrame.
The 'info' function is used to display important information about the DataFrame, such as the column names, data types, and non-null count.
The 'df_first_1000_rows' DataFrame is created by selecting the first 1000 rows of the 'df_youtube' DataFrame.
A function named 'distribution' is defined to get the distribution of a specified column in a DataFrame.
The 'df_dist' DataFrame is created by calling the 'distribution' function with the 'df_first_1000_rows' DataFrame and the column name 'channeltype'.
The 'df_first_1000_rows' DataFrame is saved to a CSV file named 'youtube_top_1000.csv'.
An SQLAlchemy engine is created with the database connection details using the 'create_engine' function.
The 'df_10' DataFrame is created by selecting the first 10 rows of the 'df_first_1000_rows' DataFrame.
The 'df_10' DataFrame is then written to a MySQL database table named 'df_10' using the 'to_sql' function. The data types of the columns are specified using the 'dtype' parameter. If a table with the same name already exists, it will be replaced with the new data.
