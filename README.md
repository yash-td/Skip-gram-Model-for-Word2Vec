# Skip-gram-Model-for-Word2Vec
Training a skip-gram neural network model to obtain word embeddings. 

Pre-Processing
To pre-process the data I have performed the following operations:-
1) Removing stop words using the NLTK library
2) Converting everything to a lower case
3) Removing the spaces using the strip method in python
3) Removing sentences with length of less than 3
The length of the pre-processed corpus is 13651.

Creating the Corpus Vocabulary and Preparing the Data
Following variables were created in order to create our corpus:-
1)	word2idx - extracting word-index pairs in a list form
2)	idx2word - extracting index-word pairs in a list form
3)	sentAsId - a list all the sentences in our corpus but contains index instead of word

Training the models
1)	The input to the model is the one-hot vector representing the input word whereas the output to the model is a vector containing the probability that a randomly selected nearby word is a word from our vocabulary.
2)	We use the keras framework to import a library which helps us to generate skipgrams. Further while creating a neural network we use the keras.layers to add layers to our neural network and create a model.
3)  The skip-gram approach is considered inefficient because it generates a huge number of weights. The training of a model with such weights and a large vocab-size will take a large amount of time which can be reduced with more advanced and better approaches.

