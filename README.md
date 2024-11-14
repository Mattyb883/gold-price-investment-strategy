# Gold Price Analysis and Forecasting

## Project Overview
This project aims to analyze historical gold prices and forecast near-term trends. The analysis involves exploring patterns in price movements, volatility, seasonal behavior, and potential correlations with other financial factors. This project serves as a foundation for understanding gold price dynamics and can be expanded with more complex predictive models in the future.

## Data Description
The dataset used in this project includes historical gold prices over the past five years. Key features include:
- **Date**: The date of each record.
- **Close**: The closing price of gold on each date.
- **Volume**: The volume of gold traded.
- **Dividends**: Any dividends associated with gold investments.
- **Capital Gains**: Capital gains related to gold price movements.

## Project Steps

1. ### Trend Analysis
   - **Objective**: To observe long-term trends in gold prices.
   - **Method**: A 30-day moving average was calculated to smooth out daily fluctuations, highlighting sustained price trends over time.

2. ### Volatility Analysis
   - **Objective**: To measure gold price variability.
   - **Method**: Daily returns and a 30-day rolling standard deviation were calculated to capture periods of high and low volatility. This analysis provides insights into times of economic uncertainty or market stress.

3. ### Seasonality and Statistical Patterns
   - **Objective**: To identify recurring seasonal patterns in gold prices.
   - **Method**: Monthly and annual statistics were calculated, and a box plot of monthly price distributions was created to visualize potential seasonal trends.

4. ### Rolling Mean Model for Forecasting
   - **Objective**: To create a simple short-term forecast for gold prices.
   - **Method**: A 30-day rolling mean was used as a basic forecasting model. While this method is straightforward, it provides a baseline for understanding near-term trends.

5. ### Correlation Analysis
   - **Objective**: To examine potential relationships between gold prices and other financial factors.
   - **Method**: A correlation matrix was generated for `close`, `volume`, `dividends`, and `capital gains`, then visualized with a heatmap to highlight strong relationships.

6. ### Conclusion
   - **Key Insights**: 
      - Gold prices show long-term trends that respond to economic factors.
      - Volatility is variable and likely influenced by broader financial conditions.
      - Seasonal patterns exist, with certain months exhibiting higher or more variable prices.
      - A correlation analysis highlighted relationships between gold prices and other factors, which could inform further predictive modeling.
   - **Recommendations**:
      - Explore more advanced models, such as machine learning algorithms, for improved forecast accuracy.
      - Investigate additional features (e.g., inflation, interest rates) to understand external influences on gold prices.

## Getting Started

### Prerequisites
- Python 3.x
- Libraries: `pandas`, `matplotlib`, `seaborn`, `numpy`, `scikit-learn`, `statsmodels`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/gold_analysis.git
