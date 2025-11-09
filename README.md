
# Movie Recommendation System

A machine learning-based movie recommendation engine that provides personalized movie suggestions to users based on collaborative filtering and content-based filtering techniques.

## 🎯 Overview

This project implements a comprehensive movie recommendation system using Python and Jupyter Notebook. The system analyzes user preferences, viewing history, and movie features to generate accurate and personalized movie recommendations, helping users discover films tailored to their interests.

### Key Features

- ✅ **Collaborative Filtering**: Recommends movies based on similar users' preferences
- ✅ **Content-Based Filtering**: Suggests movies based on movie features (genre, actors, director)
- ✅ **Cosine Similarity**: Measures similarity between users and items for accurate recommendations
- ✅ **User-Item Matrix**: Efficient representation of user ratings and preferences
- ✅ **K-Nearest Neighbors (KNN)**: Identifies similar users/movies for recommendation generation
- ✅ **Interactive Notebook**: Step-by-step implementation with visualizations

## 📊 Dataset

The project uses the **MovieLens dataset** or similar movie rating datasets containing:

- **User ratings**: Historical user-movie ratings
- **Movie metadata**: Title, genre, year, director, actors, runtime
- **User information**: User demographics and preferences

## 🚀 Installation

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook
- pip package manager

### Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/Ishu-2820/Movie_Recommendation_System-
   cd Movie_Recommendation_System-
   ```

2. **Create a virtual environment** (recommended)

   ```bash
   python -m venv venv
   
   # Windows
   venv\Scripts\activate
   
   # macOS/Linux
   source venv/bin/activate
   ```

3. **Install required packages**

   ```bash
   pip install -r requirements.txt
   ```

### Dependencies

```
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
scipy>=1.7.0
```

## 💻 Usage

### Basic Usage

1. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook
   ```

2. **Open the notebook**

   Navigate to `Movie_recommender_system.ipynb` and open it.

3. **Run the cells**

   Execute the cells sequentially to:
   - Load and preprocess the dataset
   - Build the recommendation model
   - Generate movie recommendations

### Example Code

```python
# Get movie recommendations
movie_name = "Inception"
recommendations = get_recommendations(movie_name, n_recommendations=10)

print(f"Movies similar to '{movie_name}':")
for i, movie in enumerate(recommendations, 1):
    print(f"{i}. {movie}")
```

## 📁 Project Structure

```
Movie_Recommendation_System-/
│
├── Movie_recommender_system.ipynb    # Main Jupyter notebook
├── data/                             # Dataset directory
│   ├── movies.csv                    # Movie metadata
│   └── ratings.csv                   # User ratings
│
├── models/                           # Saved models (if any)
├── requirements.txt                  # Python dependencies
├── README.md                         # Project documentation
└── .gitignore                        # Git ignore file
```

## 🔧 Technical Pipeline

### 1. Data Loading and Exploration
- Import movie and rating datasets
- Explore data distributions and patterns
- Analyze user rating behavior

### 2. Data Preprocessing
- Handle missing values
- Filter movies with minimum ratings threshold
- Create user-item rating matrix

### 3. Feature Engineering
- Build user-item interaction matrix
- Extract movie features (genre, year, etc.)
- Calculate similarity scores

### 4. Model Development

**Collaborative Filtering:**
- User-based collaborative filtering
- Item-based collaborative filtering
- K-Nearest Neighbors (KNN) algorithm

**Content-Based Filtering:**
- TF-IDF vectorization of movie features
- Cosine similarity calculation
- Genre and metadata-based recommendations

### 5. Recommendation Generation
- Predict ratings for unseen movies
- Rank movies by predicted rating
- Return top-N recommendations

## 📈 Model Performance

The recommendation system is evaluated using:

- **Mean Absolute Error (MAE)**: Measures prediction accuracy
- **Root Mean Squared Error (RMSE)**: Evaluates prediction error
- **Precision@K**: Accuracy of top-K recommendations
- **Recall@K**: Coverage of relevant recommendations
- **User satisfaction**: Relevance of suggested movies

## 🎨 Visualizations

The notebook includes:

1. **Rating Distribution**: Histogram of user ratings
2. **Popular Movies**: Bar chart of most-rated movies
3. **User Activity**: Distribution of ratings per user
4. **Similarity Matrix**: Heatmap of item-item or user-user similarity
5. **Recommendation Results**: Sample recommendations for test users

## 🎯 Use Cases

- **Streaming Platforms**: Personalized content discovery for Netflix, Amazon Prime
- **E-commerce**: Product recommendations based on viewing history
- **Content Curation**: Automated playlist and watchlist generation
- **User Engagement**: Increase platform usage through relevant suggestions

## 🔮 Future Improvements

### Technical Enhancements

- **Deep Learning Models**: Implement neural collaborative filtering
- **Hybrid Approach**: Combine collaborative and content-based methods
- **Matrix Factorization**: Use SVD or ALS for better scalability
- **Real-time Updates**: Incorporate streaming data for dynamic recommendations
- **Cold Start Problem**: Address new user/item recommendations with meta-learning

### Feature Additions

- **Web Application**: Deploy as a Flask/Streamlit web app
- **User Interface**: Create interactive recommendation dashboard
- **A/B Testing**: Evaluate different recommendation strategies
- **Sentiment Analysis**: Incorporate user reviews for better recommendations
- **Diversity Metrics**: Ensure recommendation diversity and serendipity

### Deployment

- **API Development**: REST API for recommendation service
- **Cloud Deployment**: Host on AWS, Azure, or Heroku
- **Containerization**: Docker support for easy deployment
- **MLOps**: Implement CI/CD for model versioning and monitoring

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- **MovieLens Dataset**: GroupLens Research for providing the dataset
- **Libraries**: scikit-learn, pandas, numpy, matplotlib, seaborn
- **Community**: Thanks to the open-source community for inspiration and support

## 📞 Contact

**Ishu-2820** - [GitHub Profile](https://github.com/Ishu-2820)

⭐ **If you found this project helpful, please give it a star!** ⭐

---

*Last updated: November 2025*
