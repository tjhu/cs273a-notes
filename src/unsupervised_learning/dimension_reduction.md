# Dimensionality Reduction

can be used for

- data compression
- noise removal
- supervised learning

## Principal Components Analysis

- subtract data mean from each point
- scale each dimension by its variance

### PCA Applications

- Eigen face
- LSA: PCA on text for similarity
- Non-linear latent space
  - Auto-encoder
  - word2vec
- recommendation system
  - PCA can fill in empty spaces
  - can add an user effect term cuz some users always give high ratings
  - can add an item effect term cuz some movies are just bad