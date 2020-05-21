# Anime-Recommendation-System

<p align="center">
  <img src="Images/anime.png" height="300" width="600">
</p>

## Recommendation Systems

#### "So, if you're a newbie to Recommender Systems i suggest you read through or else you could skip to Dataset Info"

We literally see Recommendation Systems all around us. Online shopping sites like Amazon where products are recommended to us, or media service providers like Netflix or Amazon Prime where movies or tv shows are recommended or social cataloguing websites like goodreads where books are recommended!

<img src="Images/amazon.jpg" width="430" height="200" > <img src="Images/prime.jpg" width="430" height="200">

So how do these people do it!? How are Products, Movies or Books recommended to us in a personalised way?

First, let’s look into the low tech way of doing this!
How do we do it? Friends right! Friends or Cousins or whoever we think have better “taste” in shopping, books or movies than the others, something we’ve learnt over time by observing whether they usually like the same things as you. But is it practical that they would be knowing about everything out there? No.

There comes COLLABORATIVE FILTERING! Making it all pretty practical and easier – the more tech way of doing it!
A collaborative filtering algorithm usually works by searching a large group of people and finding a smaller set with tastes similar to yours. It looks at other things they like and combines them to create a ranked list of suggestions. There are a lot of ways of deciding which people are similar and combining their choices to make a list.

## TYPES OF COLLBORATIVE FILTERING

![](Images/types.jpg)

In this project we're using Memory-Based Filtering technique.
  1. User Based
  2. Item Based

User Based           |  Item Based
:-------------------------:|:-------------------------:
<img src="Images/user.png" width="300" height="300" >  | <img src="Images/item.jpg" width="300" height="300"> 

## Dataset Info

This data set contains information on user preference data from 73,516 users on 12,294 anime. Each user is able to add anime to their completed list and give it a rating and this data set is a compilation of those ratings.

Here's the link to the Kaggle Dataset ==> https://www.kaggle.com/CooperUnion/anime-recommendations-database

## Content

It has 2 files.

1. Anime.csv
    * anime_id - myanimelist.net's unique id identifying an anime.
    * name - full name of anime.
    * genre - comma separated list of genres for this anime.
    * type - movie, TV, OVA, etc.
    * episodes - how many episodes in this show. (1 if movie).
    * rating - average rating out of 10 for this anime.
    * members - number of community members that are in this anime's "group".
2. Rating.csv
    * user_id - non identifiable randomly generated user id.
    * anime_id - the anime that this user has rated.
    * rating - rating out of 10 this user has assigned (-1 if the user watched it but didn't assign a rating).

As the file is too large, you wont find the file uploaded here. Instead here's the drive link to the files!

https://drive.google.com/open?id=1_hZA7JmXp67tqSUL95Eq_wsX9FInCEXK


## Outputs

### Using User Based

1. Euclidean Distance 

  * Input(user_id) :
  
    top_rec,user = recommendations(preferences,1)

  * Output:
  
  <img src="Images/euclidean-output.png">

2. Pearson Correlation

  * Input(user_id) :
  
    top_rec,user = recommendations(preferences,1)

  * Output:
  
  <img src="Images/pearson-output.png">

### Using Item Based

Cosine Similarity

  * Input(anime_id)
  
  * Output:
  
  <img src="Images/item-output.png">

## Conclusion

We have outputs for both User Based and Item Based Collaborative Filtering above.

Which recommends better?

User-based filtering is expected to be superior when dealing with big amounts of data, whereas item-based collaborative filtering is expected to perform better on smaller datasets. :)






