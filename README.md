# Automated GST Invoice Generator

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Input Format](#input-format)
- [Output Format](#output-format)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Introduction

The **Automated GST Invoice Generator** is a Python-based tool designed to streamline the process of generating GST tax invoices from ledger or bill details provided in an Excel sheet. This tool automates the invoice creation process, merging multiple invoices into a single PDF file for easy distribution and storage.

## Features

- **Batch Processing**: Generate multiple invoices at once from a single Excel sheet.
- **GST Compliance**: Invoices are generated according to GST regulations, ensuring compliance.
- **Merged PDF Output**: All generated invoices are merged into a single PDF file, making it convenient to share and store.
- **Customizable Templates**: Modify invoice templates to fit your branding and design needs.
- **User-Friendly Interface**: Simple command-line interface for ease of use.

## Getting Started

To get started with the Automated GST Invoice Generator, follow the steps below:

### Prerequisites

Make sure you have the following software installed on your system:

- Python 3.x
- pip (Python package installer)
- xlsxwriter
- openpyxl
- PyExcelerate
- PyPDF2

Here’s a brief overview of each library you mentioned, along with its primary use cases:

1. XlsxWriter
Description: XlsxWriter is a Python library for creating Excel .xlsx files. It allows you to write data to Excel files and has support for formatting, charts, and more.
Use Cases:
Creating complex Excel files with features like charts, formatting, and multiple worksheets.
Writing data programmatically to Excel, especially for reporting purposes.
Adding formulas, images, and other Excel-specific elements.
2. OpenPyXL
Description: OpenPyXL is a library to read and write Excel files in the .xlsx format. It is often used for modifying existing Excel files and is compatible with many Excel features.
Use Cases:
Reading data from existing Excel files for data analysis or report generation.
Modifying existing Excel files, such as updating values or formatting.
Accessing and editing various Excel features, such as styles, charts, and formulas.
3. PyExcelerate
Description: PyExcelerate is a fast library for writing Excel .xlsx files. It is optimized for speed and memory usage, making it suitable for large datasets.
Use Cases:
Writing large datasets to Excel files quickly and efficiently.
Simplifying the process of creating Excel files without the overhead of formatting and styling unless necessary.
Exporting data directly from databases or data processing tasks to Excel for reporting.
4. PyPDF2
Description: PyPDF2 is a library for working with PDF files in Python. It allows you to manipulate PDFs, including merging, splitting, and extracting text.
Use Cases:
Merging multiple PDF files into one, such as combining generated invoices into a single document.
Splitting a PDF file into separate pages or sections.
Extracting text, images, or metadata from PDF files for analysis or reporting.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/iamkrishnaagarwal/automated-bill-generator.git

### Input Format
The input Excel file should be structured with the following columns:

Invoice Number	Customer Name	Customer Address	Item Description	Quantity	Rate	GST Percentage	Total Amount
001	John Doe	123 Main St.	Product A	10	100	18%	1180
002	Jane Smith	456 Elm St.	Product B	5	200	18%	1180
Make sure the data is clean and formatted correctly for accurate invoice generation.

### Output Format
The output will be a merged PDF file containing all generated GST invoices, structured as follows:

Each invoice will include:
Invoice Number
Date of Issue
Seller's Details (Name, Address, GST Number)
Buyer's Details (Name, Address)
Itemized list of products/services
Total Amount with GST breakdown
Payment Terms
Dependencies
This project requires the following Python libraries:

XlsxWriter: For creating new Excel files with formatting and charts.
openpyxl: For reading and modifying existing Excel files.
PyExcelerate: For fast writing of large Excel files.
PyPDF2: For manipulating PDF files, including merging invoices.
You can install these dependencies using pip, as mentioned in the Installation section.

### Contributing
Contributions are welcome! If you have suggestions for improvements or want to add features, please fork the repository and create a pull request.

Fork the repository.
Create your feature branch (git checkout -b feature/AmazingFeature).
Commit your changes (git commit -m 'Add some AmazingFeature').
Push to the branch (git push origin feature/AmazingFeature).
Open a pull request.
