# Movie Genre Classification for Film Festival I'm Part Of

This project analyzes movie submissions downloaded from FilmFreeway to categorize films for film festivals. It classifies movies into genres based on their titles and synopses, utilizing a language model to identify applicable genres while allowing for existing genre data in the CSV file.

## Features

- **Genre Classification**: Automatically classifies movies into genres such as Scary, Drama, Fantasy, and Comedy. This can be easily changed to suit one's needs. 
- **CSV Input**: Reads movie data from a CSV file downloaded directly from FilmFreeway, including project titles, synopses, project types, and existing genres.
- **Document Generation**: Outputs the results into a well-formatted DOCX file for easy review.
- **Exclusion Logic**: Skips entries marked as "Documentary" or "Music Video" to focus on narrative films.

## Requirements

- Python 3.x
- `pandas` library
- `python-docx` library
- Access to a language model (e.g., via an API)

## Installation

Clone the repository
Install the required packages:
pip install pandas python-docx
Usage
Download your CSV file from FilmFreeway, ensuring it includes the following columns:

Project Title
Synopsis
Project Type
Genres (optional)
Place your CSV file in the project directory

Run the script:

python NameOfYourScript.py

The results will be saved in a DOCX file named movie_genre_classification_results.docx.

Example CSV Format
Project Title,Synopsis,Project Type,Genres
"Bay for Blood","James and Rob are hiding out in isolation...","Drama, Thriller",""
"Running Towards the Fire","A War Correspondent's Story...","Documentary",""
