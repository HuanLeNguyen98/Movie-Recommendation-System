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
