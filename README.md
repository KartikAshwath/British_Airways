# Airline Review Insights – From Web to Dashboard ✈️

## Overview
This is an end-to-end Data Science project demonstrating:
- Web scraping skills
- Data cleaning & preprocessing
- Natural Language Processing (NLP) techniques
- Integration of multiple DS tools & libraries
- Interactive data visualization

## Workflow
1. **Web Scraping:** `scripts/scraper.py` – Collects airline reviews from the web.
2. **Data Cleaning & Preprocessing:** `scripts/preprocessing.py` – Cleans and prepares data for analysis.
3. **NLP Analysis:** `notebooks/nlp_analysis.ipynb` – Sentiment analysis, topic modeling, keyword extraction.
4. **Visualization:** `notebooks/eda.ipynb` – Exploratory Data Analysis & insights.
5. **Dashboard:** `dashboard/app.py` – Interactive dashboard with Streamlit or Power BI integration.

## Tools & Libraries
- Python: requests, BeautifulSoup, pandas, nltk, spacy, gensim, scikit-learn, matplotlib, seaborn, wordcloud
- Visualization: Power BI / Streamlit
- Cloud (Optional): Streamlit Cloud / Heroku / GCP BigQuery

## Project Structure
```
airline_review_portfolio/
│── data/               # Raw and processed datasets
│── notebooks/          # Jupyter notebooks for EDA & NLP
│── scripts/            # Python scripts for scraping & preprocessing
│── dashboard/          # Dashboard files (Streamlit app / Power BI)
│── docs/               # Documentation, reports, and images
│── README.md           # Project documentation
```

## How to Run
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the scraper: `python scripts/scraper.py`
4. Process data: `python scripts/preprocessing.py`
5. Explore notebooks in `notebooks/` for analysis.
6. Launch dashboard: `streamlit run dashboard/app.py`
