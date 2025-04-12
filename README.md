# Sentiment Analysis of Customer Reviews

Welcome to my sentiment analysis project! This repository contains a Python-based analysis of customer reviews using Jupyter Notebook, designed to classify sentiments and uncover insights through data visualization and statistical analysis. The project leverages popular libraries like TextBlob, pandas, Matplotlib, and Seaborn to process and visualize review data.

## Overview

This project analyzes a dataset of customer reviews to determine sentiment (Positive, Negative, or Neutral) and explores relationships between sentiment and metrics such as helpfulness votes, review timing, and calculated scores. The goal is to provide actionable insights into customer satisfaction and feedback trends, showcasing skills in data science, natural language processing (NLP), and data visualization.

### Key Features
- Sentiment classification using TextBlob to assign polarity scores.
- Data cleaning to handle missing values and prepare the dataset.
- Rich visualizations including count plots, bar charts, word clouds, and correlation heatmaps.
- Statistical analysis to identify correlations between review metrics.

## Project Highlights

### Visualizations
1. **Sentiment Distribution (Count Plot)**  
   - Displays the frequency of Positive, Negative, and Neutral sentiments, with Positive reviews dominating (over 4,000 counts).
2. **Helpful Votes by Sentiment (Bar Chart)**  
   - Shows that Positive reviews average ~15 helpful votes, far exceeding Negative and Neutral (~1 vote each).

3. **Positive Review Word Cloud**  
   - Highlights frequent terms like "great," "phone," "easy," and "Samsung" from positive reviews.

4. **Correlation Matrix (Heatmap)**  
   - Reveals strong correlations (e.g., 1.00 between helpfulness and total votes) and negative correlations (e.g., -1.00 between `days_since_first_review` and `day_diff`).

### Key Insights
- Positive sentiments dominate, indicating high customer satisfaction.
- Positive reviews receive significantly more helpful votes, suggesting their influence.
- Strong correlations between metrics like review length and helpfulness votes offer data-driven insights.

## Getting Started

### Prerequisites
Ensure you have Python 3.x installed, along with the following libraries:
- `pandas`
- `matplotlib`
- `seaborn`
- `nltk`
- `textblob`
- `wordcloud`

You can install these using pip:
```bash
pip install pandas matplotlib seaborn nltk textblob wordcloud
```

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yashreddy1154/amazon-sentiment-analysis
   cd amazon-sentiment-analysis
   ```
2. Download the dataset (e.g., `amazon.csv`) and place it in the repository root directory.
3. Install dependencies as listed above.

### Usage
1. Open the Jupyter Notebook (`code.ipynb`) in Jupyter Notebook or VS Code with the Jupyter extension.
2. Run all cells to load the data, clean it, perform sentiment analysis, and generate visualizations.
3. Explore the output plots and correlation matrix to analyze the results.

## Project Structure
- `code.ipynb`: Main Jupyter Notebook with the complete analysis and visualizations.
- `amazon.csv`: Dataset containing review data (ensure this matches your file name).
- `README.md`: This file, providing project documentation.

## Built With
- **Python**: Core programming language.
- **pandas**: Data manipulation and analysis.
- **Matplotlib & Seaborn**: Data visualization with a custom dark theme.
- **TextBlob**: Sentiment analysis and polarity scoring.
- **NLTK**: Text preprocessing.
- **WordCloud**: Word cloud generation.
- **Jupyter Notebook**: Interactive development environment.

## Challenges & Solutions
- **Missing Data**: Dropped rows with missing `reviewText` to ensure clean input for TextBlob.
- **Visualization Issues**: Resolved Seaborn warnings and ensured plots saved correctly with `plt.tight_layout()` and higher DPI.
- **Time Metrics**: Noted a perfect negative correlation between `days_since_first_review` and `day_diff`, prompting further investigation into dataset structure.

## Future Improvements
- Incorporate more advanced NLP techniques (e.g., BERT) for sentiment analysis.
- Add time-series analysis to track sentiment trends over months or years.
- Enhance the dataset with additional features (e.g., product categories).

## Acknowledgments
- Thanks to the open-source community for tools like TextBlob and WordCloud.
- Inspired by my learning journey in data science and feedback from peers.

## Contact
Have questions or suggestions? Connect with me on [LinkedIn](https://www.linkedin.com/in/yash1154) or open an issue in this repository!
