# Beer Review Analysis Project

This project analyzes a dataset of beer reviews to answer key questions about beer preferences, brewery performance, and user behavior. The analysis is conducted using two notebooks: one written in **R** and the other in **Python**.

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

The goal of this project is to analyze beer reviews to:
- Identify the top breweries producing the strongest beers.
- Determine the year with the highest beer ratings.
- Understand which factors (taste, aroma, appearance, palette) are most important to users.
- Recommend beers based on user ratings.
- Analyze beer styles based on written reviews.
- Find similar beer drinkers using machine learning techniques.

---

## Dataset Description

The dataset (`reviews.csv`) contains the following columns:
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

1. **Top 3 Breweries Producing the Strongest Beers**  
   - Grouped by `beer_brewerId` and calculated the average ABV for each brewery.

2. **Year with the Highest Beer Ratings**  
   - Extracted the year from `review_time` and calculated the average rating for each year.

3. **Important Factors in User Ratings**  
   - Calculated the correlation between `review_overall` and factors like taste, aroma, appearance, and palette.

4. **Top 3 Recommended Beers**  
   - Used weighted ratings to recommend beers based on user preferences.

5. **Favorite Beer Style Based on Reviews**  
   - Analyzed written reviews to determine the most liked beer style.

6. **Comparison of Written Reviews and Overall Ratings**  
   - Compared sentiment scores from written reviews with overall ratings.

7. **Finding Similar Beer Drinkers**  
   - Used TF-IDF and cosine similarity to group users with similar review patterns.

---

## Methodology

### R Notebook
- Libraries used: `dplyr`, `readr`, `syuzhet`, `ggplot2`, `pracma`.
- Steps:
  1. Loaded and cleaned the dataset.
  2. Analyzed correlations between review factors.
  3. Performed sentiment analysis on written reviews.
  4. Visualized results using bar plots and scatter plots.

### Python Notebook
- Libraries used: `pandas`, `numpy`, `nltk`, `sklearn`, `re`, `tqdm`.
- Steps:
  1. Loaded and cleaned the dataset.
  2. Performed text preprocessing on written reviews.
  3. Used TF-IDF and cosine similarity to group similar users.
  4. Applied K-means clustering to identify user clusters.

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

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
