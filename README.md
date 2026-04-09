# day-38
Word2Vec-based semantic analysis on e-commerce reviews, including polysemy handling, context disambiguation, and similarity evaluation.

### Q1: Word2Vec & Polysemy

* Trained Word2Vec model on ShopSense reviews dataset
* Demonstrated limitation of Word2Vec:

  * Single vector representation for polysemous word **"cheap"**
* Computed cosine similarity:

  * cheap vs affordable
  * cheap vs flimsy

### Q1(b): Context-Based Disambiguation

* Built a simple system to classify meaning of "cheap":

  * **Affordable** (positive)
  * **Low-quality** (negative)
* Used:

  * Sentence embeddings (average Word2Vec vectors)
  * Anchor word comparison

### Q1(c): Window Size Analysis

* Compared:

  * `window = 2` → syntactic relationships
  * `window = 10` → semantic relationships
* Observed impact on contextual understanding

---

### Q2: Semantic Similarity Comparison

Compared similarity between two reviews using:

1. **Bag of Words (BOW)**
2. **TF-IDF**
3. **Word2Vec (averaged embeddings)**
4. **Sentence-BERT**

---

## 🔍 Key Insights

* Word2Vec captures semantic relationships but fails with polysemy
* BOW fails due to lack of semantic understanding
* TF-IDF improves weighting but still relies on exact words
* Word2Vec captures word-level meaning
* Sentence-BERT best captures full sentence meaning and context



---

## 👤 Author

Your Name

