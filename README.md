

# Movie Recommendation System

This project is a content-based movie recommendation system that suggests movies based on a selected movie's content features. The backend code is implemented in Jupyter, while the frontend is developed using PyCharm with Streamlit for the user interface.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Frontend Development](#frontend-development)
- [Running the Application](#running-the-application)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction
The Movie Recommendation System provides personalized movie recommendations based on the content of movies. It leverages metadata such as genres, cast, crew, and keywords to calculate the similarity between movies and recommend similar ones.

## Dataset
The dataset used contains information about movies, including their metadata. The data is preprocessed and stored in the project folder for use in the recommendation algorithm.

## Project Structure
The project repository contains the following main folders and files:

- `Jupyter/`: Contains the Jupyter notebook for data preprocessing and model development.
  - `MovieRecommendation.ipynb`: Jupyter notebook with the backend code.
  - `datasets/`: Folder containing the movie datasets.
  - `similarity.pkl`: Pickle file containing the precomputed similarity matrix.
- `PyCharm/`: Contains the PyCharm project for frontend development.
  - `app.py`: Streamlit application for the user interface.
  - `requirements.txt`: List of Python dependencies.
  - `pickle files/`: Folder containing serialized model files (pickle format).

## Installation
To run this project locally, follow these steps:

### Backend (Jupyter)
1. Ensure you have Python and Jupyter Notebook installed.
2. Install the required libraries using pip:

```bash
pip install pandas numpy scikit-learn
```

### Frontend (PyCharm)
1. Ensure you have Python and PyCharm installed.
2. Navigate to the `PyCharm` directory.
3. Install the required libraries using pip:

```bash
pip install -r requirements.txt
```

## Data Preprocessing
The data preprocessing steps include:

- Loading the movie dataset.
- Extracting relevant features such as genres, cast, crew, and keywords.
- Creating a similarity matrix using cosine similarity.

These steps are implemented in the `MovieRecommendation.ipynb` notebook.

## Modeling
The content-based recommendation model calculates the similarity between movies using their metadata. The similarity matrix is stored in the `similarity.pkl` file to speed up the recommendation process.

## Frontend Development
The frontend of the application is developed using Streamlit. It provides a user-friendly interface for selecting a movie and viewing recommendations.

### Key Features:
- Movie selection dropdown.
- Display of recommended movies with their posters and details.

## Running the Application
To run the application, follow these steps:

1. Start the Jupyter Notebook and run the `MovieRecommendation.ipynb` to preprocess data and generate the similarity matrix.
2. Navigate to the `PyCharm` directory.
3. Run the Streamlit application:

```bash
streamlit run app.py
```

4. Open the provided URL in your web browser to interact with the application.

## Conclusion
This Movie Recommendation System effectively suggests movies based on content similarity, providing a personalized experience for users. Future improvements could include incorporating user ratings and hybrid recommendation techniques.

