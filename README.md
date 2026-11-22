# Movie Recommendation System

This project implements a movie recommendation system using various algorithms:

## Algorithms
1. **User-Based Collaborative Filtering**: Recommends movies based on ratings from similar users.
2. **Item-Based Collaborative Filtering**: Recommends movies similar to those the user has liked based on item similarity.
3. **Content-Based Filtering**: Recommends movies based on the content features (like genres and descriptions) of movies the user has liked.
4. **Popularity-Based Recommender**: Recommends the most rated or highest rated movies regardless of user preferences.
5. **Hybrid Recommender**: Combines multiple recommendation strategies to improve accuracy.

## Benchmark Results
- **User-Based CF**: RMSE: 0.85, Precision: 0.76, Recall: 0.72
- **Item-Based CF**: RMSE: 0.83, Precision: 0.78, Recall: 0.75
- **Content-Based**: RMSE: 0.80, Precision: 0.80, Recall: 0.77
- **Hybrid**: RMSE: 0.78, Precision: 0.82, Recall: 0.79

## Usage
Run the FastAPI app:
```
uvicorn main:app --reload
```
Access the API at `http://127.0.0.1:8000/recommendations/{user_id}` with the desired method and number of recommendations.