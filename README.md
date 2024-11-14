# Gold Price Analysis and Forecasting Project

This project provides a comprehensive analysis of gold prices over the past five years, covering trend analysis, volatility assessment, seasonality analysis, and a forecasting model using ARIMA. The analysis helps to understand patterns in gold prices, evaluate market volatility, and generate short-term price forecasts.

## Project Structure
The project includes the following steps:
1. **Data Cleaning**: We used a custom data cleaning tool to ensure the dataset was clean and consistent before analysis.
2. **Trend Analysis**: Analyzed long-term price trends using a 30-day moving average.
3. **Volatility Analysis**: Examined daily price variability to understand market risk.
4. **Seasonality and Statistical Patterns**: Investigated monthly patterns to uncover any recurring trends or seasonal behaviors.
5. **Forecasting with ARIMA**: Developed a short-term forecast using an ARIMA model, with evaluation metrics to assess accuracy.

## Data Cleaning Tool
To ensure accurate results, we used a **data cleaning tool** to prepare the dataset for analysis. This tool handles missing values, adjusts date formats, and performs initial data validation. The data cleaning step is crucial for improving data quality before applying any analytical methods.

### Running the Data Cleaning Tool
You can run the data cleaning tool with the following code snippet. Make sure the raw data file is saved in the `data/raw/` directory with the filename `gold_prices_raw.csv`. The cleaned data will be saved in `data/cleaned/cleaned_gold_prices.csv`.

```python
import pandas as pd

def clean_gold_data(input_file='data/raw/gold_prices_raw.csv', output_file='data/cleaned/cleaned_gold_prices.csv'):
    # Load the dataset
    data = pd.read_csv(input_file)
    
    # Convert the 'date' column to datetime format
    if 'date' in data.columns:
        data['date'] = pd.to_datetime(data['date'], errors='coerce')
        data = data.dropna(subset=['date'])
    
    # Fill or drop any remaining missing values as needed
    data = data.fillna(method='ffill').fillna(method='bfill')
    
    # Save the cleaned data
    data.to_csv(output_file, index=False)
    print(f"Data cleaned and saved to {output_file}")

# Run the data cleaning function
clean_gold_data()