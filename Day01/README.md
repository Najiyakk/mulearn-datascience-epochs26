# Netflix Movies & TV Shows Dataset Analysis

## Dataset Overview

This project explores the **Netflix Movies & TV Shows** dataset, which contains information about content available on Netflix. The dataset includes details such as the title, type (Movie or TV Show), director, cast, country, release year, content rating, duration, genre, and description.

The dataset consists of **8,807 records** and **12 columns**. Most columns contain categorical or text data, while `release_year` is the only numerical feature.

---

# Business Problem

Netflix has a large collection of movies and TV shows, making it difficult for users to discover content that matches their interests.

**Business Problem:**

How can Netflix group similar movies and TV shows to improve its recommendation system and help users discover relevant content more easily?

---

# Machine Learning Problem Framing

### Machine Learning Approach

**Clustering (Unsupervised Learning)**

### Justification

Clustering groups similar content based on common characteristics such as genre, description, rating, duration, release year, and country.

Since there are no predefined labels indicating which titles belong together, clustering is an appropriate machine learning approach. The generated clusters can be used to recommend similar movies or TV shows to users.

---

# Target Variable

There is **no target variable** because clustering is an **unsupervised learning** technique.

---

# Key Features

The following features are useful for grouping similar Netflix content:

- `listed_in` (Genre)
- `description`
- `country`
- `rating`
- `duration`
- `release_year`

---

# Dataset Exploration

## Dataset Shape

- Rows: **8,807**
- Columns: **12**

---

## Data Types

- Object (Categorical/Text): **11 columns**
- Integer: **1 column (`release_year`)**

---

## Missing Values

| Column | Missing Values |
|---------|---------------:|
| director | 2634 |
| cast | 825 |
| country | 831 |
| date_added | 10 |
| rating | 4 |
| duration | 3 |

The `director`, `cast`, and `country` columns contain the highest number of missing values and would require preprocessing before building a machine learning model.

---

## Summary Statistics

Some important findings from the dataset include:

- There are **2 content types**: Movie and TV Show.
- **Movie** is the most common content type, with **6,131** titles.
- **United States** is the most represented country, contributing **2,818** titles.
- **TV-MA** is the most common content rating.
- The average release year is **2014**.
- The oldest title was released in **1925**, while the newest titles are from **2021**.

---

# Three Key Observations

### Observation 1

Movies dominate the Netflix catalog, with **6,131 movies** compared to TV Shows.

### Observation 2

The dataset contains missing values, especially in the **director**, **cast**, and **country** columns, indicating that data cleaning is necessary before applying machine learning algorithms.

### Observation 3

Most Netflix content originates from the **United States**, and the average release year is **2014**, showing that the catalog mainly consists of relatively recent content.

---

# Conclusion

The Netflix Movies & TV Shows dataset is suitable for solving recommendation-related business problems. By applying **Clustering**, Netflix can group similar content based on features such as genre, description, rating, duration, and release year. These clusters can improve content discovery and provide users with more personalized recommendations.
