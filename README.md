# WebScrapping-Booksite
# WebScrapping-Booksite

A Python-based web scraper designed to extract information about books from the [Books to Scrape](https://books.toscrape.com) website. This script collects data such as book titles, prices, availability, and links to individual book pages and saves the results in Excel and CSV formats.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Dependencies](#dependencies)
6. [Output](#output)
7. [Troubleshooting](#troubleshooting)
8. [Contributors](#contributors)
9. [License](#license)

---

## Introduction
The **WebScrapping-Booksite** project is a simple yet robust script for scraping book details from the [Books to Scrape](https://books.toscrape.com) website. It navigates through all available pages, collects relevant data, and exports it to Excel and CSV formats for further analysis.

---

## Features
- Scrapes book information:
  - **Title**
  - **Price**
  - **Stock Availability**
  - **Book Page Links**
- Automatically handles pagination, continuing until the last page.
- Saves data in:
  - `books.xlsx` (Excel format)
  - `books.csv` (CSV format)
- Provides detailed progress updates in the console.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/WebScrapping-Booksite.git
   cd WebScrapping-Booksite
   ```
2. Install the required dependencies using pip:
   ```bash
   pip install requests beautifulsoup4 pandas
   ```

---

## Usage
1. Run the script:
   ```bash
   python scraper.py
   ```
2. The script will scrape book data across all pages of the website.
3. After completion, two files will be created in the project directory:
   - `books.xlsx`
   - `books.csv`

---

## Dependencies
The script requires the following Python libraries:
- **requests** - For making HTTP requests.
- **beautifulsoup4** - For parsing HTML content.
- **pandas** - For handling tabular data and exporting it to Excel/CSV.

Install them using the command:
```bash
pip install requests beautifulsoup4 pandas
```

---

## Output
The scraped data will be saved in:
- **Excel File**: `books.xlsx`
- **CSV File**: `books.csv`

### Columns in the Output:
- **Title**: The title of the book.
- **Price**: The price of the book.
- **Stock**: Stock availability.
- **Link**: URL to the book's page.

---

## Troubleshooting
- **Empty Excel/CSV files**: Ensure that the target website ([Books to Scrape](https://books.toscrape.com)) is accessible and the URL structure hasn't changed.
- **404 Not Found Errors**: The script stops scraping when it encounters a non-existent page. Verify the website structure if issues persist.
- **Missing Dependencies**: Install the required libraries using:
  ```bash
  pip install requests beautifulsoup4 pandas
  ```

---

## Contributors
- **Your Name** - Developer and maintainer of this project.

Contributions are welcome! Feel free to fork the repository, submit pull requests, or report issues.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

### Example Console Output
```plaintext
Currently scrapping page: 1
In stock
In stock
Currently scrapping page: 2
In stock
...
```

Happy scraping! 🎉
