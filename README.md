# RECOMMENDATION-SYSTEM

"COMPANY" : CODTECH

"NAME" : VAISHNAVI NARAYANDAS

INTERN ID : CT04WT240

"DOMAIN" : MACHINE LEARNING

"DURATION": 4WEEKS

"MENTOR" : NEELA SANTOSH

#DESCRIPTION

This project demonstrates the development of a **Recommendation System** using **Collaborative Filtering** and **Matrix Factorization** techniques to suggest movies to users based on their past preferences and the preferences of similar users. Recommendation systems have become a fundamental part of many digital platforms, especially in e-commerce, entertainment, and social media, where personalized content delivery is key to user engagement and satisfaction.

This project is built around the **MovieLens** dataset, a widely used dataset in recommendation system research and education. The system predicts movie ratings for users who haven’t rated them yet and recommends movies they are likely to enjoy based on the patterns extracted from existing user-movie rating interactions.



### Tools and Technologies Used

* **Python**: Programming language used for data analysis and model development.
* **Pandas & NumPy**: Used for data manipulation, loading, and preprocessing tasks.
* **Scikit-learn**: Employed for basic matrix factorization, metrics evaluation, and optional model pipelines.
* **Surprise Library**: A specialized Python library for building and analyzing recommender systems. Used for SVD (Singular Value Decomposition)-based collaborative filtering.
* **Matplotlib & Seaborn**: Used for data visualization and analysis of recommendation results.
* **Jupyter Notebook**: The primary development and analysis environment. It allows for code execution, visualization, and markdown documentation in a structured format.
* **VS Code (Optional)**: Can also be used for writing and running code via Python and Jupyter extensions.



### Dataset Description

The project utilizes the **MovieLens Small Dataset** (`ml-latest-small`) from [GroupLens](https://grouplens.org/datasets/movielens/). This dataset contains:

* **Ratings.csv**: User IDs, Movie IDs, Ratings, and Timestamps.
* **Movies.csv**: Movie IDs and their corresponding titles and genres.

The dataset includes:

* 100,836 ratings
* 9,742 movies
* 610 users

This makes it an ideal dataset for testing collaborative filtering techniques due to its realistic structure and manageable size.



### Project Workflow

1. **Data Loading and Exploration**:

   * Loaded `ratings.csv` and `movies.csv` files using Pandas.
   * Explored user activity, rating distributions, and popular movies.

2. **Data Preprocessing**:

   * Merged movie titles with user ratings.
   * Filtered data to include only active users and frequently rated movies for better matrix density.
   * Split data into training and testing sets for performance evaluation.

3. **Model Building – Collaborative Filtering**:

   * Implemented **Matrix Factorization using Singular Value Decomposition (SVD)** via the `Surprise` library.
   * Trained the model on existing user-movie ratings.
   * Used the model to predict ratings for unseen combinations (user, movie).

4. **Recommendation Generation**:

   * For a given user, recommended top-N movies with the highest predicted ratings that the user hasn’t rated yet.
   * Displayed recommendations using movie titles and genres for clarity.

5. **Performance Evaluation**:

   * Evaluated model performance using:

     * **Root Mean Squared Error (RMSE)**
     * **Mean Absolute Error (MAE)**
   * These metrics indicate how accurately the system predicts unseen ratings.
   * Also visualized prediction distributions to understand the system’s bias.



### Results and Observations

The model achieved low RMSE and MAE values, showing that SVD-based collaborative filtering is effective for predicting user preferences. Sample recommendation results for specific users demonstrated good alignment with their historical tastes. For instance, users who rated action movies highly received recommendations from similar genres.

A few key findings:

* Users with more historical data receive more personalized and accurate recommendations.
* Cold-start problems (new users or new movies) still pose a challenge unless hybrid models are used.



### Applications of Recommendation Systems

Recommendation systems are core to many modern digital services:

* **Streaming platforms** (e.g., Netflix, YouTube): Recommend videos/movies based on viewing history.
* **E-commerce** (e.g., Amazon, Flipkart): Recommend products based on previous purchases or views.
* **Social media** (e.g., Instagram, Facebook): Recommend content, people, and groups.
* **Music platforms** (e.g., Spotify, Gaana): Recommend playlists and new tracks.

This project provides the foundational knowledge to build more advanced recommenders, including hybrid models, content-based filtering, or even deep learning-based recommenders.



### Conclusion

This project provides a robust and interpretable implementation of a **Movie Recommendation System** using **Collaborative Filtering** and **Matrix Factorization (SVD)** within a **Jupyter Notebook** environment. It showcases how to extract patterns from sparse rating data to deliver meaningful recommendations and evaluate model accuracy using industry-standard metrics. With a clean modular structure, the notebook is ideal for learning, experimenting, and expanding toward production-grade recommender systems.

