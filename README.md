🔹 Overview

This project involves developing an AI-based chatbot capable of answering user queries by retrieving the most relevant response from a predefined set of Frequently Asked Questions (FAQs) using Natural Language Processing (NLP) and text similarity techniques.

🧠 Core Technologies & Concepts Used

1. Natural Language Processing (NLP)

Text preprocessing: Tokenization, stopword removal, lowercasing

Vectorization using TF-IDF (Term Frequency–Inverse Document Frequency)

Calculates how important a word is in a question relative to the FAQ dataset.

2. Similarity Matching

Cosine Similarity is used to measure how close the user query vector is to the stored FAQ vectors.

The question with the highest similarity score is selected, and its answer is returned.

3. Thresholding Logic

A confidence score threshold is set (e.g., 0.2).

If no FAQ exceeds this similarity threshold, the chatbot replies with a default fallback message.

4. Interface

A basic web interface is implemented using HTML/CSS/JS or Python frameworks like Flask or Streamlit, allowing real-time interaction.

The interface accepts user input and displays the chatbot's response dynamically.

5. Dataset

The FAQ pairs are stored in a structured format (e.g., lists, JSON, or a database like SQLite).

These serve as the knowledge base for the chatbot.

📈 Advantages

Lightweight and fast

Works offline (if needed)

Easily expandable (add more FAQs)

Minimal dependencies

🔍 Limitations

Relies on exact/close keyword match (TF-IDF based)

Cannot handle very vague or complex questions

Doesn’t understand context deeply (no semantic awareness)

🚀 Possible Upgrades

Replace TF-IDF with transformer-based models (BERT, Sentence-BERT) for semantic similarity

Add multilingual NLP and voice input/output

Train on domain-specific queries using custom datasets
