🧠 Question Answering on Virat Kohli News Using Transformers

📌 Project Overview
This project builds a Question Answering (QA) system that can answer questions about Virat Kohli by analyzing recent news articles. It uses the NewsAPI to collect articles and Hugging Face Transformers for building the QA model. The text is preprocessed using spaCy, and sentiment trends are also visualized to provide more context.

📚 Table of Contents
Introduction

Tools & Libraries

Data Collection

Text Preprocessing

Question Answering System

Sentiment Analysis (Optional)

Visualization

Sample Output

Conclusion

1. 🎯 Introduction
The goal is to answer user questions (e.g., "Is Virat Kohli retiring?") using information extracted from online news articles. The project combines web scraping, NLP, and transformer models to build an intelligent QA system.

2. 🧰 Tools & Libraries Used
NewsAPI: For fetching recent news articles

Pandas: Data handling

spaCy: Text preprocessing

Transformers (Hugging Face): QA and sentiment models

Matplotlib/Seaborn: Visualization

3. 📰 Data Collection
Source: NewsAPI (get_everything)

Query: "Virat Kohli"

Timeframe: Last 30 days

Language: English

Format: JSON → Pandas DataFrame

4. ✂️ Text Preprocessing
Removing duplicates and nulls

Using spaCy for:

Tokenization

Lemmatization

Cleaning (stop words, special characters)

Combining all articles into one large context string

5. ❓ Question Answering System
Model Used: pipeline("question-answering") from Hugging Face

Inputs:

Question: User-defined (e.g., "Is Kohli injured?")

Context: All preprocessed article content

Output: Extracted answer with confidence score

python
Copy
Edit
qa_pipeline = pipeline('question-answering')
result = qa_pipeline(question="Is Virat Kohli retiring?", context=full_text)
6. 💬 Sentiment Analysis (optional but included)
Uses pipeline("sentiment-analysis")

Assigns sentiment labels to each article

Can be visualized as a trend over time

7. 📈 Visualization
Sentiment Over Time: Line graph showing public/media sentiment

Answer Confidence: Can be plotted if desired

8. 🧪 Sample Output
Question: "Is Virat Kohli retiring?"
Answer: "There is no official announcement about retirement."
Confidence: 0.92

9. ✅ Conclusion
This project successfully demonstrates how QA models can be used to extract real-time insights from web data. It combines data scraping, NLP, and transformer models into a cohesive pipeline.
