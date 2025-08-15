# Web Scraping Task

This project was developed as part of a task assigned by the **Digital Egypt Pioneers Initiative (DEPI)**, under the **Ministry of Communications and Information Technology (MCIT), Egypt**.

The goal of this task was to perform web scraping on a target webpage to extract various types of data and store them in structured formats (CSV and JSON).

## 📌 Features
- Extract **Headings** (`h1`, `h2`)
- Extract **Paragraphs** (`p`)
- Extract **Lists** (`li`)
- Extract **Table data** (`tr`, `td`), grouped by rows
- Extract **Form field information** (field names, input types, default values)
- Extract **Video link**

## 🛠 Tools & Libraries
- **Python**
- `requests` – fetch webpage content
- `BeautifulSoup` – parse HTML and extract elements
- `csv` – store structured data in CSV files
- `json` – store extracted data in JSON format

## 📂 Output Files
**CSV Files**
1. `Extract_Text_Data.csv` – Combined extracted text in a structured table
2. `Extract_Table_Data.csv` – Extracted table data only

**JSON Files**
1. `Product_Information.json` – Book title, price, stock availability, and button text
2. `Form_Information.json` – Field name, input type, and default values
3. `Video_Link.json` – Video link

## 🚀 Approach
1. Sent an HTTP request using `requests` to fetch the HTML content.
2. Parsed the HTML using `BeautifulSoup` to locate target elements.
3. Extracted and cleaned the data (removing extra spaces and newlines).
4. Stored the data in multiple CSV and JSON files.

## ⚡ Challenges Faced
- Handling different HTML structures for headings, lists, tables, and forms.
- Extracting default values from form fields that may not always have a value.
- Grouping table cells correctly when saving in CSV/JSON formats.
- Cleaning and formatting text for consistency.
- Managing multiple output files without overwriting data.

---
