# Creating-Cohorts-of-Songs

This project aims to perform exploratory data analysis (EDA) and clustering on songs by **The Rolling Stones** available on Spotify. The goal is to create **cohorts of songs** to enhance Spotify's song recommendation system, providing users with more personalized music experiences.

## Project Description

With over **456 million active users** and more than **195 million paid subscribers** (as of September 2022), Spotify is one of the world's largest music streaming services. To maintain user engagement, Spotify aims to create clusters of songs with similar characteristics, helping users discover songs that align with their preferences.

---

## Steps and Methodology

### 1. Data Inspection and Cleaning
- The dataset was loaded and inspected for any missing values, duplicates, and incorrect entries.
- We cleaned the data by removing duplicates and dropping rows with missing values to ensure a smooth analysis process.

### 2. Exploratory Data Analysis (EDA)
- We explored the dataset using visualizations, focusing on the distribution of song **popularity** and key numeric features.
- A **correlation matrix** was created to analyze the relationships between different features (e.g., energy, danceability, loudness).

### 3. Feature Engineering
- We identified popular albums by analyzing the number of popular songs (those with popularity scores above the median).
- The most popular albums were visualized, providing insights into which albums are the most well-received by listeners.

### 4. Data Preparation for Clustering
- Key numeric features such as **acousticness**, **danceability**, **energy**, etc., were standardized using `StandardScaler` to ensure uniformity across different scales.
- **Principal Component Analysis (PCA)** was applied to reduce the dimensionality of the dataset, making the data more manageable for clustering.

### 5. Clustering
- Using the **Elbow Method** and **Silhouette Scores**, we determined the optimal number of clusters.
- **K-Means Clustering** was applied to group songs into distinct clusters based on their features.
- Finally, we visualized the clusters, providing a clear understanding of the song groupings and their respective characteristics.

---

## Technologies Used

- **Python**
- **Pandas**: For data manipulation and analysis.
- **Seaborn** & **Matplotlib**: For data visualization.
- **Scikit-learn**: For PCA and K-Means clustering.

---

## Results

- The dataset was successfully analyzed, and songs were grouped into **cohorts** using K-Means clustering.
- The number of clusters was determined using both the **Elbow Method** and **Silhouette Score** techniques.
- Songs were visualized in their clusters using **PCA**, making it easy to interpret the similarities between songs based on their features.

---

## Conclusion

By creating clusters of similar songs based on their features, this project demonstrates how Spotify can improve its recommendation engine, offering users more personalized content. The clusters identified in this analysis provide a clear basis for grouping songs with similar musical characteristics, enabling more targeted song recommendations.
