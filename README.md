🎬 Genre-Based Movie Recommendation System (Using k-Nearest Neighbors)

Overview
This project is a Genre-Based Movie Recommendation System built using the k-Nearest Neighbors (k-NN) algorithm. The system recommends movies based on similar genres, IMDb ratings, and votes from a dataset of movies. It’s a simple yet powerful content-based recommendation engine designed to suggest movies with similar characteristics to the one a user selects.

---

Features
- Movie Recommendations: Recommends movies similar to a selected movie based on genre, IMDb rating, and number of votes.
- k-Nearest Neighbors (k-NN): Uses the k-NN algorithm to find and suggest the most similar movies in the dataset.
- User Input: Allows users to input a movie name and returns recommendations of similar movies.
- Easy to Run: Straightforward and beginner-friendly implementation, using popular Python libraries.

---

How It Works
The system identifies similar movies using:
- Genre: One-hot encoding of the genre field to quantify the similarity between movies.
- IMDB Rating: Numeric data to match movies based on user ratings.
- Votes: Popularity measure based on the number of votes a movie has received.

The k-Nearest Neighbors (k-NN) algorithm then calculates the distance between movies, recommending the closest (most similar) ones.

---

Dataset
The dataset used in this project contains the following fields for each movie:
- Movie Name
- Release Year
- Duration
- IMDB Rating
- Metascore
- Vote
- Genre
- Director
- Cast
- Gross

Sample Dataset
| Movie Name        | Release Year | IMDB Rating | Votes  | Genre      | Director     |
|-------------------|--------------|-------------|--------|------------|--------------|
| The Dark Knight   | 2008         | 9.0         | 2300000| Action     | Christopher Nolan |
| Inception         | 2010         | 8.8         | 2100000| Sci-Fi     | Christopher Nolan |
| Forrest Gump      | 1994         | 8.8         | 1800000| Drama      | Robert Zemeckis |

---

Tech Stack
- Python
- pandas for data manipulation
- scikit-learn for implementing the k-NN algorithm
- numpy for numeric operations
- Jupyter Notebook for development

---

Installation and Setup

Prerequisites
Ensure that you have Python installed on your machine. You can download Python from [here](https://www.python.org/downloads/).

Steps to Run the Project:
1. Clone the Repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-knn.git
   ```
   
2. Navigate to the Project Directory:
   ```bash
   cd movie-recommendation-knn
   ```

3. Install the Required Libraries:
   Install the dependencies listed in the `requirements.txt` file:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

5. Open the Notebook:
   Open the `movie_recommendation_system.ipynb` file to see the code and run the recommendation system.

---

Usage

Once the Jupyter Notebook is open, follow these steps:

1. Load the Movie Dataset:
   The dataset is already provided in the project files. You can load and explore it in the notebook.

2. Run the Recommendation System:
   - Input a movie name when prompted, and the system will return the top 5 most similar movies.
   - Adjust the number of recommendations (`n_neighbors`) if needed.

---

Example Output
If you input "Inception", the system might recommend movies like:
```
Movies similar to Inception:
1. The Dark Knight
2. Interstellar
3. The Prestige
4. The Matrix
5. Memento
```

---

Project Structure
```bash
.
├── data
│   └── movies_dataset.csv        # Movie dataset
├── movie_recommendation_system.ipynb # Jupyter notebook with the code
├── README.md                     # Project documentation
├── requirements.txt              # List of dependencies
```

---

Future Enhancements
- Integrate user-specific recommendations based on collaborative filtering.
- Expand the dataset to include more features like user reviews or box office performance.
- Add a web interface using Flask or Django for easier user interaction.

---

Contact
For any questions or feedback, feel free to reach out to me at [gupta.pragya2101@gmail.com](mailto:gupta.pragya2101@gmail.com).

---
