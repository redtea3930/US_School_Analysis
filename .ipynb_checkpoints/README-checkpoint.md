# US School Analysis
This project uses data on public schools in the USA to demonstrate several techniques in the pandas python library, including :
* data importation and dataframe creation
* calling data by column and row values
* manipulation of  columns and rows
* concatenation 
* data cleaning
* plotting:
    - histograms
    - box plots
    - bar chart
    - scatter plots
    - pie charts
## Data Importation and DataFrame assembly
* Provided csv files are read from filepath, and imported as DataFrames
* Meaning of column names is determined by calling on row values of provided 'dictionary' dataframe against column names in a seperate DataFrame
* Unique identifiers are found for rows in each of two dataframes, which are then concatenated into one.
* Index is reset to unique identifiers and columns are renamed for better legibility.
## Data Cleaning
#### Nulls
* Nulls in dataframe are identified, and analyzed to determine how to treat them.
* Nulls that can be safely changed to 0 are filled, rows with nulls representing potentially bad data are discarded
#### Outliers
* histograms and box plots are used on several values to find and outliers
* conditional statements are used to remove rows with outlier values
## Data Analysis and Plotting
* Geographic plot of schools is contstructed from lattitude/longitude data
* Anomalies are used to review data cleaning process and determine if valid data was removed
* Correlation plot from Seaborn library used to find correlations between dataframe columns
* Groupby analysis is used to group school values by state 
* Bar chart of state mean school teacher ratio, sorted by decreasing ratio
* Additional scatterplot of O'ahu schools by level and pie chart of O'ahu student body demographic data 