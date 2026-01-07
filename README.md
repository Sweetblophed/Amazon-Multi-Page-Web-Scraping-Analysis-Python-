# Amazon Multi-Page Web Scraping Analysis Python
This project demonstrates how to scrape multiple pages of Amazon search results using Python in Google Colab, extract product information, and perform basic data cleaning and analysis. 

The goal is to showcase web scraping fundamentals, pagination handling, and data analysis skills for educational purposes.

---
**⚠️ Disclaimer:**
This project is for educational and research purposes only. Amazon’s Terms of Service discourage automated scraping. No data is used commercially.


---
**🎯 Objectives**

Scrape product data from multiple Amazon search result pages

Handle pagination programmatically

Extract key product attributes

Clean and structure scraped data

Export data for analysis

Demonstrate ethical scraping awareness

---
**🧰 Tools & Technologies**

- Python

- Google Colab

- Requests

- BeautifulSoup (bs4)

- Pandas

- fake-useragent

- lxml

---
**📂 Project Structure**
amazon-web-scraping/
│
├── amazon_scraping.ipynb        # Google Colab notebook
├── amazon_multi_page_data.csv   # Scraped dataset
├── README.md                    # Project documentation

----
**🌐 Data Source**
Website: Amazon search result pages

Example URL pattern:

https://www.amazon.com/s?k=wireless+earbuds&page=1
---
**🔍 Data Extracted**

For each product, the following attributes are collected:

Product Name

Price

Rating
---
**⚙️ Methodology**
1. HTTP Requests with Headers

To reduce blocking, requests are sent with randomized User-Agent headers to mimic real browser behavior.

2. Pagination Handling

Amazon pagination is handled by dynamically appending a page parameter to the base search URL.

3. HTML Parsing

Page content is parsed using BeautifulSoup

Product containers are identified using Amazon’s HTML attributes

4. Polite Scraping

Random delays (3–7 seconds) are added between requests

Limited number of pages scraped to reduce server load
---
**🧹 Data Cleaning**

Prices are converted from strings to numeric format

Missing values are handled gracefully

Final dataset is structured using Pandas DataFrame
---
**📊 Sample Analysis**

Basic exploratory analysis includes:

Price distribution

Rating frequency

Product count per page

Example:

df.describe()
---
**📁 Output**

Scraped data is saved as:

amazon_multi_page_data.csv
---
**⚠️ Challenges & Limitations**

- Amazon actively blocks bots (503 errors, CAPTCHA)

- HTML structure may change over time

- Scraping reliability is not guaranteed
---
**✅ Ethical Considerations**

- No login or authentication used

- Minimal requests sent

- Scraping conducted strictly for learning purposes

- For production use, official APIs or licensed datasets are recommended
---
**🔄 Recommended Alternatives**

- Amazon Product Advertising API

- Kaggle Amazon datasets

- Web scraping practice websites
---
**🚀 Future Improvements**

- Add product review count

- Scrape additional attributes (brand, availability)

- Implement Selenium for dynamic pages

- Integrate proxy rotation

- Perform advanced data visualization
  
---
**👤 Author**

Adewuyi Blophed
Data Analyst | Python | Web Scraping | Data Visualization

---
**⭐ Acknowledgement**

This project is inspired by the need to understand real-world data collection challenges in web scraping.
