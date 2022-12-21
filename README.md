# Movie-Recommendation-System
## **Introduction**

<img align="right" width="350" src="img/Netflix.jpg">

Online streaming platforms like **Netflix** have plenty of movies in their repository and if we can build a **Recommendation System** to recommend **relevant movies** to users, based on their **historical interactions**, this would **improve customer satisfaction** and hence, it will also improve the revenue of the platform. The techniques that we will learn here will not only be limited to movies, it can be any item for which you want to build a recommendation system.

## **Objective**

In this project we will be building various recommendation systems: 
- Knowledge/Rank based recommendation system
- Similarity-Based Collaborative filtering
- Matrix Factorization Based Collaborative Filtering

we are going to use the **ratings** dataset. 

## **Dataset**

The **ratings** dataset contains the following attributes: 
- userId
- movieId
- rating
- timestamp

## **Exploring the dataset**
The distribution of ratings is showed:

<img align="center" width="650" src="img/Distribution Rating.jpg">

As per Histogram, **Rating '4'** has **highest count** of ratings (>28000).Rating '3' being second with 20000 + and Rating '5' being third in count of ratings with a little over 15000. The ratings are biased towards 4,3 & 5 more than 1,2.

**Write your Answer here:**
- User-based and Item-based Collaborative Models have nearly same. User based RMSE values (0.9925) while the "Item based" model's RMSE is 1.003. Clearly, tuned Collaborative Filtering Models gives similar baseline model and the user-user based tuned model is performing better and have  rmse of 0.9808
 
- The Collaborative Models use the user-item-ratings data to find similarities and make predictions rather than just predicting a random rating based on the distribution of the data. 
 
- Collaborative Filtering searches for neighbors based on similarity of item (example) preferences and recommend items that those neighbors interacted while Matrix factorization works by decomposing the user-item matrix into the product of two lower dimensionality rectangular matrices.
 
- RMSE for Matrix Factorization (0.92) is better than the Collaborative Filtering Models (0.99).

- Tuning SVD matrix factorization model is not improving much the base line SVD. 

- Matrix Factorization has lower RMSE due to the reason that it assumes that both items and users are present in some low dimensional space describing their properties and recommend a item based on its proximity to the user in the latent space. Implying it accounts for latent factors as well.

### **Conclusions**
In this case study, we saw three different ways of building recommendation systems: 
- rank-based using averages
- similarity-based collaborative filtering
- model-based (matrix factorization) collaborative filtering

I also understood advantages/disadvantages of these recommendation systems and when to use which kind of recommendation systems. Once we build these recommendation systems, we can use **A/B Testing** to measure the effectiveness of these systems.
