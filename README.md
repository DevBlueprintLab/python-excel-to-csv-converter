# 📄 Excel to CSV Converter

![Python Version](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Dependency](https://img.shields.io/badge/Dependency-openpyxl-orange)
![License](https://img.shields.io/badge/License-MIT-green)

A Python automation tool that converts Excel worksheets into clean CSV files while allowing users to select the desired worksheet and export data into an organized output folder.

---

# 🖥️ Demo

### Excel Workbook ➜ Worksheet Selection ➜ CSV Output

<p align="center">
  <img src="images/excel-input.png" width="380" alt="Excel input file" />
  <img src="images/conversion-process.png" width="380" alt="Conversion process" />
</p>

<p align="center">
  <img src="images/csv-output.png" width="765" alt="Generated CSV file" />
</p>

---

# 🎯 Problem

Excel workbooks are commonly used for storing and sharing structured data, but many systems and applications require CSV format instead.

Manually copying worksheet data into CSV files is repetitive and can introduce errors during the conversion process.

---

# ✅ Solution

This tool automates Excel-to-CSV conversion by:

- Loading Excel workbooks
- Allowing users to choose a worksheet
- Exporting worksheet data into CSV format
- Saving the converted file separately without modifying the original workbook

---

# ⚡ Core Features

- 📊 **Excel Worksheet Conversion**  
  Converts selected Excel worksheets into CSV files.

- 📑 **Multi-Sheet Workbook Support**  
  Allows users to choose which worksheet to export from workbooks containing multiple sheets.

- ✅ **Input Validation**  
  Checks that the provided Excel file exists before processing.

- 🛡️ **Error Handling**  
  Detects workbook loading issues and prevents failed conversions.

- 📂 **Organized Output Management**  
  Automatically creates a `converted` folder and saves generated CSV files separately.

- 📈 **Conversion Summary**  
  Displays the exported workbook name, selected worksheet, row count, and output location.

---

# 🛠️ Tech Stack

- **Language:** Python 3.x
- **Excel Processing:** `openpyxl`
- **CSV Processing:** Built-in `csv` module
- **File Handling:** `pathlib`

---

# 🚀 Quick Start

## 1. Clone the repository

```bash
git clone https://github.com/DevBlueprintLab/python-excel-to-csv-converter.git

cd python-excel-to-csv-converter
```

## 2. Install dependencies

```bash
pip install -r requirements.txt
```

## 3. Run the converter

```bash
python excel_to_csv.py
```

## 4. Select your Excel file and worksheet

Example:

```text
========================================
CSV Converter
========================================

Enter Excel file path: sales_report.xlsx

Available sheets:['Sales', 'Employees', 'Inventory']

Choose worksheet: Sales

-------------------
 Conversion completed.
-------------------

Workbook:
sales_report.xlsx

Worksheet:
Sales

Rows exported:
25

CSV saved at:
converted/sales_report.csv
```

---
# 📁 Project Structure

```text
python-excel-to-csv-converter/

├── excel_to_csv.py              # Main automation script
├── README.md                    # Project documentation
├── LICENSE                      # MIT License
├── requirements.txt             # Project dependencies
├── sample_data/
│   └── sales_report.xlsx        # Example Excel input file
└── images/
    ├── excel-input.png          # Excel workbook example
    ├── conversion-process.png   # CLI conversion process
    └── csv-output.png           # Generated CSV example
```

---

# 💼 Practical Use Cases

This automation tool can help with:

- Converting Excel reports into CSV format for importing into other systems
- Preparing spreadsheet data for analysis workflows
- Exporting specific worksheets from large workbooks
- Automating repetitive data transfer tasks

---
