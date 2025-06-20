This model helps in identifying duplicate questions in quora dataset. It is implemented using 3 different strategies:

1. The questions are vectorized using BoW and trained RandomForest and XGBClassifier algorithms
2. The questions are tokenized and sent into a Neural network. Each question is embedded seperately and performed attention to identify the context of each question. Then using cosine similarity, the similarity scores are computed and classified.
3. The question-pairs are joined together and sent in as a single sequence of tokens into a neural network and embedded it. Then applied attention on that one big sentence flattened attention output and a fully connected layer is used to perform classification
