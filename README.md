
# Book Recommender System Using Machine Learning

This project implements a book recommendation system using machine learning techniques. It analyzes user ratings and book metadata to provide personalized book recommendations.

## Overview

The system uses collaborative filtering and nearest neighbors algorithms to find similar books based on user ratings. It includes:

- Data preprocessing and cleaning of book ratings data
- Creation of a user-item rating matrix 
- Nearest neighbors model to find similar books
- Streamlit web app for interactive recommendations

## Key Components

### Data Processing
- Loads and cleans book ratings and metadata
- Filters for books with sufficient ratings
- Creates a pivot table of user-item ratings

### Machine Learning Model  
- Uses scikit-learn NearestNeighbors algorithm
- Finds similar books based on rating patterns
- Model is trained on the sparse user-item matrix

### Web Application
- Built with Streamlit 
- Allows users to select a book and get recommendations
- Displays book covers and titles for recommendations

## Usage

The main app is in `app.py`. To run:

```
streamlit run app.py
```

Select a book from the dropdown and click "Show Recommendation" to get similar book suggestions.

## Files

- `Book Recommender System.ipynb`: Jupyter notebook with data analysis and model development
- `app.py`: Streamlit web application
- `requirements.txt`: Python dependencies  
- `setup.py`: Package configuration
- `artifacts/`: Saved model and data files

## Future Improvements

- Add content-based filtering using book metadata
- Incorporate more advanced algorithms like matrix factorization
- Allow users to rate books and get personalized recommendations
- Expand the dataset with more recent books and ratings
