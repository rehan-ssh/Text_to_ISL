# 🧏‍♂️ English Grammar to Indian Sign Language (ISL) Grammar Converter

## 📌 Overview

This project aims to **bridge the communication gap between spoken English and the Deaf community** by converting **English sentences into Indian Sign Language (ISL) grammar**.

Instead of building a model from scratch, we leveraged an **existing English-to-German translation model** and **adapted it for grammatical restructuring**, since German and ISL share similarities in **sentence reordering (especially verb placement)**. By training the model on a **custom cleaned dataset aligned with ISL grammar rules**, we achieved meaningful English-to-ISL grammar conversion.

---

## 🎯 Problem Statement

* English follows a **Subject–Verb–Object (SVO)** structure.
* Indian Sign Language commonly follows **Subject–Object–Verb (SOV)** or **Topic–Comment** structure.
* Direct translation from English to ISL leads to:

  * Incorrect grammar
  * Loss of meaning
  * Poor sign interpretation

There is a lack of **automated tools that respect ISL grammatical structure**.

---

## 💡 Our Approach

### 🔹 Model Reuse & Adaptation

* Used a **pre-trained English → German translation model**
* Reason:

  * German grammar involves **verb repositioning**, similar to ISL
  * The model already understands **syntactic transformations**
* Fine-tuned the model using a **cleaned and structured dataset** that maps:

  * English sentences → ISL grammar equivalents

---

## ⚙️ Key Features

* ✅ Converts English sentences into ISL-compliant grammar
* ✅ Removes unnecessary English constructs (articles, auxiliaries, fillers)
* ✅ Reorders sentence structure based on ISL rules
* ✅ Efficient reuse of a pre-trained NLP model
* ✅ Scalable for future sign language applications

---

## 🛠️ Technologies Used

* **Model**: Pre-trained English → German translation model
* **Dataset**: Custom cleaned dataset aligned with ISL grammar
* **Techniques**:

  * Data cleaning & normalization
  * Grammar restructuring
  * Transfer learning
* **Libraries/Frameworks**:

  * *[NLTK/spCy, Pandas, numpy, LSTM architecture]*

---

## 🔄 Example

**Input (English):**

> She is eating an apple.

**Output (ISL Grammar):**

> She apple eat.

*(Output reflects ISL grammatical order, not spoken English.)*

---

## 📊 Dataset Preparation

* Removed articles (a, an, the)
* Removed auxiliary verbs (is, am, are, was)
* Normalized verb forms
* Reordered sentences to match ISL grammar
* Ensured consistency and reduced noise in training data

---

## 📈 Future Enhancements

* 🔹 Support for complex and compound sentences
* 🔹 Integration with ISL sign animation or video generation
* 🔹 Expansion to regional ISL variations
* 🔹 Improve accuracy with larger ISL-aligned datasets

---

## 🌍 Impact

This project contributes to:

* 🌐 Accessible communication for Deaf and Hard-of-Hearing individuals
* 🤝 Inclusive language technologies
* 📚 Awareness of Indian Sign Language grammar
* 🚀 Research in low-resource language adaptation
