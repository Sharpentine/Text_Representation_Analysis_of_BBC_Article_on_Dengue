### **Text Representation Analysis of BBC Article on Dengue**

---

#### **Introduction**

This report examines the application of three text representation methods – Bag of Words (BoW), Term Frequency-Inverse Document Frequency (TF-IDF), and Word Embeddings – to a BBC article focusing on dengue fever in the Philippines. The primary goal is to assess the effectiveness of each method in capturing the article's semantic meaning and facilitating further analysis.

---

#### **Data and Methods**

The dataset used for this analysis is a news article sourced from BBC News, titled **"Philippine town offers bounty for mosquitoes as dengue rises."** The article details the response of a Philippine town to an increase in dengue cases by offering rewards for captured mosquitoes.

Three text representation methods were employed:

1. **Bag of Words (BoW):**
   - Represents text as a collection of words and their frequencies, disregarding word order and semantic relationships.

2. **TF-IDF (Term Frequency-Inverse Document Frequency):**
   - Similar to BoW but considers the importance of words in the entire corpus, giving higher weights to words that are frequent in a specific document but rare overall.

3. **Word Embeddings (Word2Vec):**
   - Represents words as dense vectors in a continuous space, capturing semantic relationships and placing words with similar meanings closer together.

---

#### **Findings**

- **BoW:**
  - This method successfully created a basic representation of the article's vocabulary and word frequencies.
  - However, it failed to capture the semantic relationships between words, hindering a deeper understanding of the article's context.

- **TF-IDF:**
  - While offering an improvement over BoW by highlighting important words, TF-IDF still exhibited limitations in capturing the nuances of the article's meaning.
  - It couldn't fully grasp the connections between words like "dengue" and "fever" or "mosquito" and "insect."

- **Word Embeddings:**
  - This method proved to be the most effective in capturing the article's semantic meaning.
  - By leveraging pre-trained word embeddings (`word2vec-google-news-300`), it successfully represented words as vectors in a semantic space, allowing for the identification of relationships between words and phrases.
  - This representation provided a deeper understanding of the article's context and subject matter.

---

#### **Analysis and Discussion**

Each method exhibits distinct strengths and weaknesses:

1. **BoW:**
   - **Strengths:** Simple and efficient, suitable for basic text analysis.
   - **Weaknesses:** Overlooks semantic relationships and word order. Inadequate for complex semantic understanding.

2. **TF-IDF:**
   - **Strengths:** Improves upon BoW by considering word importance.
   - **Weaknesses:** Still lacks the ability to capture deeper semantic relationships.

3. **Word Embeddings:**
   - **Strengths:** Offers the most comprehensive semantic representation, capturing relationships between words and phrases, enabling a richer understanding of the text.
   - **Weaknesses:** Can be computationally expensive for training and might not perfectly handle out-of-vocabulary words.

---

#### **Conclusion**

For this specific task of capturing the semantic meaning of a news article about dengue, **Word Embeddings** emerged as the most effective method. By representing words as vectors in a semantic space, it facilitated the understanding of relationships between crucial concepts like "dengue," "fever," "mosquito," and "bounty." 

While **BoW** and **TF-IDF** provide basic representations, they fall short in capturing the deeper meaning and context embedded in the article. For tasks requiring nuanced semantic understanding, such as topic modeling or sentiment analysis, **Word Embeddings** are the preferred choice.

---
