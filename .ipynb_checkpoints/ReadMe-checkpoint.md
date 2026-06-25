# Customer Sentiment Analysis on Flipkart Product Reviews

## 📌 Project Overview
This project focuses on exploring and analyzing customer reviews from Flipkart to understand consumer sentiment and purchasing behaviors. Utilizing Python-based Natural Language Processing (NLP) workflows, the pipeline handles text cleaning, removes structural data anomalies, parses literal reviews, and assigns distinct sentiment buckets (Positive, Negative, Neutral) mapped closely against actual user star ratings.

## 📊 Dataset Specifications
The pipeline utilizes an source-ingested dataset file named `flipkart.csv` consisting of **2,304 rows** and the following target features:
* **Product_name:** Identity information of the laptop/device bought.
* **Review:** Literal customer feedback text regarding performance or quality.
* **Rating:** Numeric satisfaction tracking metric score ranging across 1 to 5 stars.

## 🛠️ Technology Stack & Libraries
* **Language:** Python
* **Data Core:** Pandas
* **NLP Engines:** NLTK, TextBlob
* **Data Visualization:** Matplotlib, Seaborn

## 🚀 Quick Setup & Execution

1. **Clone the project repository or open your working environment directory:**
```bash
   cd path/to/your/project/folder
