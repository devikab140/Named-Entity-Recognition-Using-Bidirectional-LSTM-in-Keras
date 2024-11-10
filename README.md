# Named Entity Recognition Using Bidirectional LSTM in Keras
This repository contains the implementation of a Named Entity Recognition (NER) model using a bidirectional Long Short-Term Memory (LSTM) network in Keras with TensorFlow as the backend. The project demonstrates how deep learning techniques, specifically bidirectional LSTMs, can be effectively used to recognize named entities within text, including names, organizations, locations, and other essential categories.

## Project Overview
Named Entity Recognition (NER) is a core NLP task that involves identifying and categorizing key information in text. This project leverages a bidirectional LSTM model, which captures contextual information in both forward and backward directions, thereby enhancing the accuracy of entity recognition in complex text patterns. The project's approach is beneficial for various NLP applications, such as information extraction, question answering, and machine translation.

## Dataset
The project uses an annotated dataset where each word in a sentence is tagged with its corresponding entity label (e.g., PERSON, LOCATION, ORGANIZATION). You can use standard datasets like the CoNLL-2003 NER dataset or other tagged NER datasets, which can be preprocessed for tokenization and entity label encoding.

The dataset should be structured as follows:

Each sentence is tokenized into words and assigned entity tags.
Preprocessing involves converting words to embeddings and encoding entity labels for model input.
## Model Architecture
The model consists of:

- Embedding Layer: For representing words as dense vectors.
- Bidirectional LSTM Layer: Captures dependencies in both forward and backward directions to enhance contextual understanding.
- Dense Output Layer with Softmax Activation: Classifies each token into its respective entity category.
## Training and Evaluation
Training Parameters:

- Optimizer: Adam
- Loss Function: Categorical Cross-Entropy
- Metrics: Precision, Recall, F1-Score
## Evaluation:

The model is evaluated based on precision, recall, and F1-score across various entity types.
## Results
The bidirectional LSTM model achieved high performance on the NER task, demonstrating strong results in terms of precision, recall, and F1-score. The bidirectional structure helps capture the context on both sides of each word, which is especially beneficial for complex, context-dependent entity recognition.


