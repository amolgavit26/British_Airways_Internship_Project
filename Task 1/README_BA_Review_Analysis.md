# British Airways Review Analysis ✈️📝

This project involves **web scraping**, **data cleaning**, and **sentiment analysis** of customer reviews for British Airways from [Skytrax](https://www.airlinequality.com/airline-reviews/british-airways). 

It demonstrates a full cycle of data collection to analysis using Python libraries such as `BeautifulSoup`, `pandas`, and `vaderSentiment`.

---

## 📁 Project Structure

```
├── getting_started_uncleaned.ipynb   # Web scraping raw reviews
├── getting_started_cleaned.ipynb     # Data cleaning + sentiment analysis
├── BA_reviews.csv                    # Output cleaned dataset
└── README.md                         # Project description
```

---

## 🛠️ Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/ba-review-analysis.git
cd ba-review-analysis
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install pandas beautifulsoup4 requests vaderSentiment
```

---

## 🔎 Features

### 1. Web Scraping
- Collects British Airways reviews (up to N pages)
- Extracts:
  - Review text
  - Date
  - Country
  - Rating

### 2. Data Cleaning
- Removes boilerplate text and formatting
- Extracts "Trip Verified" status
- Parses date formats

### 3. Sentiment Analysis
- Uses VADER sentiment analyzer
- Computes compound score
- Classifies into:
  - Positive
  - Neutral
  - Negative

---

## 📊 Sample Output

| review_snippet       | verified | rating | sentiment_score | analysis |
|----------------------|----------|--------|------------------|----------|
| Great flight overall | Yes      | 8      | 0.71             | Positive |
| Delayed and crowded  | No       | 2      | -0.45            | Negative |

---

## 📌 Usage

1. Run `getting_started_uncleaned.ipynb` to scrape reviews.
2. Run `getting_started_cleaned.ipynb` to clean and analyze.
3. Final output will be saved as `BA_reviews.csv`.

---

## 📃 License

This project is licensed under the MIT License.

---

## 🙏 Acknowledgements

Thanks to:
- [Skytrax](https://www.airlinequality.com/) for public data
- Developers of `BeautifulSoup` and `vaderSentiment`
