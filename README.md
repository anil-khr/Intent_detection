# Intent_detection


### Twitter Customer Support Dataset 

The dataset contains more than 2.8 million tweets and includes metadata such as tweet ID, author ID, inbound or outbound tweet, timestamp, text of the tweet, and response tweet ID.
Download the Twitter Customer Support Dataset from Kaggle and save it to your local machine.

### Data labelling
The Data labelling is done by identifing the customer's intent by associating certain keywords with specific intent categories. The output of the code is a dataframe that shows the inbound text messages, the associated customer intent, and the sentiment of the message.


### Preprocessing
The input text data is preprocessed using NLTK's stopwords and word_tokenize functions. The Tokenizer class from Keras is used to convert the text to sequences of integers, and pad_sequences is used to make the sequences of equal length.

### Model Architecture
The model is built using Keras Sequential API. It consists of an embedding layer, a bidirectional LSTM layer, a dense layer, and a dropout layer. The model is trained using the categorical cross-entropy loss function and the Adam optimizer.

### Training
The training data is split into training and validation sets using train_test_split from Scikit-learn. The model is trained for 50 epochs with a batch size of 64. The best model is saved using ModelCheckpoint from Keras.

### GloVe Embeddings
Pre-trained GloVe embeddings are used to initialize the embedding layer. The glove.twitter.27B.100d.txt file is used, which contains word embeddings of 100 dimensions.

