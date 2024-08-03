
# Data representation design patterns

- embeddings
- number of features
- normalization
    -   zscore
    -   minmax
- boxcox transform to control the heterostoscestact

- dummy encode
- one hot encode

## Hashed feature

- using hashes for possible categorical features
    - deal with the cardinality problem

## Embeddings

- text embeddings
- image embeddings
    - dimension?

# Feature Cross

-  combinations of inputs as separate features
- tf.feature_column.crossed_column()
    - Crossed features will be hashed according to hash_bucket_size. Conceptually, the transformation can be thought of as: Hash(cartesian product of features) % hash_bucket_size

# Multimodal Input

- to combine multiple types of data on input
- strong relations to embeddings
- bag of words
'''
Embeddings add an extra layer to our model and provide extra information about
word meaning that is not available from the BOW encoding. However, embeddings
require training (unless we can use a pre-trained embedding for our problem). While
a deep learning model may achieve higher accuracy, we can also try using BOW
encoding in a linear regression or decision-tree model using frameworks like scikit-
learn or XGBoost. Using BOW encoding with a simpler model type can be useful for
fast prototyping or to verify that the prediction task we’ve chosen will work on our
dataset. Unlike embeddings, BOW doesn’t take into account the order or meaning of
words in a text document. If either of these are important to our prediction task,
embeddings may be the best approach.
'''








