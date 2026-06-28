# 🎵 Spotify Music Recommendation System

A **Content-Based Music Recommendation System** built with **Python**, **Scikit-learn**, and **Natural Language Processing (NLP)** that recommends similar Spotify tracks based on textual metadata using **TF-IDF Vectorization** and **Cosine Similarity**.

The project analyzes Spotify music data, visualizes category distributions, and suggests songs that share similar characteristics, making music discovery more personalized and efficient.

---

# 📌 Overview

With millions of tracks available on music streaming platforms, discovering songs that match a listener's preferences can be challenging. This project demonstrates how a **content-based recommendation engine** can suggest similar songs by analyzing textual features such as song titles, genres, artists, playlists, or other metadata available in the dataset.

Instead of relying on user listening history, the system identifies relationships between songs based on their content, making it effective even for new users.

---

# 🚀 Features

* 🎵 Content-Based Song Recommendation
* 🔍 Similar Track Discovery
* 📊 Interactive Spotify Category Visualization
* 🧠 TF-IDF Text Vectorization
* 📐 Cosine Similarity Matching
* ⚡ Fast Recommendation Retrieval
* 📈 Exploratory Data Analysis using Plotly

---

# 📂 Dataset

The project uses a Spotify dataset containing song metadata.

Typical columns include:

| Column           | Description                                        |
| ---------------- | -------------------------------------------------- |
| Title            | Song title                                         |
| Artist           | Artist name                                        |
| Spotify Category | Playlist, genre, or category                       |
| Features         | Combined textual metadata used for recommendations |

> **Note:** The exact columns may vary depending on the dataset version.

---

# 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Plotly
* TF-IDF Vectorizer
* Cosine Similarity

---

# 🧠 How It Works

## 1. Load the Dataset

The Spotify dataset is imported into a Pandas DataFrame for analysis.

---

## 2. Explore Music Categories

The distribution of Spotify categories is visualized using an interactive Plotly bar chart, providing insights into the diversity of the music catalog.

---

## 3. Feature Engineering

Relevant song metadata is combined into a single textual feature. The text is then transformed into numerical vectors using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

TF-IDF highlights distinctive words while reducing the influence of common terms.

---

## 4. Compute Song Similarity

The recommendation engine calculates **Cosine Similarity** between TF-IDF vectors to measure how closely songs are related.

Similarity scores range from **0** (completely different) to **1** (highly similar).

---

## 5. Recommend Similar Songs

When a user selects a song:

1. The system locates the selected track.
2. Computes similarity scores with all other songs.
3. Sorts songs by similarity.
4. Returns the top recommended tracks.

---

# 📊 Visualizations

The project generates:

* 📈 Spotify Category Distribution
* 🎵 Top Similar Song Recommendations

---

# 📁 Project Structure

```text
Spotify-Recommendation-System/
│
├── data/
│   └── spotify_dataset.csv
│
├── recommendation.py
├── spotify_recommendation.ipynb
├── requirements.txt
└── README.md
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/Spotify-Recommendation-System.git
```

Navigate to the project directory:

```bash
cd Spotify-Recommendation-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook or Python script.

---

# 📦 Required Libraries

```text
numpy
pandas
scikit-learn
plotly
```

Or install manually:

```bash
pip install numpy pandas scikit-learn plotly
```

---

# 💻 Example Usage

```python
recommendations = recommend_music("Blinding Lights")

print(recommendations)
```

Example Output:

```text
Save Your Tears
Starboy
Less Than Zero
After Hours
Die For You
```

---

# 🧩 Recommendation Technique

This project uses **Content-Based Filtering**, where recommendations are generated based on song metadata rather than user behavior.

The workflow consists of:

* Feature Extraction using TF-IDF
* Similarity Computation using Cosine Similarity
* Ranking Songs by Relevance

This approach performs well even when user interaction history is unavailable.

---

# 🎯 Learning Outcomes

This project demonstrates practical experience with:

* Recommendation Systems
* Natural Language Processing (NLP)
* Content-Based Filtering
* TF-IDF Vectorization
* Cosine Similarity
* Exploratory Data Analysis (EDA)
* Interactive Data Visualization
* Python for Machine Learning

---

# 🔮 Future Improvements

* Integrate Spotify Web API for live recommendations
* Use audio features such as danceability, energy, valence, and tempo
* Replace TF-IDF with transformer-based embeddings
* Build an interactive web application using Streamlit
* Add artist- and genre-based filtering
* Deploy the recommendation engine as a REST API using FastAPI

---

# 🤝 Contributing

Contributions are welcome! If you have ideas for improvements or new features, feel free to fork the repository, create a feature branch, and open a Pull Request.

---

# 📜 License

This project is licensed under the MIT License.

---

# ⭐ Support

If you found this project useful, consider giving it a **⭐ Star**. Your support helps others discover the project and encourages future improvements.
