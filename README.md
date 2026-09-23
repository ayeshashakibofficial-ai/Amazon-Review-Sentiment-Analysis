# Amazon-Review-Sentiment-Analysis
End-to-end NLP project performing sentiment analysis (VADER) and emotion detection on 20,000 Amazon customer reviews using Python, NLTK, and Seaborn.
# 🎭 Amazon Customer Reviews: Sentiment Analysis & Emotion Detection

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![NLTK](https://img.shields.io/badge/NLTK-VADER-green)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-purple)

While basic sentiment analysis classifies text as positive or negative, this project goes a step further by layering **granular emotion categorization** (Joy, Trust, Frustration, Sadness, Fear) to deliver actionable business insights for product teams.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Environment:** Google Colab
* **Data Manipulation:** `pandas`, `numpy`
* **Text Preprocessing & Modeling:** `nltk` (Tokenization, Stopwords, VADER Lexicon), `re`
* **Data Visualization:** `seaborn`, `matplotlib`, `wordcloud`

---

## ⚙️ Methodology & Pipeline

1. **Data Acquisition & Sampling:** Loaded a 20,000-row review dataset and drew a stratified 5,000-row working sample for high-performance processing.
2. **Text Preprocessing:** Cleaned review text by lowercasing, stripping URLs/punctuation/digits, tokenizing, and removing English stop words.
3. **Sentiment Classification (VADER):** Applied NLTK's VADER `SentimentIntensityAnalyzer` to compute compound polarity scores:
   * **Positive:** Compound score $\ge$ 0.05
   * **Neutral:** Score between -0.05 and 0.05
   * **Negative:** Compound score $\le$ -0.05
4. **Visual Analytics:** Generated distribution bar charts, compound score density plots, and frequency word clouds.
5. **Emotion Mapping:** Categorized underlying customer emotions using keyword frequency tracking across core affect categories.

---

## 📊 Key Findings & Visualizations

* **Overwhelming Positive Polarity:** Nearly **79%** of reviews were categorized as positive, with compound scores heavily skewed toward $+0.75$ to $+1.0$.
* **Primary Drivers:** Keywords like *great*, *love*, *game*, *easy*, and *time* dominated customer praise.
* **Emotional Breakdown:**
  * **Joy / Satisfaction:** ~4,437 occurrences
  * **Trust / Reliability:** ~1,090 occurrences
  * **Frustration / Anger:** ~496 occurrences
  * **Fear / Concern:** ~171 occurrences


---

## 💡 Business & Strategic Takeaways

1. **High Satisfaction & Usability:** Product adoption is strong, driven primarily by intuitive usability (*easy, simple*) and high entertainment value.
2. **Targeted Bug Fixes Needed:** Negative emotional clusters (*Frustration* and *Fear*) stem mainly from technical friction points like app freezing, download errors, or device compatibility. Prioritizing stability patches in future updates will reduce customer churn and protect review ratings.

---

## 🚀 How to Run locally / in Colab

1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/amazon-review-sentiment-emotion-analysis.git](https://github.com/YOUR_USERNAME/amazon-review-sentiment-emotion-analysis.git)
