# GenAI_LLM_engineering_SCFP125041

1.Load IMDB Dataset.csv and subsample a smaller portion, e.g., 2,000–3,000 rows, for lab speed training.

2.Convert the sentiment column into numeric labels: positive = 1 and negative = 0.

3.Split the data into training and test sets.

4.Tokenize the review texts using tiktoken cl100k_base encoding to convert each review into a list of token IDs.

5.Pad or truncate the token sequences to a fixed length so all inputs are the same size.

6.Convert the token sequences and labels into tensors.

7.Build a model with an Embedding layer → nn.RNN → Linear output layer.

8.Train the model using an appropriate loss function and optimizer, printing the loss periodically.

9.Check the model accuracy on the test dataset.

10.Test the model on 2–3 new review sentences you write yourself and print the predicted sentiment.