
# Sentiment Analysis of Nike Shoes Using Machine Learning: BERTopic  

## 📌 Project Overview  
This project analyzes consumer sentiment and market performance of **Nike’s sustainable vs. non-sustainable** footwear. Using **web scraping, statistical analysis, and BERTopic-based text clustering**, we explore customer preferences and their alignment with product descriptions.  

### 🔍 Key Insights  
- **Customer satisfaction** is primarily influenced by comfort and quality, **not sustainability labels**.  
- **Price and sustainability status** have **no significant impact** on consumer engagement (confirmed via t-tests & chi-square tests).  
- **BERTopic analysis** reveals that marketing descriptions closely align with actual customer reviews, indicating effective brand messaging.  

---

## 📂 Dataset  
- **Scraped Nike product data off the homepage**: Includes product IDs, prices, discounts, review counts, and ratings.  
- **Sustainable vs. Non-Sustainable Shoes**: Categorized based on Nike’s product descriptions.  
- **Customer Reviews**: Extracted using BeautifulSoup from Nike’s website.  

🗂 **Files in this repository:**  
- `Nike_Analysis.ipynb` → Full code for web scraping, preprocessing, and analysis.
- `dataset` → Folder containing all scraped data files (csv)
- `cleaned_non_sus_data.csv` → Cleaned dataset of non sustainable shoes used in this analysis.  
- `cleaned_sus_data.csv` → cleaned dataset of sustainable shoes.
- all other csv files under dataset  →  scraped raw data before preprocessing
- 'Project Report - Nike Shoes.pdf' → PDF version of full project report
---

## 📊 Methodology  
1. **Data Collection**:  
   - Used **BeautifulSoup** and Python to scrape Nike’s website for product info and reviews.  
   - Categorized products as **sustainable vs. non-sustainable**.
   - **sustainable** shoes were scraped from the sustainable shoe category.
   - **non sustainable** shoes were those left after excluding the sustainable shoes from all the shoe data. 

2. **Data Preprocessing**:  
   - Cleaned and tokenized text using **NLTK**.  
   - Applied **TF-IDF** for keyword extraction.  

3. **Statistical Analysis**:  
   - **T-test**: Compared average ratings of sustainable vs. non-sustainable shoes.  
   - **Chi-square test**: Analyzed differences in review engagement.  

4. **BERTopic Clustering**:  
   - Extracted **key topics** from customer reviews and product descriptions.  
   - Identified trends in consumer sentiment for both categories.  

---

## 📈 Results & Findings  
✔ **No significant difference** in customer satisfaction between sustainable and non-sustainable shoes.  
✔ **Customer sentiment topics** (from BERTopic analysis):  
   - **Sustainable shoes**: Comfort, recycled materials, innovation.  
   - **Non-sustainable shoes**: Classic styles, performance, comfort.  
✔ **Statistical tests confirm** that price and sustainability labels **do not** significantly impact customer engagement.

Customer sentiments focus on comfort and preference regardless of the shoe’s sustainability. Additionally, the alignment between consumer sentiment and product description was strong, suggesting that Nike’s product marketing strategies effectively resonate with consumers. 
The results suggest that Nike has the opportunity to enhance its investment in sustainable products, aligning more closely with environmental goals and consumer demand.


📊 **Visualization Examples:**  
Shown on the later pages of the project report as it's too much to show here

---

## 🚀 How to Use  
1. Clone this repository:  
   ```bash
   git clone https://github.com/thsdbswl606/Nike-Sentiment-analysis.git
   cd Nike-Sentiment-Analysis
