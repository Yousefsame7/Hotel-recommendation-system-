# Hotel-recommendation-system-

---

## 🧠 What kind of system is this?

**Content-Based Hotel Recommendation System**

* Recommends hotels based on:

  * **Country (location)**
  * **Text similarity of Tags**
* Uses **text processing + word matching**, not training.

---

## 🛠 Tools & Libraries Used

### 1️⃣ **pandas**

**Purpose:** Data handling & cleaning
Used for:

* Reading CSV
* Dropping columns
* Creating new columns
* Filtering hotels by country

```python
import pandas as pd
```

---

### 2️⃣ **numpy**

**Purpose:** Indexing & numerical operations

```python
import numpy as np
```

Used for:

* Resetting index
* Handling array shapes

---

### 3️⃣ **NLTK (Natural Language Toolkit)** ⭐

**Main library of this project**

```python
import nltk
```

Used for **text processing (NLP)**:

#### ✔ Tokenization

```python
word_tokenize()
sent_tokenize()
```

#### ✔ Stopwords removal

```python
stopwords.words("english")
```

#### ✔ Lemmatization

```python
WordNetLemmatizer()
```

#### ✔ NLTK datasets

* `punkt`
* `stopwords`
* `wordnet`
* `omw-1.4`

---

### 4️⃣ **ast (literal_eval)**

**Purpose:** Convert string → list safely

```python
from ast import literal_eval
```

Used to process the **Tags** column.

---

## 🔍 Technique Used (Not a Model)

### ✅ Text Similarity using:

* Tokenization
* Stopword removal
* Lemmatization
* **Set intersection** (word overlap)

```text
Similarity = number of common words
```

More common words → higher similarity → better recommendation

---

## ⚙️ Recommendation Logic (Simple)

1. User enters:

   * Country (FR, UK, IT…)
   * Description (e.g. “Business trip”)
2. Clean & process text
3. Compare user words with hotel Tags
4. Rank hotels by:

   * Similarity score
   * Average hotel rating
5. Return **Top 10 hotels**

---

## 🧾 One-line summary (perfect for report)

> This project is a content-based hotel recommendation system using NLP techniques without machine learning.

---

## 🎯 Very short viva answer

> No model is used. It is a rule-based recommendation system using NLTK for text similarity.

If you want:

* **Add ML (TF-IDF + Cosine Similarity)**
* **Upgrade to ML project**
* **Arabic explanation**
* **Fix & clean the code**


