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
