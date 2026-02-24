# 🎬 Netflix-Style Movie Recommendation System

A Hybrid Movie Recommender inspired by Netflix that suggests movies using **Content-Based Filtering + Personalized Recommendation Logic**.

Implemented in: **`Movie Recommmendation system.ipynb`**

---

## ✨ Features

* Cleaned and preprocessed movie dataset
* Genre-based Content Recommendation
* Cosine Similarity Engine
* Personalized Hybrid Recommendations (Netflix-style)
* Cold-start friendly (works without ratings)
* Simple, fast, and extensible

---

## 📂 Project Structure

```
Movie-Recommendation-System/
│
├── Movie Recommmendation system.ipynb   # Main notebook (full pipeline)
├── movies.csv                           # Raw dataset
├── clean_movies.csv                     # Cleaned dataset (generated)
├── README.md                            # Documentation
└── requirements.txt                     # Dependencies
```

---

## ⚙️ How It Works

### 1. Data Cleaning

* Removed duplicates
* Handled missing values
* Normalized genres
* Converted genre string → list
* Encoded genres using MultiLabelBinarizer

### 2. Feature Engineering

* Created binary genre matrix
* Each movie represented as genre vector

### 3. Content-Based Recommendation

* Computed Cosine Similarity between movies
* Recommends movies similar to selected movie

### 4. Hybrid Netflix-Style Recommendation

* Takes user watch history
* Aggregates similarity scores
* Filters watched movies
* Returns personalized Top-N recommendations

---

## 🚀 Getting Started

### Install Dependencies

```bash
pip install pandas numpy scikit-learn
```

### Run the Notebook

1. Open Jupyter Notebook / Google Colab
2. Open:

```
Movie Recommmendation system.ipynb
```

3. Run all cells sequentially
4. Test recommendation function

---

## 💡 Example

```python
recommend_movies("Toy Story (1995)")
```

Output → List of similar movies

---

## 📊 Future Improvements

* Add Collaborative Filtering (SVD / Matrix Factorization)
* Use real ratings dataset (userId, movieId, rating)
* Popularity & Trending ranking
* Deep Learning Recommender (Neural CF)
* Deploy as Web App (Streamlit / Flask)
* Convert to REST API

---

## 🧠 Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Cosine Similarity
* MultiLabelBinarizer

---

## 🎯 Use Cases

* Movie streaming recommendation
* Recommender systems learning
* Machine Learning academic project
* Resume / portfolio project

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

---

## 📜 License

This project is open-source and available for educational use.

---

## ⭐ If you like this project

Give it a star on GitHub and feel free to fork!
