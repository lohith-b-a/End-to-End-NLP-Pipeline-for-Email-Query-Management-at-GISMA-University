# End-to-End NLP Pipeline for Email Query Management at GISMA University

## Project Overview

This project builds a custom Natural Language Processing (NLP) pipeline to analyze and manage student emails received by the GISMA University administration team. It addresses the operational challenge of high email volume and limited staff resources by extracting key information and identifying topics automatically.

The project simulates a real-world deployment scenario and prepares the groundwork for future chatbot development to automate frequent queries.

---

## Business Problem

GISMA University receives a large volume of emails daily from:
- Enrolled students (requests, complaints, documents, date changes)
- Prospective students (course inquiries, admissions, deadlines)

Due to limited administrative staff, response delays are causing dissatisfaction.  
This NLP pipeline will:
- Automatically extract key information (student name, ID, program, etc.)
- Classify email intent using topic modeling
- Streamline routing and resolution of queries

---

## Dataset

- Type: Synthetic email dataset generated for simulation
- Columns: `Email`, `Text`, `Program`, `Date`, etc.
- Labels: No manual labels; unsupervised + custom NER

---

## NLP Tasks Performed

1. Text Preprocessing
   - Lowercasing, punctuation removal
   - Removing stopwords and email-specific noise (email addresses, URLs)
   - Tokenization and lemmatization

2. Named Entity Recognition (NER)
   - Built a custom NER model using spaCy
   - Extracted entities like:
     - Student Name
     - Student ID
     - Program
     - Date references
   - Used a blank spaCy model trained on hand-labeled examples

3. Topic Modeling
   - Performed topic modeling using LDA (Latent Dirichlet Allocation)
   - Identified dominant themes in student concerns
   - Visualized topics with pyLDAvis

---

## Key Features

- Custom spaCy NER model trained on domain-specific entity types
- Information extraction for automated email triage
- Unsupervised topic modeling to understand frequent concerns
- Designed for real-world university operations with future chatbot integration

---

## Tools & Technologies

- Python (Jupyter Notebook)
- spaCy (custom NER training)
- NLTK, re (cleaning and tokenization)
- Gensim + pyLDAvis (Topic modeling)
- pandas, seaborn, matplotlib

---

## Skills Demonstrated

- Named Entity Recognition (NER)
- Text preprocessing for NLP
- Unsupervised topic modeling (LDA)
- Custom model training (spaCy)
- Business-oriented problem solving with NLP

---

## Author

**Lohith Basavanahalli Anjinappa**  

