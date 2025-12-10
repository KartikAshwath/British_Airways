
# ✈️ British Airways Customer Review Sentiment Analysis

## 🎯 Project Goal

The primary goal of this project is to collect, clean, and analyze customer reviews for **British Airways** (BA) scraped from the Skytrax website. The project involves a two-stage approach to sentiment classification:

1. **Baseline Analysis:** Using the lexicon-based **VADER** model.  
2. **Machine Learning:** Training and evaluating several supervised classification algorithms to build a more robust sentiment predictor.

---

## 📁 Project Structure

| File/Folder | Description |
|------------|-------------|
| `Web_Scrapping.ipynb` | **Data Collection:** Jupyter notebook containing the code for scraping reviews from Skytrax using `requests` and `BeautifulSoup`. |
| `getting_started.ipynb` | **Analysis & Modeling:** Main notebook for data cleaning, baseline VADER analysis, and training of Machine Learning models. |
| `BA_reviews.csv` | **Clean Data:** The final, structured dataset of British Airways reviews (approx. 1500 records) used for analysis. |
| `british_airways_reviews.json` | **Raw Data:** The initial output file from the web scraping process. |
| `Untitled.ipynb` | *(Placeholder/Draft Notebook)* |
| `README.md` | This document. |

---

## ⚙️ Setup and Dependencies

To run this project, you will need **Python 3.x** and the following libraries. Install them using:

```bash
pip install pandas requests beautifulsoup4 nltk scikit-learn seaborn matplotlib
````

### Core Libraries

* **requests**, **BeautifulSoup4** — Web scraping
* **pandas** — Data manipulation and cleaning
* **nltk** — VADER sentiment analysis
* **scikit-learn** — KNN, Naive Bayes, Decision Tree, and Random Forest algorithms

---

## 📈 Methodology & Analysis Steps

### **Step 1: Data Collection**

* **Source:** Skytrax
* **Method:** Web scraping in `Web_Scrapping.ipynb`
* **Output:** ~1500 customer reviews stored in the JSON file and converted to CSV (`BA_reviews.csv`)

---

### **Step 2: Baseline Sentiment Analysis (VADER)**

VADER is used to generate sentiment scores (`compound`, `pos`, `neg`, `neu`) for each review.

#### ⚠️ IMPORTANT CORRECTION

The notebook `getting_started.ipynb` currently contains two issues:

* VADER is applied to the literal string `'Reviews'` instead of the review text variable.
* A `break` statement prematurely ends the loop.

**These errors must be corrected to run sentiment scoring across the full dataset.**

---

### **Step 3: Supervised Machine Learning Modeling**

Trains four classifiers to predict sentiment (Positive/Negative) using review text features.

| Model                         | Classification Principle                                                                 |
| ----------------------------- | ---------------------------------------------------------------------------------------- |
| **Naive Bayes**               | Probabilistic model based on word frequency. Fast and effective for text classification. |
| **Decision Tree**             | Builds decision rules based on text features. Highly interpretable.                      |
| **K-Nearest Neighbors (KNN)** | Classifies based on similarity to nearest labeled reviews.                               |
| **Random Forest**             | Ensemble of Decision Trees for improved accuracy and reduced overfitting.                |

---

### **Step 4: Model Evaluation**

Evaluation metrics include:

* **Precision:** How many predicted positives were correct?
* **Recall:** How many actual positives were captured?
* **F1-Score:** Harmonic mean of Precision and Recall; primary model comparison metric.

---

## 🚀 How to Run the Project

1. **Clone the repository** (if applicable).
2. **Install the required dependencies** using the pip command above.
3. **Launch Jupyter Notebook/Lab** on your machine.
4. **Open and run `getting_started.ipynb`:**

   * Loads and cleans the dataset
   * Runs VADER sentiment analysis
   * Vectorizes review text
   * Trains the four ML models
5. **Review results:** Compare Precision, Recall, and F1-Score to determine the best sentiment prediction model.

---

If you’d like, I can also generate **badges**, a **project logo**, or a more polished **GitHub-ready README**.

.
