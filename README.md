# 🏦	 PyBank & PyRamen with Python

## 1. PyBank

Your task is to create a Python script that analyzes the [records](/PyBank/DataFolder/budget_data.csv) to calculate each of the following:

* The total number of months included in the dataset.

* The net total amount of Profit/Losses over the entire period.

* The average of the changes in Profit/Losses over the entire period.

* The greatest increase in profits (date and amount) over the entire period.

* The greatest decrease in losses (date and amount) over the entire period.

## 2. PyRamen 
* Opening a ramen shop has always been your dream, and now it's finally been realized––you're closing out on your second year of sales! Like last year, you need to analyze your business's financial performance by cross-referencing your sales data with your internal menu data to figure out revenues and costs for the year.

* This year, you also want to analyze how well your business did on a per-product basis (as you have several choices of ramen) in order to better understand which products are doing well, which are doing poorly, and, ultimately, which products may need to be removed or changed.
* * Write out the contents of the `report` dictionary to a text file. The report should output each ramen type as the keys and `01-count`, `02-revenue`, `03-cogs`, and `04-profit` metrics as the values for every ramen type as shown:

  ```
  spicy miso ramen {'01-count': 9238, '02-revenue': 110856.0, '03-cogs': 46190.0, '04-profit': 64666.0}
  tori paitan ramen {'01-count': 9156, '02-revenue': 119028.0, '03-cogs': 54936.0, '04-profit': 64092.0}
  truffle butter ramen {'01-count': 8982, '02-revenue': 125748.0, '03-cogs': 62874.0, '04-profit': 62874.0}
  tonkotsu ramen {'01-count': 9288, '02-revenue': 120744.0, '03-cogs': 55728.0, '04-profit': 65016.0}
  vegetarian spicy miso {'01-count': 9216, '02-revenue': 110592.0, '03-cogs': 46080.0, '04-profit': 64512.0}
  shio ramen {'01-count': 9180, '02-revenue': 100980.0, '03-cogs': 45900.0, '04-profit': 55080.0}
  miso crab ramen {'01-count': 8890, '02-revenue': 106680.0, '03-cogs': 53340.0, '04-profit': 53340.0}
  nagomi shoyu {'01-count': 9132, '02-revenue': 100452.0, '03-cogs': 45660.0, '04-profit': 54792.0}
  soft-shell miso crab ramen {'01-count': 9130, '02-revenue': 127820.0, '03-cogs': 63910.0, '04-profit': 63910.0}
  burnt garlic tonkotsu ramen {'01-count': 9070, '02-revenue': 126980.0, '03-cogs': 54420.0, '04-profit': 72560.0}
  vegetarian curry + king trumpet mushroom ramen {'01-count': 8824, '02-revenue': 114712.0, '03-cogs': 61768.0, '04-profit': 52944.0}
  ```

## 3. Results.

* [PyBank](/PyBank/) (Required)
    * [Python Code](/PyBank/main.ipynb)
    * [Exported results](/Output/pybank_analysis.txt) 
* [PyRamen](/PyRamen/) (Optional)
    * [Python Code](/PyRamen/main.ipynb)
    * [Exported results](/PyRamen/Output/)

