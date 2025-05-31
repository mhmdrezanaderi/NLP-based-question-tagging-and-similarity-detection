# NLP Based Question Tagging and Similarity Detection
This project implements an NLP-based system to automatically detect question similarity and assign relevant tags using a dataset of 60,000 Stack Overflow questions. The system is designed in three major phases:

    Text Preprocessing
    Clean and normalize raw question text (title and body) by removing HTML tags, special characters, and unnecessary content to prepare it for analysis and modeling.

    Similarity Retrieval with Word2Vec
    Train a Word2Vec model on the dataset and convert questions into document embeddings. Using cosine similarity, the system retrieves the most semantically similar questions for a given query. Visualizations in 3D space are also used to inspect word and document embeddings.

    Tag Prediction using KNN
    For an unseen question, the model finds its nearest neighbors in the training data using embeddings, extracts their tags, and predicts appropriate tags. Accuracy is measured by comparing predicted tags with the actual ones.

## Key Achievements

- **Preprocessed** over 60,000 questions from Stack Overflow, removing noise and HTML content.
- **Trained a Word2Vec** model to generate embeddings for words and entire documents.
- Implemented **semantic similarity** retrieval using cosine similarity on question embeddings.
- Visualized high-dimensional embeddings using **3D plots** for better interpretability.
- Applied **K-Nearest Neighbors (KNN)** for tag prediction based on semantic similarity.
- Evaluated tag prediction accuracy by comparing predicted vs. actual tags.
- Provided examples of successful and failed tag predictions with explanations.
