# Book Recommendation System using K-Nearest Neighbors (KNN)

This project implements a **book recommendation system** using the **Book-Crossings dataset** and **K-Nearest Neighbors (KNN)** algorithm. It finds books similar to a given book based on user ratings.

The notebook is designed for **FreeCodeCamp Machine Learning Certification Challenge 3**.

---

## Project Files

- `fcc_book_recommendation_knn.ipynb` – Jupyter Notebook containing:
  - Data preprocessing
  - KNN model training
  - `get_recommends()` function to get 5 similar books
  - Testing and visualization
- `README.md` – Project description and instructions

---

## Dataset

The project uses the **Book-Crossings dataset**:

- **Books file:** `BX-Books.csv` (ISBN, Title, Author)  
- **Ratings file:** `BX-Book-Ratings.csv` (User-ID, ISBN, Rating)

The dataset contains **1.1 million ratings**, **270,000 books**, and **90,000 users**.  

For statistical significance, the notebook filters:
- Users with less than 200 ratings
- Books with less than 100 ratings

---

## How to Run

### Option 1: Run in Google Colab (Recommended)

1. Open the notebook `fcc_book_recommendation_knn.ipynb` in Google Colab.
2. Run all cells sequentially:
   - Install necessary packages (Colab usually has all required packages like `pandas`, `numpy`, `scipy`, `sklearn`).
   - Download and unzip dataset using included commands in the notebook.
   - Preprocess the data and train the KNN model.
   - Use `get_recommends(book_title)` to get 5 recommended books.
3. You can test using the sample book:
   ```python
   books = get_recommends("Where the Heart Is (Oprah's Book Club (Paperback))")
   print(books)
