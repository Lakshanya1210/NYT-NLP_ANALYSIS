## NYT Article Analysis: Topic Modeling & Semantic Similarity

Exploratory NLP project on New York Times article data using topic modeling (LDA/NMF) and multi-model semantic similarity comparisons.

## Notebooks

| Notebook | Description |
|---|---|
| `NYT_Articles.ipynb` | Text preprocessing, LDA & NMF topic modeling on NYT articles |
| `All_models_comparison.ipynb` | Cross-dataset semantic similarity using 6 sentence-transformer models |

## Data

The notebooks expect three CSV files in the root directory:
- `nyt_articles.csv` — Full-text article data from the NYT Article Search API
- `nyt_mostpopular_daily.csv` — Daily snapshots from the NYT Most Popular API
- `nyt_topstories_daily.csv` — Daily snapshots from the NYT Top Stories API

> Data files are not included in this repository and are kept private.

## Setup

```bash
pip install -r requirements.txt
```

NLTK packages are downloaded automatically on first run.

## Models Compared (Similarity Notebook)

- `all-MiniLM-L6-v2`
- `all-mpnet-base-v2`
- `GIST-Embedding-v0`
- `bge-base-en`
- `e5-base`
- `bge-m3`
