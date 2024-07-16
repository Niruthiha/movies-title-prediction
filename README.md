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
