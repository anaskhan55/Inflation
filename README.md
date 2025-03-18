# Cost-of-Living Crisis Inflation Analysis: Energy and Food Sectors

## Project Overview
This repository contains code and datasets for analyzing and forecasting inflation trends in the energy and food sectors in the UK during the cost-of-living crisis. The project evaluates time-series models such as **SARIMA**,  **Prophet**, and **Holt-Winters Exponential Smoothing** to predict inflation trends for the year 2025. The code is designed to preprocess data, analyze trends, and generate forecasts with detailed performance metrics.

---

## Dataset
The data used in this project was sourced from the **Office for National Statistics (ONS)** and includes monthly inflation rates for:
- Motor Fuel
- Gas
- Food and Non-Alcoholic Beverages
- Restaurants and Cafes

Data spans from January 2013 to December 2024.

---

## Features
- **Preprocessing**: Cleans and formats inflation data for time-series analysis.
- **Visualization**: Provides exploratory data analysis (EDA) using trend plots, moving averages, histograms, and correlation heatmaps.
- **Modeling**:
  - **SARIMA**: Captures seasonality and trend components for cyclical inflation data.
  - **Prophet**: Handles complex seasonality and trend shifts effectively.
  - **Holt-Winters**: Best for stable datasets with regular seasonality.
- **Performance Metrics**: Evaluates models using **MAE**, **MSE**, and **RMSE**.

---

## Setup and Requirements
### Prerequisites
- Python 3.x
- Google Colab or a local environment with the required libraries installed.

### Required Libraries
Install dependencies using the following command:
```bash
pip install pandas matplotlib statsmodels prophet scipy pmdarima seaborn
```

## Dataset Structure
The dataset should be in .xlsx format with sheets for:

- Motor Fuel Inflation
- Gas Inflation
- Food Inflation
- Restaurant and Cafe Inflation

Each sheet must include:

- A Date column with time-series data.
- A column for inflation rates.

--- 

## Usage
Running the Code
1. Clone this repository:
```bash
git clone https://github.com/your-username/repository-name.git
```
2. Open the Jupyter Notebook (.ipynb) file in Google Colab or your local Jupyter environment.
3. Upload the dataset (.xlsx file) to your Colab session or local directory.
4. Modify the file paths in the code to match your dataset location.
5. Run all cells sequentially to:
  - Preprocess data.
  - Visualize trends and correlations.
  - Fit forecasting models.
  - Generate inflation forecasts and evaluate performance metrics.

---

## Results
- SARIMA: Best for cyclical inflation trends, especially in food and restaurant sectors.
- Prophet: Effective for flexible seasonality but less robust for volatile datasets.
- Holt-Winters: Performs well in stable datasets but struggles with high volatility.

---

## File Structure
```
📁 project-directory/
├── 📄 README.md        # Documentation for the project
├── 📄 *.ipynb  # Main code file for analysis
└── 📄 requirements.txt # List of required 
```

---

## Sample Visualizations
1. Trend Analysis:
  - Line plots for inflation trends across categories.
2. Correlation Heatmap:
  - Identifies relationships between inflation rates in different sectors.
3. Distribution Analysis:
  - Histograms to examine data variability.

## Contributions
Feel free to fork this repository, raise issues, or submit pull requests to enhance its functionality.

---

## License
This project is licensed under the MIT License.

---

## Acknowledgments
Special thanks to the Office for National Statistics (ONS) for providing the dataset and to the University of Hertfordshire for guidance and support.

---