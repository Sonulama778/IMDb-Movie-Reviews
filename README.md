# 🎬 IMDb Movie Reviews – Web Scraping, Cleaning & Preprocessing

This project demonstrates how to build an end-to-end data pipeline to extract, clean, and preprocess IMDb movie metadata. The data was collected from the IMDb Top 250 movies list and transformed into a structured, analysis-ready format.

## 📦 Project Structure

IMDb-Movie-Reviews/
├── Milestone 1.ipynb # Web scraping with requests + BeautifulSoup
├── Milestone 2.ipynb # Data cleaning, normalization, encoding
├── cleaned_top_IMDB_db.csv # Final cleaned dataset (250 records)
├── README.md # Project documentation (this file)


## 🚀 Getting Started

### ✅ Requirements

Install the required packages:

```bash
pip install pandas requests beautifulsoup4 scikit-learn
```

 ## 📜 Usage Guide
### 🔹 Milestone 1: Web Scraping

Scraped IMDb Top 250 using Python requests and BeautifulSoup

Extracted fields from JSON-LD embedded in <script type="application/ld+json">

Fields collected:

Title

Description

Rating

Duration

Genre

URL

🔹 Milestone 2: Data Cleaning & Preprocessing
Duration Extraction
Used regex to parse strings like "PT2H22M" into integer minutes

Missing Values
Handled missing durations with default values

Duplicate Removal
Used drop_duplicates()

Normalization
Min-Max scaling applied to Rating and Duration

Genre Encoding
One-hot encoded genres using str.get_dummies(sep=', ')

🔧 Key Tools Used:
re for regex

MinMaxScaler from sklearn

pandas.get_dummies()
Assumptions & Notes
Focused only on IMDb’s Top 250 movies

Duration values default to 0 when not available

Genre columns are multi-labeled and split correctly

✅ Final Output
The cleaned dataset (cleaned_top_IMDB_db.csv) contains:

250 movies

Fully preprocessed fields

Normalized numeric features

Binary-encoded genres

Ready for:

🧪 Machine Learning

📊 Visualization

📈 Time Series or EDA

✍️ Author
Sonu Tamang
📍 Newark, NJ
🔗 LinkedIn
📧 sonulama778@gmail.com

📌 License
This project is shared under the MIT License. Feel free to reuse or build on it.





