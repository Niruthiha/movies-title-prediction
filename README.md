# Movie Analysis 

This project implements a movie analysis and recommendation system using natural language processing techniques and vector embeddings.

## Requirements

- Python 3.x
- Required packages:
  - re
  - pandas
  - seaborn
  - langchain
  - chromadb
  - sentence_transformers

## Setup

1. Clone the repository
2. Install the required packages
3. Ensure you have the movie dataset (`movies.csv`) in the `data` directory.

## Features

- **Data Processing**: Import and filter movie data
- **Text Analysis**: Analyze word count distribution in movie overviews
- **Text Splitting**: Implement sentence splitting for efficient processing
- **Vector Database**: Use Chroma DB for storing and querying movie embeddings
- **Querying**: Find movies based on description

The "all-MiniLM-L6-v2" model is a smaller, faster version of BERT that's been optimized for generating sentence embeddings. It's particularly good at capturing semantic similarity between sentences, which makes it ideal for tasks like finding similar movie descriptions.
By using this model, the project can efficiently process movie descriptions, generate meaningful embeddings, and perform similarity searches to find movies based on textual queries. This forms the basis of the recommendation system, allowing users to find movies similar to a given description.

## Usage Example  
    ```bash
    get_title_by_description(query_text="monster, underwater")

## Example output:
  ```bash
'Title: Hidden Dragon \n'
('Description: In a magical undersea world where dragons rule and humans are '
 "feared a naive young dragon forms an uneasy alliance with the sea's greatest "
 'enemy - a human girl. \n')
'-------------------------------------------------'
'Title: Meg 2: The Trench \n'
('Description: An exploratory dive into the deepest depths of the ocean of a '
 'daring research team spirals into chaos when a malevolent mining operation '
 'threatens their mission and forces them into a high-stakes battle for '
 'survival. \n')
'-------------------------------------------------'
'Title: Legend of the Ocean \n'
('Description: A marine science fiction that follows Xiaohai a 12 year old boy '
 "who exchanges souls with the aquarium's star sea lion—Candy. \n")
'-------------------------------------------------'
