### CSV File Combiner
** This program reads in all CSV files in a given directory and combines them into a single file. It does so by matching the columns "ID" and "Date" in each file. If a new column is found in one of the files, it is appended to the combined file.
### Requirements
* Python 3.x
* pandas library
### Usage
* Place all CSV files you want to combine into a single directory.
* Update the directory variable in the code to match the directory containing your CSV files.
* Run the program using the command python csv_combiner.py.
* The combined CSV file will be saved in the same directory as the input files, with the filename combined.csv.
### Additional Features
* If multiple rows with the same ID are found, only the row with the latest date is kept.
* Null values are kept as NaN instead of 0.
* The combined file is sorted by ID and Date.
### Notes
* The first row of each CSV file is assumed to be the header row.
* All files in the directory with a .csv extension will be combined.
* Files with different column names for ID or Date will not be combined.