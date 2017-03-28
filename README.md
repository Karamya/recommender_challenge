# Recommender Challenge



The data contains information about the user and his/her purchase history of certain products and the time of purchase. The aim is to create a recommender system that recommends 5 new products that a given customer has not yet purchased. 



## Requirements:



Python 3.5.2 

Pandas 0.19.0

NumPy 1.12.1

PySpark 2.0.0


## Challenges



- Provide good user experience to every user
- Satisfy the business objectives
- Measure its impact
- Scaling
- Expired items
- Cold start - new users, new products
- Sparsity of user preference

## Types of Recommenders



- Content based
    - using explicit features of the users and/or items
- Collaborative filtering
    - implicit features
    - based on observed interactions rather than metadata
- Hybrid

## Alternating Least Square(ALS) - Method of Choice



There are many techniques for generating recommendations, such as
- Matrix factorization
- co-occurrence analysis
- content based filtering
- graph based algorithms
- hybrids

In our case, the given datase contains only implicit features. I choose ALS recommender, which is a widely popular matrix factorization algorithm that uses alternating least squares with weighted lambda regularization. It factors the user-to-item matrix into the user-to-feature matrix and the item-to-feature matrix. This recommendation was also successfully used in the Netflix competition.
One of the big strengths of ALS based recommender, compared to the user or item based recommender, is its ability to handle large sparse data sets and its better prediction performance. It is best suited for our datasets.

———————————————————————————————————————

