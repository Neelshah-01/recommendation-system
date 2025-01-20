# Product Recommendation System

Problem statement: Design a real-time recommendation system for an e-commerce platform. The system should provide product recommendations based on the user’s recent browsing or purchase history using collaborative filtering or content-based filtering.

Dataset used: https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation/

## Techniques Used in the Recommendation System
### User-Based Collaborative Filtering:
This technique recommends products based on the preferences of users who have similar interaction patterns.

- Cosine Similarity is used to compute the similarity between users based on their product interactions.
- Products that similar users have interacted with, but the target user has not, are recommended.
- This approach leverages actual user-item interaction data to identify and recommend relevant products.

### Model-Based Collaborative Filtering using Singular Value Decomposition (SVD):
This technique uses matrix factorization to identify latent features in the user-item interaction matrix.

- The SVD algorithm decomposes the interaction matrix into three components (U, Sigma, Vt), representing users, latent features, and products.
- The reconstructed matrix predicts the interaction scores between users and products.
- Products are recommended by ranking predicted scores for items that the user has not yet interacted with.
