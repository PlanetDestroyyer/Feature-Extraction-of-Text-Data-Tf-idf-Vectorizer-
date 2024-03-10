TF-IDF (Term Frequency-Inverse Document Frequency) is a numerical statistic used in information retrieval and text mining to evaluate the importance of a word in a document relative to a collection of documents. It consists of two components:

1. **TF (Term Frequency):** This measures the frequency of a term (word) in a document. It is calculated by dividing the number of times a term appears in a document by the total number of terms in the document. It helps to identify the importance of a term within a single document.

   TF(t, d) = (Number of times term t appears in document d) / (Total number of terms in document d)

2. **IDF (Inverse Document Frequency):** This measures the importance of a term across a collection of documents. It is calculated by dividing the total number of documents by the number of documents containing the term, and then taking the logarithm of the result. It helps to identify the rarity of a term across the entire document collection.

   IDF(t) = log_e(Total number of documents / Number of documents containing term t)

The TF-IDF score for a term in a document is obtained by multiplying its TF and IDF scores:

   TF-IDF(t, d) = TF(t, d) * IDF(t)

**Key Points:**

- Terms with higher TF-IDF scores are considered more important within a document and across a collection of documents.
- Common words that appear frequently in many documents (e.g., "the", "and", "is") tend to have low TF-IDF scores because they are less discriminative.
- Rare words that appear in only a few documents tend to have higher TF-IDF scores because they are more discriminative.

TF-IDF is commonly used in various natural language processing (NLP) tasks such as document classification, information retrieval, text summarization, and keyword extraction. It helps in identifying important terms that represent the content of a document or a collection of documents.