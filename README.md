# Netflix_Movie_Recommendation_Project
Netflix Movies and TV Shows Recommendation Unsupervised ML Clustering Model

## Project Summary
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.
It will be interesting to explore what insights can we obtain and use it to recommend top choice movies to our users.
We start with understanding the data set, then we clean the data to make analysis ready. We performed textual data preprocessing using NLTK to build a content-based recommendation system using textual attributes from the data.
We implemented K-mean clustering algorithm, used the elbow method, silhouette score and Hierchial clustering to find optimal number of clusters and recommended movies using cosine similarity.

Our objective was to cluster shows based on their similarities and differences, with the ultimate goal of creating a content-based recommender system that recommends 5 shows to users based on their viewing history.

We began our exploration with a dataset consisting of 7787 records and 11 attributes, with a focus on missing value imputation and exploratory data analysis (EDA). The analysis revealed that Netflix has a greater number of movies than TV shows, with a rapidly growing collection of shows from the United States.

To cluster the shows, we selected six key attributes: director, cast, country, genre, rating, and description. These attributes were transformed into a 9000-feature TFIDF vectorization, and Principal Component Analysis (PCA) was used to address the curse of dimensionality. We captured more than 80% of the variance by reducing the components to 2500.

Next, we used K-Means and Agglomerative clustering algorithms to group the shows. The elbow method and Silhouette score analysis confirmed that the optimal number of clusters was 7 for K-Means. However, Agglomerative clustering suggested 5 clusters, which we visualized with a dendrogram.

We continued our efforts by creating a content-based recommender system using the similarity matrix obtained through cosine similarity. This system offers personalized recommendations based on the type of show the user has watched and provides the user with 5 top-notch suggestions to explore.


## Insights derived
![image](https://github.com/GeetanjliRC/Netflix_project_unsuper/assets/91873936/4c837848-7346-420b-b133-3175ca9c1a9e)

![image](https://github.com/GeetanjliRC/Netflix_project_unsuper/assets/91873936/d8fc57f9-2bd3-4c9a-a7e0-a0dc63e56d38)

![image](https://github.com/GeetanjliRC/Netflix_project_unsuper/assets/91873936/fc877f6b-dfdf-48ef-93dc-a7c1ae3d73ab)

![image](https://github.com/GeetanjliRC/Netflix_project_unsuper/assets/91873936/c3964bcb-59fc-4c31-8bcb-2aa626bb6444)

![image](https://github.com/GeetanjliRC/Netflix_project_unsuper/assets/91873936/2e457603-dfad-4dad-b759-b0f8c3ea6a87)




