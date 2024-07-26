# Data Visualization Project: UK Life Aspects

![2024-07-26_152306](https://github.com/user-attachments/assets/da966047-02bf-47d6-9bfc-7a5605a871c4)


## Overview

This project provides visual representations and analysis of three aspects of life in the United Kingdom: housing prices in London and Newcastle, UK internet speeds, and the share prices of the top 100 companies. The visualizations are created using Python and various data visualization libraries.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Sci-Kit

## Data Sources

- **Housing Prices:** `Average-prices-Property-Type-2021-05_wrangled.csv`
- **Internet Speeds:** `202006_fixed_laua_performance_wrangled.csv`
- **FTSE 100 Share Prices:** `ftse_data_wrangled.csv`

## How to Run

1. Ensure all the required libraries are installed:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

2. Place the CSV data files in the same directory as the script.

3. Run the script:
    ```bash
    python script.py
    ```

4. The script will generate a visualization saved as `figure_output.png` and display it.

## Project Components

### Data Wrangling

The `wrangle_data` function processes the raw data:
- Filters housing prices for April 2011 and April 2021.
- Standardizes region and property type names.
- Calculates the decade change in housing prices.
- Filters broadband speed data to remove outliers.
- Processes FTSE 100 data to focus on a two-year period from October 2019 to October 2021.

### Visualization

The `plot_data` function creates visualizations for the following:
1. **Housing Prices:**
   - Bar chart comparing the increase in average house prices in London and Newcastle from 2011 to 2021.
   - Bright colors differentiate property types.
   - Gestalt design principles such as continuity are followed.

2. **Broadband Performance:**
   - Scatter plot showing the correlation between mean download and upload speeds across 209 UK regions.
   - Regression line added to visualize the correlation.

3. **FTSE 100 Share Prices:**
   - Line chart displaying FTSE 100 closing prices over a two-year period.
   - Bollinger Bands and Simple Moving Average (SMA) included to provide additional insights.

4. **Conclusions:**
   - Text box summarizing the key findings from the visualizations.

## Visualization Descriptions

### A. House Prices

#### Use of Visual Channels
- Bar charts are used to display the increase in average house prices for different property types.

#### Gestalt Design Principles
- **Continuity:** Charts are sorted to maintain visual continuity.
- **Color:** Bright colors are used to differentiate property types and regions, ensuring clarity.

#### Language and Narrative
- The captions and titles provide context and highlight key findings, such as the significant price increase in London compared to Newcastle.

### B. Broadband Performance Data

#### Use of Visual Channels
- Scatter plots show the relationship between download and upload speeds.

#### Gestalt Design Principles
- **Color:** Different colors and a regression line enhance readability and highlight correlations.

#### Language and Narrative
- Captions explain the weak positive correlation found between download and upload speeds.

### C. Financial Time Series Data

#### Use of Visual Channels
- Line charts visualize FTSE 100 share prices over time, with additional indicators like Bollinger Bands and SMA.

#### Gestalt Design Principles
- **Color:** Different line styles and colors distinguish between the stock price, SMA, and Bollinger Bands.

#### Language and Narrative
- Captions provide insights into the stock price trends, especially the impact of the COVID-19 pandemic.

## Conclusion

The visualizations effectively communicate the changes in housing prices, broadband speeds, and stock prices in the UK. By following principles of good design and clear narration, the project aims to make data insights accessible and understandable to the viewer.

## License

This project is licensed under the MIT License.
