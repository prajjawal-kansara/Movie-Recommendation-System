# Movie Recommendation System
A web-based movie recommendation system that suggests movies based on user input, using machine learning for similarity matching. This project leverages HTML, CSS, jQuery, Flask, and machine learning models to provide an engaging and interactive recommendation experience.

## Features
- **Movie Recommendation:** Provides movie suggestions based on a selected or entered movie title using a similarity score.
- **Movie Details:** Displays additional details like cast information, IMDb rating, genre, release date, runtime, and user reviews.
- **User Reviews:** Utilizes a natural language processing model to classify IMDb reviews as "Good" or "Bad" based on sentiment analysis.
- **Auto-complete Suggestions:** Shows suggestions while typing a movie name for quick search.

## Technologies Used
- **Frontend:** HTML, CSS, jQuery
- **Backend:** Flask
- **Machine Learning:** Natural Language Processing with a Count Vectorizer and a similarity model using cosine similarity
- **Data:** CSV data file `main_data.csv` containing movie information
- **Web Scraping:** BeautifulSoup for IMDb review extraction

## Installation
**1. Clone the repository:**
```bash
git clone https://github.com/username/movie-recommendation-system.git
```

**2. Install the dependencies:**
```bash
pip install -r requirements.txt
```

**3. Ensure you have the following files in the project directory:**
- `main_data.csv` (dataset of movies)
- `nlp_model.pkl` and `tranform.pkl` (trained NLP model and vectorizer)

**4. Run the application:**
```bash
python main.py
```

**5. Access the web application at `http://127.0.0.1:5000`.**

## Usage
- **Home Page:** Enter a movie title to receive recommendations.
- **Recommendation Page:** Shows similar movies and details like cast and crew, reviews, and rating.
- **Review Classification:** Reviews are categorized as Good or Bad based on sentiment.

## How It Works
1. **Recommendation:** The system creates a similarity matrix based on movie features and suggests the top ten similar movies.
2. **Sentiment Analysis:** Each review is classified as "Good" or "Bad" based on the sentiment prediction from the trained NLP model.

## Acknowledgments
This project uses data from IMDb for movie details and reviews.
