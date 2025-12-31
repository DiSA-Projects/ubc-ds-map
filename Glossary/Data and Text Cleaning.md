
**Data cleaning** is the process of identifying and correcting errors, inaccuracies, and inconsistencies in a dataset to improve its quality. This involves detecting corrupt, incomplete, or improperly formatted data, then correcting, modifying, or deleting it to prepare the dataset for subsequent analysis. This process is sometimes referred to as **data preprocessing**.

## Data Cleaning Tools

If the dataset is relatively small or mostly error-free, then you might be able to clean the data by directly editing the CSV or Excel spreadsheet file. Many research projects, however, involve fairly large and frequently messy datasets that are composites or aggregates of other data sources or whose data was collected more informally or inconsistently.

### Microsoft Excel/Google Sheets

You can perform simple data cleaning tasks by opening the dataset as a spreadsheet in Microsoft Excel or Google Sheets. Both offer built-in features to remove duplicates, convert text into columns, trim extra spaces, and remove non-printable characters. Excel’s Power Query method allows for sophisticated queries for more complex or repeatable tasks. Although Google Sheets does not have Power Query, you can use QUERY to apply a subset of SQL to filter, sort, aggregate, and transform data within the dataset. Both Excel and Google Sheets provide dataset analysis tools within the spreadsheet to quickly identify and fix data issues in a sheet.

- [Data Cleaning in Excel](https://support.microsoft.com/en-us/office/top-ten-ways-to-clean-your-data-2844b620-677c-47a7-ac3e-c2e157d1db19)
- [SmartCleanup in Google Sheets](https://support.google.com/docs/answer/10098582?hl=en)

### Python

If the data cleaning tasks are more complicated or require a more complex set of instructions to correct, [[Python]] combined with the Pandas library may be a good option. Pandas provides powerful data structures like DataFrames and Series, as well as many functions for data manipulation.

You might also use RegEx (Python’s regular expressions library) if you need access to more pattern-matching tools and features, or NumPy, a library that extends your ability to work with numbers. You can use Python to handle missing values, remove duplicate entries, standardize data formats and types, handle outliers (find statistically or visually, then remove, cap, or transform them), and address inconsistent data (correcting typos, standardizing units, etc).

Python is a great solution for data that is not formatted for a spreadsheet (blocks of text, documents, etc), or for a data cleaning process that is based on context or particular conditions that might require multiple steps or more complicated programming.

- [Pandas Documentation](https://pandas.pydata.org/docs/user_guide/10min.html)
- [Data Cleaning with NumPy and Pandas (Kaggle)](https://www.kaggle.com/code/mejbahahammad/data-cleaning-with-numpy-and-pandas)

### OpenRefine

OpenRefine (formerly Google Refine) is a free open-source desktop application designed specifically to diagnose data quality and to perform data cleanup. It features a very user-friendly interface and, unlike working with Python, does not require extensive programming knowledge to use.

Unlike spreadsheet programs that are designed to work on individual rows and cells, OpenRefine can operate on large ranges of data at once and has many other features and functions, including tools that identify similar values as clusters and merge them (eg. cells with “homeowner”, “homeowners”, “home owner”, “home owners”, “hone owner” could have these values replaced with a standard “homeowner” value).

OpenRefine is built to work on datasets and regularly formatted text that can be converted into columns.

- [OpenRefine Documentation](https://openrefine.org/docs)
- [OpenRefine Screencasts](https://github.com/OpenRefine/OpenRefine/wiki/Screencasts)
- [OpenRefine Tutorials (list)](https://github.com/OpenRefine/OpenRefine/wiki/External-Resources)
- [Cleaning Data with OpenRefine (Programming Historian)](https://programminghistorian.org/en/lessons/cleaning-data-with-openrefine)