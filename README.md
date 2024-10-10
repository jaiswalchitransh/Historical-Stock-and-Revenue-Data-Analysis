# Historical Stock and Revenue Data Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [Contribution](#contribution)

## Project Overview
This project focuses on extracting and visualizing stock data for companies like Tesla and GameStop. By using libraries such as `yfinance` for stock data extraction and web scraping techniques to retrieve revenue data, the project provides insights into the relationship between stock prices and company revenues. The extracted data is visualized using Python libraries like `Plotly` and `Matplotlib` for easy interpretation.

The project contains:
- A graphing function to visualize stock price and revenue.
- Data extraction from Yahoo Finance and MacroTrends.
- Graphs for Tesla and GameStop stock data.

## Installation
This project requires Python 3.12.1 or later.
To set up the project:
1. Ensure Python 3.12.1 or a later version is installed on your system. You can download Python from [python.org](https://www.python.org/downloads/).
2. Clone or download the repository to your local machine.
    
       git clone https://github.com/jaiswalchitransh/Historical-Stock-and-Revenue-Data-Analysis.git
  
3. Install the necessary Python packages:
   
   Required packages:
   - `yfinance`
   - `pandas`
   - `requests`
   - `beautifulsoup4`
   - `plotly`
   - `matplotlib`

4. Run the script in your Python environment.

## Usage
To run the analysis and visualize the stock data, follow these steps:

1. Open the `analyzer.ipynb` Jupyter Notebook in your preferred environment. You can use Jupyter Notebook or JupyterLab for this purpose.

       jupyter notebook analyzer.ipynb

2. Run all the cells in the notebook to:
   - Extract Tesla and GameStop stock data from Yahoo Finance using `yfinance`.
   - Scrape Tesla and GameStop revenue data from MacroTrends.
   - Visualize the stock prices and revenue data using the `make_graph` function.

3. The notebook will display interactive graphs of Tesla and GameStop stock prices and revenue over time.

## Features
- **Stock Data Extraction**: Fetches historical stock data from Yahoo Finance using `yfinance`.
- **Revenue Data Extraction**: Uses web scraping to extract Tesla and GameStop revenue data from MacroTrends.
- **Data Visualization**: Displays the relationship between stock prices and company revenue using dual-axis graphs.
- **Graphing Function**: The `make_graph` function is used to plot historical stock prices and revenue.

## Results
Below are the visualizations of stock data and revenue for **Tesla** and **GameStop**:

Tesla Stock Data and Revenue :

![Tesla Stock Price and Revenue](https://github.com/jaiswalchitransh/Analyzing-Historical-Stock-Data/blob/main/Sample%20Output/tesla_stock_graph.png)
*Figure 1: Tesla's Stock Price (Blue) and Revenue (Green) Over Time.*

GameStop Stock Data and Revenue :

![GameStop Stock Price and Revenue](https://github.com/jaiswalchitransh/Analyzing-Historical-Stock-Data/blob/main/Sample%20Output/gamestop_stock_graph.png)
*Figure 2: GameStop's Stock Price (Blue) and Revenue (Green) Over Time.*

These graphs display the historical trends in both stock price and revenue for Tesla and GameStop, giving insights into their performance over time.


## Contribution
I, **[Chitransh Jaiswal](https://www.linkedin.com/in/jaiswalchitransh/)** developed this Project Individually. I was responsible for all aspects of the project, including design, development, testing, and documentation.
Contributions to improve the efficiency, readability, or functionality of the code are welcome. To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature`).
6. Create a new Pull Request.

Please ensure your contributions adhere to the coding standards and follow the existing style and structure.

---

Thank you for exploring the Historical Stock and Revenue Data Analysis!
