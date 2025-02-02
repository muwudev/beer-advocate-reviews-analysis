# Beer Advocate Review Analysis

This project analyzes a dataset of beer reviews to answer key questions about beer preferences, brewery performance, and user behavior. The analysis is conducted using two notebooks: one written in **R** and the other in **Python**.

[![Dataset](https://img.shields.io/badge/Dataset-Kaggle-blue)](https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate)

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset Description](#dataset-description)
3. [Analysis Questions](#analysis-questions)
4. [Methodology](#methodology)
5. [Results](#results)
6. [Usage](#usage)
7. [Dependencies](#dependencies)
8. [Contributing](#contributing)
9. [License](#license)

---

## Project Overview

This project uses **Exploratory Data Analysis (EDA)**, **Natural Language Processing (NLP)**, **Sentiment Analysis**, and **Machine Learning (ML)** techniques to analyze a dataset of beer reviews. The goal is to answer specific questions about beer ratings, user preferences, and brewery performance.

---

## Dataset Description

The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate). It contains the following columns:
- `beer_ABV`: Alcohol by volume (ABV) of the beer.
- `beer_beerId`: Unique identifier for each beer.
- `beer_brewerId`: Unique identifier for each brewery.
- `beer_name`: Name of the beer.
- `beer_style`: Style of the beer.
- `review_appearance`: User rating for the beer's appearance.
- `review_palette`: User rating for the beer's palette.
- `review_overall`: Overall user rating for the beer.
- `review_taste`: User rating for the beer's taste.
- `review_profileName`: Username of the reviewer.
- `review_aroma`: User rating for the beer's aroma.
- `review_text`: Written review by the user.
- `review_time`: Timestamp of the review.

---

## Analysis Questions

The project answers the following questions using statistical methods, NLP, and ML techniques:

1. **Rank top 3 Breweries which produce the strongest beers?**  
   - Grouped by `beer_brewerId` and calculated the average ABV for each brewery.

2. **Which year did beers enjoy the highest ratings?**  
   - Extracted the year from `review_time` and calculated the average rating for each year.

3. **Based on the user’s ratings, which factors are important among taste, aroma, appearance, and palette?**  
   - Calculated the correlation between `review_overall` and factors like taste, aroma, appearance, and palette.

4. **If you were to recommend 3 beers to your friends based on this data, which ones will you recommend?**  
   - Used weighted ratings to recommend beers based on user preferences.

5. **Which Beer style seems to be the favorite based on reviews written by users?**  
   - Analyzed written reviews using sentiment analysis to determine the most liked beer style.

6. **How does written review compare to overall review score for the beer styles?**  
   - Compared sentiment scores from written reviews with overall ratings.

---

## Methodology

### Tools and Techniques
- **Languages**: R, Python
- **Skills**: EDA, Data Visualization, Machine Learning, NLP, Sentiment Analysis, Documentation
- **Libraries**:
  - R: `dplyr`, `readr`, `syuzhet`, `ggplot2`, `pracma`
  - Python: `pandas`, `numpy`, `nltk`, `sklearn`, `re`, `tqdm`

### Notebooks
- **R Notebook**: Performs data cleaning, correlation analysis, sentiment analysis, and visualization.
- **Python Notebook**: Focuses on text preprocessing, TF-IDF, cosine similarity, and K-means clustering.

---

## Results

### Key Findings
1. **Top 3 Breweries by ABV**: Breweries with IDs `22`, `694`, and `2724` produce the strongest beers.
2. **Highest Rated Year**: The year `2012` had the highest average beer ratings.
3. **Most Important Factor**: `review_aroma` has the highest correlation with overall ratings.
4. **Recommended Beers**: Top 3 recommended beers based on weighted ratings.
5. **Favorite Beer Style**: `American Blonde Ale` is the most liked beer style based on sentiment analysis.
6. **User Clusters**: Users were grouped into 3 clusters based on their review patterns.

---

## Usage

### Running the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```
2. Install dependencies:
   - For R: Install the required libraries (`dplyr`, `readr`, `syuzhet`, `ggplot2`, `pracma`).
   - For Python: Install the required libraries (`pandas`, `numpy`, `nltk`, `sklearn`, `re`, `tqdm`).
3. Run the notebooks:
   - Open the R notebook in RStudio or Jupyter Notebook.
   - Open the Python notebook in Jupyter Notebook or Google Colab.

### Notebook Conversion
- Convert the R notebook to PDF using [Vertopal](https://www.vertopal.com/en/convert/rmd-to-pdf).

---

## Dependencies

### R
- `dplyr`
- `readr`
- `syuzhet`
- `ggplot2`
- `pracma`

### Python
- `pandas`
- `numpy`
- `nltk`
- `sklearn`
- `re`
- `tqdm`

---

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.

---

## Contact

For any queries, feel free to contact me on **Discord**.
