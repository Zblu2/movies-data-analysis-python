# Movie Data Analysis with Python in Google Colab

This is my first attempt at data handling and analysis using Python, performed within a Google Colab environment. This project focuses on exploring and analyzing a dataset of movies to understand various characteristics and relationships within the data.

## Project Overview

The goal of this project was to gain hands-on experience with fundamental data analysis techniques using Python libraries such as pandas, numpy, matplotlib, and seaborn. The analysis includes:

*   Data loading and initial inspection.
*   Handling missing data.
*   Checking data types.
*   Identifying potential outliers.
*   Exploring relationships between different movie attributes (e.g., budget vs. gross earnings).
*   Analyzing correlations between numerical features.
*   Investigating trends over time (e.g., average movie gross per year).
*   Identifying top performers (e.g., top directors and writers by average gross).
*   Building a simple regression model to understand factors influencing gross revenue.

## Dataset

The dataset used in this project is a CSV file named `movies.csv` that I acquired from Kaggle. It contains information about various movies, including details like budget, gross earnings, score, year, director, writer, etc.

## Technologies and Libraries Used

*   **Google Colab:** The interactive notebook environment used for coding and execution.
*   **Python:** The primary programming language.
*   **pandas:** For data manipulation and analysis.
*   **numpy:** For numerical operations.
*   **matplotlib:** For creating static, interactive, and animated visualizations.
*   **seaborn:** For creating informative statistical graphics.
*   **statsmodels:** For statistical modeling (specifically OLS regression).

## How to View the Notebook

You can view the analysis directly on GitHub, as GitHub renders Jupyter notebooks (`.ipynb` files). Simply navigate to the notebook file (`your-notebook-name.ipynb`) in the repository.

Alternatively, you can open the notebook in Google Colab:

1.  Go to Google Colab.
2.  Click on "File" > "Open notebook".
3.  Go to the "GitHub" tab.
4.  Enter your repository URL or search for it.
5.  Select the notebook file to open it.

## Key Findings

Through this analysis, several key insights were gained regarding the movie dataset:

*   **Data Cleaning:** Missing values were identified and handled by dropping rows with incomplete information. This ensured that the subsequent analysis was based on clean and complete data points.
*   **Data Exploration:** Initial exploration provided an overview of the dataset's structure, data types, and the presence of potential outliers in the 'gross' earnings. Duplicate entries were also addressed.
*   **Relationship between Budget and Gross:** Visualizations, including scatter plots with regression lines, indicated a positive correlation between the movie's budget and its gross earnings. Generally, higher budgets tend to be associated with higher gross revenues.
*   **Relationship between Score and Gross:** A positive relationship was also observed between a movie's score (representing a rating or review score) and its gross earnings. Higher-rated movies tend to perform better financially.
*   **Correlation Analysis:**
    *   A correlation matrix for numeric features confirmed the positive relationships between 'budget' and 'gross', and 'score' and 'gross'.
    *   By factorizing categorical columns, a broader correlation analysis was performed across all features. This helped identify potential relationships between categorical variables and 'gross', excluding the 'name' of the movie as it's not typically a predictive factor. Strong correlations involving 'gross' were identified, highlighting features that might be significant drivers of revenue.
*   **Trends Over Time:** Analyzing the average gross earnings per year revealed trends in the movie industry's revenue over the years covered by the dataset.
*   **Top Performers:** Identifying the top writers and directors based on their average movie gross highlighted individuals who have historically been associated with higher-earning films. A box plot visualized the distribution of gross revenue for these top directors, providing a clearer picture of their financial performance range.
*   **Regression Analysis:** A simple OLS regression model was built to quantify the impact of certain features on 'gross' revenue. Initial modeling with 'year' showed its relationship with gross. A more comprehensive model including 'budget' and an encoded representation of 'director' (based on average gross) helped to understand the combined influence of these factors on a movie's financial success.

This initial analysis provides a foundation for understanding the factors that may contribute to a movie's gross earnings and offers insights into industry trends and key individuals.

## Acknowledgements

*   Thanks to [Kaggle] for providing the dataset.
*   Thanks to Google Colab for providing a free and accessible environment for this project.
