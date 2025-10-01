# sentiment.analysis
This project performs **sentiment analysis** on IMDB movie reviews using **TF-IDF** vectorization and **Logistic Regression**. It predicts whether a movie review is **positive** or **negative**.
## Dataset
- Source: IMDB movie reviews
- Columns:
  - `reviews` → the text of the review
  - `sentiment` → 0 = negative, 1 = positive

---

## Approach
1. **Text Preprocessing**
   - Convert text to lowercase
   - Remove punctuation
   - Optional: remove stopwords

2. **Feature Extraction**
   - TF-IDF Vectorization
   - Unigrams + Bigrams (`ngram_range=(1,2)`)
   - Max features: 10,000

3. **Model**
   - Logistic Regression
   - `max_iter=500`, `C=1.0`
   - Trained on 80% of the data, tested on 20%

4. **Evaluation**
   - Accuracy: ~90.3%
   - Metrics: Classification Report & Confusion Matrix

---

