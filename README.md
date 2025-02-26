# **Web Scraping Project: Quotes Scraper**

## **Overview**
This project demonstrates how to efficiently scrape quotes, authors, and tags from the ["Quotes to Scrape"](http://quotes.toscrape.com) website using Python. The script, `scrape_quotes.py`, handles pagination, manages errors, and saves the extracted data into a CSV file for further analysis.  

This project is a great example of how web scraping can be used to gather structured data from websites, showcasing skills in HTTP requests, HTML parsing, and data management.

---

## **Project Structure**
```
web-scraping/
├── scrape_quotes.py        # Main script for scraping quotes
├── data/
│   └── quotes.csv          # Output CSV file with scraped quotes
├── README.md               # Project documentation
└── requirements.txt        # Required Python packages
```

---

## **Features**  
### **1. Data Extraction**  
The script extracts the following details for each quote:  
- **Quote**: The text of the quote.  
- **Author**: The person who authored the quote.  
- **Tags**: Keywords associated with the quote.  

### **2. Pagination Handling**  
The script automatically navigates through all pages of the website by following the "Next" button, ensuring comprehensive data collection.  

### **3. Error Handling**  
- **Retry Mechanism**: Automatically retries failed requests with exponential backoff.  
- **Error Reporting**: Provides clear error messages for connection issues or parsing errors.  

### **4. Output**  
The collected data is saved in a structured CSV file (`quotes.csv`) located in the `data` directory, making it easy to analyze or use in other applications.  

---

## **Setup**  
### **Prerequisites**  
Ensure you have the following Python packages installed:  
- `pandas==1.3.3`  
- `requests==2.26.0`  
- `beautifulsoup4==4.10.0`  

Install the dependencies using:  
```bash
pip install -r requirements.txt
```

---

## **Usage**  
1. **Clone the Repository**:  
   ```bash
   git clone https://github.com/DataAnalysisHub/owurakwarteng/web-scraping.git
   cd web-scraping
   ```

2. **Run the Script**:  
   Navigate to the `scripts` directory and execute the script:  
   ```bash
   cd scripts
   python scrape_quotes.py
   ```

3. **Check the Output**:  
   - The script will print each quote, author, and tag to the console.  
   - The complete dataset will be saved in `data/quotes.csv`.  

---

## **Troubleshooting**  
- **Connection Errors**: Ensure your internet connection is stable. The script includes retry logic to handle temporary issues.  
- **Parsing Errors**: If the website’s structure changes, update the parsing logic in the script accordingly.  

---

## **Contributing**  
Contributions are welcome! If you have suggestions or improvements, please:  
1. Fork the repository.  
2. Create a new branch:  
   ```bash
   git checkout -b feature/your-feature-name
   ```  
3. Commit your changes:  
   ```bash
   git commit -m "Add your commit message here"
   ```  
4. Push to the branch:  
   ```bash
   git push origin feature/your-feature-name
   ```  
5. Submit a pull request.  

---

## **License**  
This project is licensed under the **MIT License**. See [LICENSE](LICENSE.md) for details.
