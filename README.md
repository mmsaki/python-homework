# PyBank & PyRamen with Python

## 1. PyBank 💰

* Your task is to create a Python script that analyzes the [records](./PyBank/Resources/budget_data.csv)
   * To run this code you would need `pathlib` and `csv` libraries
   * Calculate total number of months and Profit/Losses included in the dataset. 
        * First create empty lists to append our data 
    ```python
    # Create empty 'month_list' and 'profit_list' list
    month_list = [] 
    profit_list = []

    # Create 'total_months' and 'total_profits' variables and set to 0
    total_months = 0 
    total_profits = 0
    ```
   * Read the the data and iterate through it using a for loop
   ```python
   # Open budget_data.csv
   with open(budget_path, newline="") as csvfile:
    # Read budget data
    csvreader = csv.reader(csvfile, delimiter=",")
    # Skip the header
    csv_header = next(csvreader) 
    
    # Using loop, slice the rows in data and append to our empty lists and add rows to 'total_months' and 'total_profits'
    for row in csvfile:     
        month_list.append(row[:8])
        profit_list.append(row[9:]) 
        total_months +=len(row[0]) 
        total_profits += int(row[9:])
   ```
   * Calculate average of the changes in Profit/Losses over the entire period.
    ```python
    # Set variable 'change_in_pnl' to store change in profits and losses list 
    change_in_pnl = [int(current_month) - int(previous_month) for previous_month, current_month in zip(profit_list, profit_list[1:])] 

    # Sort the change in Profits/Losses 
    change_sorted = sorted(change_in_pnl) 
    average = round(sum(change_in_pnl)/len(change_in_pnl),2)   
    ```
   * The greatest increase and decrease in profits (date and amount) over the entire period.
    ```python
    # Set variables for the greatest profit month and the loss month using our sorted list
    profit_month = change_in_pnl.index(change_sorted[-1]) + 1
    loss_month = change_in_pnl.index(change_sorted[0]) + 1 
    ```

## 2. PyRamen 🍜
* Opening a ramen shop has always been your dream, and now it's finally been realized––you're closing out on your second year of sales! Like last year, you need to analyze your business's financial performance by cross-referencing your [sales data](./PyRamen/Resources/sales_data.csv) with your internal [menu data](./PyRamen/Resources/menu_data.csv to figure out revenues and costs for the year.
    * Write out the contents of the `report` dictionary to a text file. The report should output each ramen type as the keys and `01-count`, `02-revenue`, `03-cogs`, and `04-profit` metrics as the values for every ramen type.


## 3. Results
* [PyBank](./PyBank/) (Required)
    * [Python Code](./PyBank/main.ipynb)
    * [Exported results](./PyBank/Output/pybank_analysis.txt) 
* [PyRamen](./PyRamen/) (Optional)
    * [Python Code](./PyRamen/main.ipynb)
    * [Exported results](./PyRamen/Output/ramen_report.txt)

