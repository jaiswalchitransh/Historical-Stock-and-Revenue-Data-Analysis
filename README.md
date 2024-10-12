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
  
         pip install yfinance pandas requests beautifulsoup4 plotly matplotlib

4. Open the project in Jupyter Notebook or any Python IDE.
5. Run the script in your Python environment.

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
This project offers several powerful features designed to simplify data extraction, analysis, and visualization for stock market insights:

### 1. **Stock Data Extraction (yfinance)**:
   - The project uses the `yfinance` library to effortlessly pull historical stock price data for Tesla and GameStop. This includes detailed information such as Open, High, Low, Close, Volume, Dividends, and Stock Splits.
   - The ability to retrieve data over the entire history ("max" period) provides valuable insights into long-term stock performance, making it ideal for detailed financial analyses.

### 2. **Revenue Data Extraction (Web Scraping with BeautifulSoup)**:
   - Leveraging the `requests` library in combination with `BeautifulSoup`, the project web scrapes quarterly revenue data for Tesla and GameStop from MacroTrends.
   - The process automatically cleans and formats the extracted data (removing commas, dollar signs, and handling NaN values), ensuring a clean and structured dataset for analysis.
   - This automated scraping method makes it easy to continuously update the revenue data without manual intervention.

### 3. **Dual-Axis Graphing Function**:
   - A key feature is the **custom graphing function**, `make_graph`, which allows for dual-axis plotting:
     - **Primary Axis**: Stock Price (blue) on the left y-axis.
     - **Secondary Axis**: Revenue (green) on the right y-axis.
   - By plotting both stock price and revenue on a single graph, it becomes much easier to visualize and interpret the correlation between a company's stock performance and its revenue trends over time.
   - The function is flexible and reusable, making it simple to apply to other stocks or datasets.

### 4. **Interactive Data Visualization (Plotly & Matplotlib)**:
   - The project utilizes two powerful visualization libraries: `Plotly` for dynamic, interactive graphs, and `Matplotlib` for static, well-structured visualizations.
   - **Plotly**: Provides zooming, panning, and tooltips that allow users to explore the data interactively, making it an excellent tool for presenting insights in a dynamic and engaging way.
   - **Matplotlib**: Offers customizable and static visualizations that can be saved as images or incorporated into reports, making it suitable for documentation and formal analysis.

### 5. **Data Cleaning & Preprocessing**:
   - Includes preprocessing steps to ensure that both stock and revenue data are formatted correctly and free from inconsistencies (like NaN values or improper formatting).
   - This preprocessing ensures smooth data integration and helps avoid common errors during analysis, like type mismatches or missing values.

### 6. **Scalability**:
   - The codebase is designed to be easily extended to other stocks or datasets. Simply modify the ticker symbols or web scraping targets, and the functions will work seamlessly with the new data.
   - With a few adjustments, the framework can also be adapted to analyze other financial metrics like earnings, profits, or dividends, making it a versatile tool for financial analysis.

### 7. **Well-Documented & Modular Code**:
   - The project follows a modular structure where functions and code blocks are organized logically. Each component, whether it’s data extraction, cleaning, or visualization, is well-documented with comments explaining the purpose and functionality of each step.
   - This modularity makes it easier for developers or analysts to contribute, debug, or modify the project without needing to overhaul the entire codebase.

## Results
The project provides detailed visual insights into the historical stock price and revenue trends for **Tesla** and **GameStop**, illustrating how the performance of each company’s stock price correlates with its revenue over time.

