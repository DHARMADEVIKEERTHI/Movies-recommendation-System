# 🎬 Movie Recommendation System

## 📖 Overview
This project is a **content-based movie recommendation system** built using **Python**, **Streamlit**, and **Machine Learning** techniques.  
It recommends movies similar to the one selected by the user based on **genre similarity** using **TF-IDF Vectorization** and **Cosine Similarity**.

---

## 🚀 Features
✅ Recommend movies similar to a selected title  
✅ Interactive web interface using **Streamlit**  
✅ Uses **TF-IDF** for text feature extraction  
✅ Computes similarity using **Cosine Similarity**  
✅ Simple and lightweight — works with CSV data  

---

## 🧠 Tech Stack

| Tool | Purpose |
|------|----------|
| **Python** | Programming Language |
| **Streamlit** | Web Application Framework |
| **scikit-learn** | TF-IDF and Cosine Similarity |
| **Pandas** | Data Handling |
| **NumPy** | Numerical Computation |

---

## 📂 Dataset

The project uses two CSV files:  
- `movies.csv` → Contains movie IDs, titles, and genres  
- `ratings.csv` → *(Optional)* Contains user ratings for future collaborative filtering extensions  

**Example structure of `movies.csv`:**
```csv
movieId,title,genres
1,Toy Story (1995),Adventure|Animation|Children|Comedy|Fantasy
2,Jumanji (1995),Adventure|Children|Fantasy
3,Grumpier Old Men (1995),Comedy|Romance
```

---

## 🧩 Project Structure
```
📁 Movie Recommendation System
├── movies.py                 # Streamlit main app
├── movies.csv                # Dataset (movie info)
├── ratings.csv               # Optional dataset (user ratings)
├── python.ipynb              # Model development notebook
└── README.md                 # Project documentation
```

---

## 🧮 How It Works
1️⃣ Load `movies.csv` into a Pandas DataFrame  
2️⃣ Use **TF-IDF Vectorizer** to convert `genres` text into numerical features  
3️⃣ Compute **Cosine Similarity** between movie vectors  
4️⃣ When a user selects a movie, the app recommends the top N most similar ones  

---

## 🧑‍💻 Example Output
**Input:** `Toy Story (1995)`  
**Recommendations:**  
- 1. Emperor's New Groove, The (2000)
- 2. Adventures of Rocky and Bullwinkle, The (2000)
- 3. Toy Story 2 (1999)
- 4. Asterix and the Vikings (2006)
- 5. Antz (1998)
- 6. Wild, The (2006)
- 7. Shrek the Third (2007)
- 8. The Good Dinosaur (2015)
- 9. Monsters, Inc. (2001)

---

## 🌐 Deployment
To deploy on **Streamlit Community Cloud**:  
1. Push your code and data files to GitHub  
2. Go to [streamlit.io/cloud](https://streamlit.io/cloud)  
3. Connect your GitHub repo and choose `movies.py` as the main file  
4. Deploy 🎉

---

## 🏆 Future Improvements
- Add user-based or item-based collaborative filtering  
- Include movie descriptions and tags for better context  
- Integrate TMDb API for fetching posters and metadata  
- Improve UI with movie thumbnails and additional filters   

---

## 🪄 Acknowledgments
Special thanks to the open-source community and datasets used for building and testing this system.
