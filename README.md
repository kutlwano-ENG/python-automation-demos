# Python Automation Demos

A collection of Python automation scripts for common Excel and CSV data tasks.
Built to demonstrate practical data processing skills for freelance work.

---

## Scripts

### `csv_cleaner.py` — Excel & CSV Data Cleaner

Automates the most common spreadsheet cleaning and reporting tasks in one command.

**What it does:**
- Removes duplicate rows
- Fixes inconsistent text formatting (whitespace, capitalisation)
- Parses and standardises date columns
- Sorts data by any column
- Filters rows by keyword or value
- Generates a formatted Excel report with a summary sheet

**Requirements:**
```bash
pip install pandas openpyxl
```

**Usage:**
```bash
# Basic clean
python csv_cleaner.py --input your_file.csv --output clean_report.xlsx

# With sorting and filtering
python csv_cleaner.py --input your_file.csv --output clean_report.xlsx --sort "Date" --filter-col "Status" --filter-val "Active"
```

**Demo — run with the included sample data:**
```bash
python csv_cleaner.py --input sample_data/sales_dirty.csv --output sample_data/sales_clean.xlsx --sort "Date" --filter-col "Status" --filter-val "Active"
```

**Example output:**

The script produces a two-sheet Excel workbook:

| Sheet | Contents |
|---|---|
| Clean Data | Fully cleaned, sorted, filtered data with formatted headers |
| Summary | Row count, duplicates removed, numeric column stats |

---

## About

Scripts written by an Electrical & Electronic Engineering student at the University of Cape Town.
Available for freelance Python automation work on Fiverr.

---

## License
NON.
