# Mini-Language-Translator


## Objective
This repository contains the completed projects for the 2nd Year Tasks, focusing on Natural Language Processing (NLP) and classical Machine Learning. It includes a multi-language translator and a smart expense categorizer.

---
## Project 1: Mini Language Translator 🌐

### Objective
To build a simple but powerful language translator that can translate English sentences into multiple regional Indian languages (Hindi and Marathi).

### Tech Stack
* **Language:** Python
* **Libraries:** Hugging Face `transformers`, `torch`, `sentencepiece`
* **Models:**
    * `Helsinki-NLP/opus-mt-en-hi` (English to Hindi)
    * `Helsinki-NLP/opus-mt-en-mr` (English to Marathi)
* **Environment:** Jupyter Notebook

### Implementation
This project leverages pre-trained, state-of-the-art models from the Hugging Face Hub. Instead of training from scratch, it uses the `pipeline` API from the `transformers` library to download and perform direct inference with these powerful models.

### Translation Examples
```
English: Hello, how are you doing today?
Hindi: हैलो, आप आज कैसे कर रहे हैं?
Marathi: हॅलो, आज तुम्ही कसे आहात?
------------------------------
English: Data science is an exciting field.
Hindi: डाटा साइंस एक रोमांचक क्षेत्र है।
Marathi: डेटा सायन्स हे एक रोमांचक क्षेत्र आहे.
------------------------------
```

---
## Project 2: Smart Expense Categorizer 🧾

### Objective
To build a machine learning model that automatically categorizes financial transactions based on their text descriptions (e.g., 'Swiggy order' -> 'Food').

### Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Scikit-learn
* **Environment:** Jupyter Notebook

### Implementation
This project demonstrates a complete, end-to-end machine learning workflow:
1.  **Data Collection:** A custom dataset of over 100 transaction examples across 8 categories was created.
2.  **Preprocessing:** Text was cleaned by converting it to lowercase, removing special characters, and filtering out common English "stop words."
3.  **Feature Extraction:** Cleaned text was converted into numerical vectors using `TfidfVectorizer`.
4.  **Modeling & Evaluation:** A `LinearSVC` (Support Vector Classifier) model was trained and evaluated using 5-fold cross-validation to ensure a reliable measure of its performance.

### Example Predictions
```
'Coffee at Starbucks' ==> Predicted Category: Food
'IRCTC Ticket Booking' ==> Predicted Category: Travel
'Monthly rent transfer' ==> Predicted Category: Bills & Utilities
```
