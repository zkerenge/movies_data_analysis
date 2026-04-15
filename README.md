# 🎬 TMDB Movies Analytics

A comprehensive exploratory data analysis (EDA) project analyzing the TMDB Movies dataset to uncover insights about film industry trends, movie performance, and audience preferences.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Analysis Sections](#analysis-sections)
- [Requirements](#requirements)
- [License](#license)

## 🔍 Overview

This project performs in-depth analysis on over 1.18 million movies from the TMDB (The Movie Database) dataset. The analysis covers:

- **Data Cleaning & Preprocessing**: Handling missing values, converting dates, creating derived features
- **Univariate Analysis**: Understanding distributions of individual variables
- **Bivariate Analysis**: Exploring relationships between two variables
- **Multivariate Analysis**: Analyzing complex relationships across multiple dimensions

## ✨ Features

- 📊 Comprehensive statistical analysis of movie data
- 🎨 Rich visualizations using Matplotlib and Seaborn
- 📈 Trend analysis of movies over time
- 💰 Budget vs Revenue correlation studies
- ⭐ Rating and popularity analysis
- 🌍 Geographic and language distribution
- 🎭 Genre-based insights
- 👥 Director and cast analysis

## 📦 Dataset

**Source**: [TMDB Movies Daily Updates](https://www.kaggle.com/datasets/alanvourch/tmdb-movies-daily-updates) by `alanvourch`

- **Update Frequency**: Daily
- **License**: Open Data
- **Size**: ~1.18M movies with 28 features

### Key Features

| Feature | Description |
|---------|-------------|
| `title` | Movie title |
| `vote_average` | Average user rating |
| `vote_count` | Number of votes |
| `revenue` | Box office revenue |
| `budget` | Production budget |
| `runtime` | Movie duration in minutes |
| `release_date` | Release date |
| `genres` | Movie genres |
| `production_companies` | Production studios |
| `production_countries` | Country of origin |
| `original_language` | Original language |
| `director` | Movie director |
| `cast` | Main cast members |
| `imdb_rating` | IMDb rating |
| `popularity` | Popularity score |

## 🚀 Installation

### Prerequisites

- Python 3.8+
- pip package manager

### Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-directory>
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Install kagglehub (for dataset access):
```bash
pip install kagglehub
```

## 📖 Usage

### Running the Analysis

Open and run the Jupyter notebook:

```bash
jupyter notebook notebooks/movies_analytics.ipynb
```

Or convert to Python script and run:

```bash
jupyter nbconvert --to script notebooks/movies_analytics.ipynb
python movies_analytics.py
```

### Dataset Access

The dataset is automatically downloaded and cached using `kagglehub` when you run the notebook. The first run will download the dataset to your local cache directory.

## 📁 Project Structure

```
├── notebooks/
│   └── movies_analytics.ipynb    # Main analysis notebook
├── data/
│   └── README.md                  # Dataset documentation
├── requirements.txt               # Python dependencies
└── README.md                      # This file
```

## 📊 Analysis Sections

### 1. Initial Setup & Data Loading
- Environment setup and library imports
- Dataset download and loading

### 2. Data Exploration
- Basic statistics and missing value analysis
- Statistical summary of numerical features
- Duplicate detection
- Sample data inspection

### 3. Data Cleaning
- Handling missing data strategies
- Date conversion and formatting
- Creating derived features (e.g., release year, decade)

### 4. Univariate Analysis
- Distribution plots for numerical columns
- Box plots for outlier detection
- Categorical variable analysis:
  - Movie status distribution
  - Original language breakdown
  - Genre frequencies
  - Production countries
  - Top directors

### 5. Bivariate Analysis
- Budget vs Revenue relationship
- Runtime vs Rating correlation
- Release year trends analysis

### 6. Multivariate Analysis
- Correlation heatmap
- Genre-based multi-dimensional analysis

## 📋 Requirements

Main dependencies (see `requirements.txt` for complete list):

- `pandas` - Data manipulation
- `numpy` - Numerical computing
- `matplotlib` - Visualization
- `seaborn` - Statistical visualization
- `scikit-learn` - Machine learning utilities
- `kagglehub` - Dataset access

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source. The dataset is subject to its own license terms (Open Data).

## 🙏 Acknowledgments

- Dataset provided by [alanvourch](https://www.kaggle.com/alanvourch) on Kaggle
- Data sourced from The Movie Database (TMDB)
- Built with open-source Python data science libraries

---

**Author**: Zacharia Kerenge  
**Created**: 2024  
**Last Updated**: 2024
