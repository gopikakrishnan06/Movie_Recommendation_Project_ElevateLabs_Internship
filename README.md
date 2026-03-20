Movie Recommendation System
Overview
This project is a Movie Recommendation System built using Machine Learning techniques on the MovieLens dataset. It suggests movies to users based on their preferences by combining:
●	Collaborative Filtering
●	Content-Based Filtering
●	Hybrid Recommendation Approach
The system takes user input and returns the Top 5 personalized movie recommendations.

Features
●	Data preprocessing and cleaning
●	User-item matrix creation
●	Collaborative filtering using SVD (Matrix Factorization)
●	Content-based filtering using movie genres
●	Hybrid recommendation system
●	Simple interactive UI using ipywidgets (Colab)

Dataset
●	MovieLens Latest Small Dataset
●	Contains:
○	Movies metadata (title, genres)
○	User ratings


Technologies Used
●	Python 
●	Pandas & NumPy
●	Scikit-learn
●	ipywidgets (for UI in Colab)

STEPS
1. Data Preprocessing
●	Clean and split genres
●	Convert genres into numerical format using MultiLabelBinarizer
●	Merge movies and ratings datasets
2. Collaborative Filtering
●	Create a user-item matrix
●	Apply Truncated SVD
●	Predict missing ratings
3. Content-Based Filtering
●	Use cosine similarity on genre features
●	Recommend similar movies based on selected movie
4. Hybrid Model
●	Combine results from:
○	Collaborative filtering
○	Content-based filtering
●	Return top 5 recommendations

User Interface
●	Input:
○	User ID
○	Favorite Movie
●	Output:
○	Top 5 recommended movies

How to Run
1.	Open Google Colab
2.	Copy and paste the full code
3.	Run all cells
4.	Enter:
○	User ID (e.g., 1)
○	Favorite movie (e.g., Toy Story (1995))
5.	Click Recommend

Sample Output
Top 5 Recommendations:
1.	Movie A
2.	Movie B
3.	Movie C
4.	Movie D
5.	Movie E
Future Improvements
●	Add movie posters using TMDB API
●	Improve recommendations using Deep Learning
●	Build a web app using Streamlit or Flask
●	Add search dropdown for better UX
