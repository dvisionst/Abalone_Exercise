# Abalone_Exercise


The abalone.data file contains the data and can be read in with pd.read_csv().  abalone.data does not have a header that stores the column names like the data we've been using so far.  You can tell Pandas that the first row is NOT column names by adding the argument: header=None.

You will notice that there are no column names in the .data file.  The column names can be found in a separate file called abalone.names which is a plain text file that stores metadata (information about the dataset).  Use a text editor to open this file and find the names that correspond to the columns in your dataframe.  You will need to type names into your code by hand to change the column names.





Prepare the Abalone Dataset for Modeling
The rings column will be your target column.

Note: Similar to trees, the number of rings for Abalone can be used to determine the age.  



Tasks:
1) Separate your data into the features matrix (X) and target vector (y).

2) Train/test split the data. Please use the random number 42 for consistency.

3) Create a ColumnTransformer to preprocess the data. Remember to:

    a) Create column selectors for the numeric and categorical columns

    b) Create a OneHotEncoder for one-hot encoding the categorical columns

    c) Create a StandardScaler for scaling numeric columns

    d) Match each transformer with the appropriate selector in a tuple

    e) Use the tuples to create a ColumnTransformer to preprocess the data.

4) Transform your data and display the result.
