# BrandLens.AI

An NLP-powered social media analytics framework for brand sentiment and topic analysis, built as an MBA dissertation project (Amity University, 2026).

## Overview

BrandLens.AI analyzes brand-related social media conversation at scale — combining sentiment scoring, topic modelling, and an interactive dashboard so non-technical stakeholders can explore trends without touching code. The pipeline was applied to a case study brand (Pinsout) using a 100K+ tweet dataset.

## What it does

- **Sentiment analysis** — scores tweet sentiment using two approaches for comparison: VADER (rule-based) and BERT (transformer-based)
- **Topic modelling** — uses BERTopic to surface dominant conversation themes automatically, without manually predefined categories
- **Interactive dashboard** — a Plotly Dash app for exploring sentiment trends and engagement metrics in real time

## Results

| Method | Accuracy |
|---|---|
| VADER | 69% |
| BERT | 80% |

BERTopic identified **28 distinct topics** within the conversation dataset, used to generate strategic content recommendations.

## Tech stack

- **Data & modelling:** Python, Pandas, VADER, BERT, BERTopic
- **Visualization:** Plotly Dash
- **Dataset:** Sentiment140 (100K+ tweets), case study brand: Pinsout

## Project structure

```
brandlens-ai/
├── notebooks/          # EDA, VADER, BERT, BERTopic, dashboard notebooks
├── environment.yml      # Conda environment for reproducing results
├── README.md
└── .gitignore
```

## Running it locally

1. Clone the repo: `git clone https://github.com/chitranpande/brandlens-ai.git`
2. Recreate the environment: `conda env create -f environment.yml`
3. Activate it: `conda activate brandlens-ai`
4. Launch Jupyter: `jupyter notebook`
5. Run the notebooks in order (EDA → VADER → BERT → BERTopic → dashboard)

## Author

Chitran Pande — [LinkedIn](https://linkedin.com/in/chitranpande)
