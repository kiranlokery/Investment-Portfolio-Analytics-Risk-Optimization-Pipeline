#  Portfolio Optimization and Risk Analysis

This project focuses on **portfolio risk analysis and optimization** using Python.  
It involves collecting financial data, preprocessing it, analyzing portfolio performance, and implementing optimization techniques to identify the optimal portfolio weights.

---

##  Project Structure

The project is organized into the following directories and files:

- **data/**: Contains historical stock and benchmark data in CSV format.  
- **notebooks/**: Jupyter notebooks for data exploration, analysis, and visualization.  
- **scripts/**: Python scripts for data collection, preprocessing, portfolio analysis, and optimization.  
- **README.md**: This file, providing an overview of the project.  
- **requirements.yml**: YAML file listing the Conda packages and their versions required to run the project.  

---

##  Data Collection

The `data_collection.py` script fetches historical stock data using the **Yahoo Finance API** and saves it as `stock_data.csv` in the `data` directory.  
You can customize the stock symbol and date range as needed.

---

##  Data Preprocessing

The `data_preprocessing.py` script cleans and preprocesses the stock data by:
- Handling missing values  
- Aligning dates across different assets  
- Calculating daily returns  

The preprocessed data is saved as `preprocessed_stock_data.csv` in the `data` directory.

---

##  Portfolio Analysis

The `portfolio_analysis.py` script calculates various portfolio metrics, such as:
- Mean returns  
- Volatility  
- Correlation coefficients between assets  

It also provides an option for **Monte Carlo simulations** to estimate portfolio performance under different scenarios.

---

##  Optimization

The `optimization.py` script implements portfolio optimization techniques to construct an **optimal portfolio**.  
You can customize:
- The optimization strategy (e.g., Mean-Variance Optimization, Sharpe Ratio maximization)  
- The constraints (e.g., weight bounds, risk limits)

The optimized portfolio weights and metrics are saved as needed for further analysis.

---

##  How to Run the Project

1. **Create a Conda environment** using the provided YAML file:
   ```bash
   conda env create -f environment.yml
   conda activate portfolio-optimization
2. **Execute the following scripts in order:**
   - python scripts/data_collection.py
   - python scripts/data_preprocessing.py
   - python scripts/portfolio_analysis.py
   - python scripts/optimization.py


