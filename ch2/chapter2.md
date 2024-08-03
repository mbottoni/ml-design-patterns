
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





