# Book Recommendation Engine using KNN 📚

## Project Overview
This project implements a book recommendation system using the K-Nearest Neighbors (KNN) algorithm. By leveraging the Book-Crossings dataset, which contains over 1.1 million ratings for 270,000 books from 90,000 users, the model will recommend similar books based on user preferences.

## Challenge Description
In this challenge, you will create a book recommendation algorithm that takes a book title as input and returns a list of five similar books along with their distance metrics. The algorithm employs the KNN method from `sklearn.neighbors` to evaluate the "closeness" of books based on user ratings.

## Dataset
The project utilizes the Book-Crossings dataset, which can be accessed [here](https://github.com/mayankyadav23/Machine-Learning-with-Python/blob/main/Book%20Recommendation%20Engine%20using%20KNN/BX-Book-Ratings.zip). The dataset includes:
- **1.1 million ratings** on a scale from 1 to 10.
- **270,000 books** rated by **90,000 users**.

### Data Preprocessing
Before building the recommendation system:
1. Import and clean the data.
2. Filter out users with less than **200 ratings** and books with fewer than **100 ratings** to ensure statistical significance.

## Functionality
The main function `get_recommends` will provide book recommendations. The function is defined as follows:

```python
def get_recommends(book_title):
    # Implementation of the recommendation algorithm
