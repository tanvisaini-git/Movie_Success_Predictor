# Movie Success Predictor
Developed as a part of the Modern Analytics class at Duke University's Business Analytics Program. It was a team project created by Akshay Uchila Navada, Mike Shu, Niki Gao, Nina Wu, and Tanvi Saini.

## Overview
The project utilizes is a deep learning model to predict the potential sucess of a movie based on its plot, genre, and other relevant features. By leveraging natural language processing (NLP) with Word2Vec and a neural network, the tool provides IMDb rating predictions. The goal is to offer movie studios and production houses an informed prediction that could guide decisions on whether to proceed with a movie script, ultimately providing valuable insights into the potential success of a film.

## Motivation
The entertainment industry is a high-stakes environment where predicting a movie's success is crucial. With the increasing number of movies being released and screenplays being written each year, a reliable and efficient project evaluation method is essential. This project addresses this need by providing a data-driven approach to predicting IMDb ratings, enabling faster greenlighting of potentially successful projects.

## Data Sources and Feature Engineering

The model utilizes a dataset from Kaggle - https://www.kaggle.com/datasets/gufukuro/movie-scripts-corpus/data

Including:

*   **Script:** Movie Script 
*   **IMDb ID:** Unique identifier for each movie
*   **Title:** Movie title
*   **Plot Summaries:** Textual description of the movie plot.
*   **Keywords:** Relevant keywords associated with the movie.
*   **Genres:** Movie genres (e.g., Action, Comedy, Drama).
*   **Production Companies:** Companies involved in the movie's production.
*   **IMDb User Rating:** Target variable to predict.
*   **Number of IMDb User Votes:** Number of votes received on IMDb.

The following feature engineering techniques were applied:

*   **Textual Features (Plot Summaries and Keywords):** Preprocessed using NLP techniques (tokenization, embedding).
*   **Categorical Features (Genres):** Processed using MultiLabelBinarizer to handle multiple genres per movie.

## Model Architecture
<img src = "https://github.com/tanvisaini-git/Movie_Success_Predictor/blob/main/image.png?raw=true" width = "1000" />

## Predicted Rating Example
<img src = "https://github.com/tanvisaini-git/Movie_Success_Predictor/blob/main/Screenshot%202025-02-25%20032209.png?raw=true" width = "1000" />

## Future Developments and Directions
While the current model focuses on predicting IMDb ratings due to computational constraints, future advancements aim to provide a more comprehensive analysis of movie scripts. By expanding the scope of analysis, the goal is to build a "One-Stop Solution" for movie script evaluation, which would not only assist production houses in making informed decisions but also offer deeper insights into various aspects of filmmaking.

The planned developments include:
* **Expanding Predictive Capabilities:**
  * **Genre Classification:** Automatically categorizing scripts into their respective genres, helping studios understand how well a script fits within a popular or emerging genre
  * **Character Analysis:** Evaluating character depth and dynamics, which could influence audience engagement and the success of the film
  * **Scene-wise Sentiment Analysis:** Understanding the emotional tone of individual scenes to predict audience reactions, which could guide editing and storytelling decisions
  * **Budget and Revenue Prediction:** Estimating the financial performance of a movie based on script features, market trends, and historical data

