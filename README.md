# Book-Recommendation-System
* This project is all about recomendation system.In this project we tried to use some approches for recomending the books to the readers or users .We used various ways such as collaborative Filtering and Content-based Filtering for recomendation of the books to the users 

**ABOUT THE DATASET :** We have three diffrent datsets namely Books.csv which contains information about the books such as book-author , publisher , book title , year of publication, image links and unique Book ID i.e ISBN Number .Then we have Ratings.csv which contain information about ratings given by the users for the books, it contains user ID ,ISBN number and book rating (scale between 1-10). Then we have Users.csv which contain information about users such as their location , age and their user ID 

**EDA :** For the EDA part we have analysed the top Books rated by the users , top authors who got most ratings , top authors on the basis of number of books , Top publishers who have published maximum number of books, we have analysed the users age and lastly we have analysed their ratings we got that most of the users have rated 8.

**Recomendation Approaches :**

*  Collaborative Filtering

   In Collaborative Filtering we make predictions of the taste or the intrests of the user based based on the other similar users behaviour (which is called collaborative) .The simple understanding is that if a person P1 have similar opinion with person P2 , then if person P1 is reading Harry Potter books then person P2 may also read Harry Potter books

   Collaborative Filtering has mainly two implimentaion strategies
   *   Model Based
   *   Memory Based

We have used the following approaches

   Memory based
   *  User_based Collaborative Filtering 

      *In this technique we try to predict on basis of what user may like based on the ratings that they had given to the items. In simpe words here we try to indentify the neghbouring users on the basis of similarity of active users and then scoring of the items  is calculated on the basis of those neighbour users* 
   *  Item_based Collaborative Filtering

      *In Item based collaborative filtering we try to find similar items based on the items whichs user has liked or interacted with .It suggests an item based on items the user has previously consumed. It looks for the items the user has consumed then it finds other items similar to consumed items and recommends accordingly*


   Model based Collaborative Filtering Approach
   * Singular value decomposition(SVD)

     *It is a popular method in field of Data Science and Machine Learning .It is a classical method from the Linear Algebra concept. It is popular beacuse of its properties and its use in Recomendation System. We can use this in recomending Books, movies etc.*

     *SVD is a method from linear algebra that has been generally used as a dimensionality reduction technique in ML problems. It is amtrix Factorisation technique which tries to reduce the number of feature or attributes by reducing the sapce dimension from N dimension to I dimension.SVD is used as a collaborative filtering technique in recomendation technique domain. It consist of a matrix structure where the rows define the users and columns defines the item.*


  * Non-Negetive Matrix Factorisation(NMF): 
  
    *Our goal in NMF is to approximate the users-item V matrix by the dot product of two arrays W and H. Dimensions of the arrays are defined by dimensions of V and number of components we set to the algorithm. If V has n rows and m columns and we want to decompose it to k components, then W has n rows, and k columns and H has k rows and m columns.This is actually matrix factorization part of the algorithm. The Non-negative part refers to V, W, and H — all the values have to be equal or greater than zero, i.e., non-negative*
   


**Content based Filtering :**
  
   It is type of recomendation system which depends upon the data which we get from the customers , based on the data a user profile is generated
