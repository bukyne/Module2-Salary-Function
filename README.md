# Module2-Salary-Function
To develop a Jupyter Notebook to create a function that retrieves employee details, exports them to a CSV file within a zipped folder, and uses R to unzip and display the data.

Description
This project processes employee salary data using Python and R. It includes functions to retrieve employee details, handle errors, export data to CSV file, Zip the file and then unzip the folder and display the data using R. The project integrates both Python and R code within a Jupyter Notebook.

Requirements
- Python 3.13
- Jupyter Notebook
- Required Python packages: pandas, csv, zipfile, rpy2
- R
- Required R packages: utils
- Dataset: I downloaded and renamed the file 'Salaries.csv' in my system directory - download from [Kaggle](https://www.kaggle.com/code/itshorus/sf-salary).

Installation
Python Packages
- In your command prompt, install the required Python packages using pip: pip install pandas rpy2
R Packages
- Install the required R packages using R console (I used R studio): 
install.packages('IRkernel')
IRkernel::installspec()


Instructions
1. Open Jupyter Notebook from Command Prompt using 'jupyter notebook'.
2. Create a new notebook and select the Python kernel.
3. Import Data: The dataset is loaded into a pandas DataFrame for easy manipulation. Load the dataset 
4. Create employee function: The function get_employee_details searches for an employee by name (case-insensitive) and returns their details as a list of dictionaries. If the name is not found, a ValueError is raised.
5. Data input: Created a variable to retieve employee name from user input; which will print the employee's details from the spreadsheet.
6. Data Processing with Dictionary: The data is processed to compute average salaries per job title, stored in a dictionary for quick lookup.
7. Error Handling: Errors are handled using try-except blocks to ensure the program exits gracefully and provides meaningful error messages.
8. Export Employee Details: Run the export_employee_details function to generate Employee Profile.zip. The employee details are exported to a CSV file, which is then compressed into a zip folder named "Employee Profile.zip".
9. Unzip and Display Data with R: Using R within the Jupyter Notebook, the zip file is extracted, and the CSV data is read and displayed. This requires the rpy2 extension to  run the R cell in the Jupyter notebook.

This approach ensures that each task is handled efficiently, with proper error checking and data processing, providing a comprehensive solution to the problem.


Troubleshooting
1. Missing Dependencies: Run pip install -r requirements.txt if provided.
2. File Not Found: Ensure Salaries.csv is in the project root.
3. Rpy2 Errors:
  -Install R before installing rpy2.
  -Add R to your system PATH.
4. Employee Not Found: Verify the name exists in Salaries.csv.
