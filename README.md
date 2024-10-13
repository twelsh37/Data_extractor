# extract_column.py

This sis a simple utility that extracts a particular column of data fromk a csv or xls* file.

## Usage
You need python on your device to run this code. It is easily involed on the command line

```
python extract_column.py -h
```
This command displays the available comand line arguments
```
python extract_column.py -h
usage: extract_column.py [-h] (-c CSV | -e EXCEL)

Extract column data from CSV or Excel files.

options:
  -h, --help            show this help message and exit
  -c CSV, --csv CSV     Read CSV file
  -e EXCEL, --excel EXCEL
                        Read Excel file
```

## Running the file
invoking the program using any of the comand line arguments will parse a file with data and extract the column you are interested in.

Let us work through a simple example. I have provided two sample data files with the code.
here is the contents of the test-data-1.csv file

![image](https://github.com/user-attachments/assets/7d1ee460-45e9-4d35-b5ba-e74cb3021a42)

Running the utility against this file we use the following command line

```
python extract_column.py -c test-data-1.csv
```
The program will then list the headers in the file along with a corresponding number to indicate your choice.

```
python extract_column.py -c test-data-1.csv
Available headers:
1. id
2. first_name
3. last_name
4. email
5. gender
6. ip_address

Enter the number of the header you want to extract (1-6): 4
```

Select the header you are interested in , in our case we are interested in teh email address field, option 4.
hitting return will provide you a list of email addrsses on screen

![image](https://github.com/user-attachments/assets/03fc8156-8fa4-46e4-a207-0542efbd2118)


