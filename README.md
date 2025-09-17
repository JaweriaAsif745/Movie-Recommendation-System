# 🎬 Movie Recommendation System

This project is a **Content-Based Movie Recommendation System** built using the TMDB dataset.  
It suggests movies similar to a given movie by analyzing genres, keywords, cast, and director information.

---

## 📂 Dataset
The datasets used come from **TMDB 5000 Movies and Credits**:
- `tmdb_movies.csv` → Movies data (title, overview, genres, keywords, etc.)
- `tmdb_credits.csv` → Credits data (cast and crew details)

---

## ⚙️ Features
- Extracts **genres, keywords, top 3 cast members, and director** from metadata
- Creates a combined **tags column**
- Text preprocessing:
  - Tokenization
  - Stopword removal
  - Stemming (PorterStemmer)
- Converts text into vectors using **CountVectorizer**
- Calculates **cosine similarity** between movies
- Provides **top 5 similar movie recommendations**

---

## 📒 Files in this Repository
- `movie_prediction.ipynb` → Jupyter Notebook with full implementation
- `tmdb_movies.csv.zip` → Movies dataset
- `tmdb_credits.csv.zip` → Credits dataset

---
## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- NLTK (for stemming)  
- Jupyter Notebook  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/JaweriaAsif745/Movie-Recommendation-System.git
   cd movie-recommendation-system
````

2. Install dependencies:

   ```bash
   pip install pandas numpy scikit-learn nltk
   ```

3. Open Jupyter Notebook:

   ```bash
   jupyter notebook movie_prediction.ipynb
   ```

4. Run all cells and try:

   ```python
   recommend("Avatar")
   ```

---

## 📌 Example

Input:

```python
recommend("Avatar")
```

Output:

```
1. Mad Max Beyond Thunderdome (score: 0.259)
2. The Helix... Loaded (score: 0.246)
3. Jupiter Ascending (score: 0.233)
4. Krull (score: 0.228)
5. The Host (score: 0.227)
```

---

## 📜 License

This project is licensed under the MIT License.
