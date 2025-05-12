# Virat-Kohli-News-Analysis-with-NLP

📌 Project Overview
This project retrieves the latest news articles about Indian cricketer Virat Kohli from the past 30 days using the NewsAPI. It then performs preprocessing and basic Natural Language Processing (NLP) tasks such as tokenization and lemmatization using spaCy, and provides basic insights from the content.

⚙️ Technologies Used
Python

NewsAPI

Pandas

spaCy

Regular Expressions (re)

📥 Data Collection
Source: NewsAPI

Query: "Virat Kohli"

Date Range: Last 30 days

Language: English

Sorting: By relevancy

API Client: Initialized using NewsApiClient(api_key=...)

🧹 Data Preprocessing
Removing Duplicates: Dropped duplicate articles based on the title.

Handling Nulls: Removed rows with missing article content.

Text Cleaning:

Tokenization using spaCy

Lemmatization (extracting the base form of words)

Removal of punctuation, stop words, and special characters

🧠 NLP Tasks
Tokenization

Lemmatization

Entity recognition (optional, depending on code)

📊 Output
A cleaned DataFrame containing recent articles about Virat Kohli

Processed text ready for further analysis like sentiment detection, topic modeling, or word cloud generation (if implemented)