### Tesla Stock Data and Revenue Analysis:
![Tesla Stock Price and Revenue](https://github.com/jaiswalchitransh/Analyzing-Historical-Stock-Data/blob/main/Sample%20Output/tesla_stock_graph.png)
*Figure 1: Tesla's Stock Price (Blue) and Revenue (Green) Over Time.*

1. **Stock Price Trend**:
   - Tesla’s stock price has shown significant volatility over the years but exhibits a generally upward trajectory, particularly from 2020 onwards. This period corresponds with Tesla's rapid growth, expansion in production, and increased market interest in electric vehicles.
   - A few key inflection points are noticeable, such as rapid surges in stock price in late 2019 and throughout 2020. These surges align with Tesla's achievements, like hitting production milestones, reporting profitable quarters, and joining the S&P 500 index.

2. **Revenue Trend**:
   - Tesla’s revenue has steadily increased over time, reflecting the company's growing sales of electric vehicles, energy products, and services. The revenue growth has been particularly strong since 2018, with Tesla ramping up production, opening new gigafactories, and expanding its vehicle lineup.
   - From the visualization, it is clear that while revenue increases steadily, the stock price often moves more dramatically. This highlights that stock market sentiment, investor confidence, and external factors such as market speculation often influence Tesla’s stock price more than revenue growth alone.

3. **Key Observations**:
   - Despite a steady increase in revenue, Tesla's stock price shows much more fluctuation, indicating that other factors, such as investor sentiment and external market conditions, play a significant role in stock price movements.
   - The correlation between stock price and revenue becomes clearer in the long term, with both trends pointing to Tesla’s growth as a leading electric vehicle manufacturer.
   - The sharp increase in both stock price and revenue in recent years demonstrates Tesla's growth and strong financial performance, particularly as the company has become profitable and increased its production capacity.


### GameStop Stock Data and Revenue Analysis:
![GameStop Stock Price and Revenue](https://github.com/jaiswalchitransh/Analyzing-Historical-Stock-Data/blob/main/Sample%20Output/gamestop_stock_graph.png)
*Figure 2: GameStop's Stock Price (Blue) and Revenue (Green) Over Time.*

1. **Stock Price Trend**:
   - GameStop's stock price shows relatively stable and modest fluctuations until early 2021, when there is an unprecedented spike. This spike was primarily driven by the **GameStop short squeeze event**, where retail investors from Reddit’s WallStreetBets community caused a dramatic increase in the stock price, forcing short-sellers to cover their positions.
   - After reaching historical highs in early 2021, the stock price gradually declined, though it remains higher than its pre-surge levels.

2. **Revenue Trend**:
   - In contrast to the stock price, GameStop’s revenue shows a decline over the same period, particularly after 2017. This reflects the company's struggle to compete in the evolving video game retail industry, where digital downloads, online marketplaces, and new business models such as cloud gaming have gained prominence.
   - The revenue decline is consistent with GameStop’s loss of market share to digital platforms like Steam, PlayStation Store, and Xbox Marketplace, which have reduced the need for physical game sales.

3. **Key Observations**:
   - The divergence between stock price and revenue is stark. While GameStop's revenue has been declining, its stock price surged dramatically due to external factors like retail investor activity and short interest, rather than fundamental business performance.
   - The 2021 short squeeze highlights how market events, speculation, and investor sentiment can lead to stock price movements that are disconnected from the company’s financial performance.
   - Post-2021, GameStop’s stock price remains elevated compared to pre-surge levels, but the company’s revenue continues to face challenges, indicating ongoing difficulties in its core business model.


### Conclusion
The comparison between Tesla and GameStop highlights two very different stories:
- **Tesla**: The stock price aligns more closely with revenue growth, though it also experiences speculative surges. This is typical for a company in a high-growth industry (electric vehicles) with strong future potential. Tesla’s stock movements are influenced by a combination of financial performance, investor sentiment, and broader market trends like the rise of electric vehicles.
  
- **GameStop**: The stock price is largely decoupled from revenue performance, showcasing how market phenomena like the short squeeze can lead to stock price movements that are not tied to the company’s financial fundamentals. GameStop’s stock surge in early 2021 was driven by speculative trading rather than any improvement in its business operations, reflecting a unique case in stock market history.

These visualizations provide a deeper understanding of how stock prices and revenues interact and highlight the importance of considering multiple factors—financial performance, market trends, and investor sentiment—when analyzing stock movements.


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
