# About 

I made a spreadsheet for tracking our monthly spend on groceries, but found the process for updating it to be tedious. 

So, I wrote a quick and dirty iOS Shortcut for adding new items.

# Setup
- Download the Numbers document template from this repo
- Save a new copy to your iCloud, name it whatever you want (default is "Budget.numbers")
- Add the [Shortcut](https://www.icloud.com/shortcuts/f6f39d41740e4175a7421a4e8eb21fb1) to your library, then (optionally) add it to your iPhone's home screen for easy access
- When you run the shortcut for the first time, select the .number document when prompted; then enter the specific sheet and table names (defaults are `Groceries` and `Transactions`)

# How it Works

When you run the shortcut:
- Choose the date on the receipt you're adding (default is today's date)
- Select the name of the store from the list
- Enter the total on the receipt (including tax)
- _*Optional:*_ if there are any non-food items on the bill (toiletries, household cleaning supplies, etc), enter their pre-tax total value

When you submit, a new row should be added to the TOP of the transaction history. Monthly and yearly breakdown fields should update automatically as you enter more data. 

The `Current Year` and `Previous Year` should automatically update. So on January 1st of each year, the values of the Current year should replace the previous year's data, which would in turn be discarded.

The "New Total" column is the receipt's total value minus the value of `Non-food total` _multiplied by 1.05 to account for tax_. Update the formula if your local tax is different.

# Apple Shortcut
You can grab the shortcut here, then add it to your iPhone's homescreen:
https://www.icloud.com/shortcuts/f6f39d41740e4175a7421a4e8eb21fb1

## Shortcut Changelog:
_Nov 11_: Initial release
