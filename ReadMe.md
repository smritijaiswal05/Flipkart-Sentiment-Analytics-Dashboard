# Flipkart Product Reviews - Customer Sentiment Analytics Dashboard

## Project Overview
This repository contains an engineering-grade Data Analytics Major Project focusing on automated text sentiment mining and retail business intelligence pipelines. Using natural language processing (NLP), the system converts raw, unstructured textual data from Flipkart consumer reviews into structured categorical buckets (Positive, Negative, Neutral). 

Moving beyond basic aggregate counts, this workflow implements multi-variable statistical evaluation patterns—including text polarity variance mapping, metadata correlation analysis, and itemized product performance diagnostics—to isolate product pain points and core value drivers.

---

## Core Analytical Insights
Based on the processing of the provided `flipkart.csv` file (containing 2,304 clean entries), the system uncovers two layers of analytical insights:

### 1. Macro-Level Sentiment Distribution (Overview)
* **Positive Reviews:** 2,062 (89.5%)
* **Negative Reviews:** 156 (6.8%)
* **Neutral Reviews:** 86 (3.7%)
* *Observation:* The dataset shows a significant class imbalance with a strong positive bias. This standard e-commerce retail behavior is captured dynamically by the TextBlob analyzer.

### 2. Micro-Level Product Performance (Business Intelligence)
The script automates an internal SQL-style `groupby` operation to filter items with at least 5 reviews and rank them by the lowest average sentiment polarity. This isolates specific models with low customer satisfaction thresholds:
1. **realme C21Y (Cross Black/Blue):** Avg. Rating: **3.1 ★** | Calculated Polarity: **-0.3933** (Critical dissatisfaction)
2. **Redmi 9A (Sea Blue/Midnight Black/Nature Green):** Avg. Rating: **3.1 ★** | Calculated Polarity: **-0.1241** (Moderate dissatisfaction)

---

## Technology Stack & Dependencies
The pipeline is designed to execute entirely **offline and locally** without calling online APIs or downloading packages at runtime.
* **Core Environment:** Python 3.8+
* **Data Manipulation:** `pandas`
* **NLP & Text Lexicons:** `textblob`, `nltk` (Stopwords engine)
* **Visualization Layer:** `matplotlib`, `seaborn`
* **Textual Analytics Representation:** `wordcloud`

---

## Environment Setup & Installation

1. **Clone or navigate to the project directory:**
   ```bash
   cd path/to/your/project-directory