---
title: "KFC Store Locator Automation"
excerpt: "Web scraping and wrangling of KFC store locations in R. <br/><img src='/images/OIP.jpg'>"
collection: portfolio
---

This project was done while I was a freelance data analyst for a fintech company in Cape Town, 22Seven (subsdiary of Old Mutual). They are a personal digitial finance business that empowers customers to make better financial decisions and helps customers create personalised budgets to enable them to manage their money better from month to month, using an app. 

The objective of this project was to automate the extraction of KFC store locations in South Africa from the KFC website. It utilizes web scraping techniques through Selenium and data manipulation using Pandas to organize the information systematically.

**Key Components:**
1. Data Preparation:

The script begins by loading postal code data from an Excel file (*postalcodes.xls*). It extracts unique town names and formats them appropriately. A test subset (test) is created to validate initial data processing.

2. Web Scraping with Selenium:

Utilizes Chrome WebDriver to navigate to the KFC South Africa store locator [webpage](https://order.kfc.co.za/find-store). Iterates through each town, searching for KFC stores and extracting relevant information. The script employs explicit waits (time.sleep(2)) to ensure the webpage fully loads before extracting data.

3. Data Cleaning and Deduplication:

Duplicates in store names are removed to ensure a unique list. Extracted addresses are parsed to obtain provinces, cities, country codes, and exact addresses. Province names are standardized and capitalized for consistency.

4. Data Structuring:

The final results are structured into a Pandas DataFrame (*KFC*). Columns include store names, exact addresses, city names, provinces, and country codes.

5. Export to CSV:

The resulting DataFrame is exported to a CSV file (*KFC locations.csv*) for further analysis or integration with other systems.

**Noteworthy Techniques:**

Web Scraping: Utilizes Selenium for dynamic web page interaction, locating elements by XPath.
Data Cleaning: Applies various techniques to standardize and clean extracted data, including handling variations in province names.

**Dependencies:**

Pandas: Used for data manipulation and DataFrame creation.
Selenium: Employed for web scraping and automated interaction with the KFC store locator.

**Additional Considerations:**

The script requires the Chrome WebDriver (chromedriver.exe), and the path must be specified, and ensure the Excel file (*postalcodes.xls*) is present and accessible in the specified location.

*MEGA gratitude towards Simon Anderssen for taking a chance with me.*


