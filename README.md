# Relationship-Between-Corporate-ESG-Performance-and-Profitability
# Introduction<br>

As global extreme weather events become more frequent and political situations remain unstable, companies are facing unprecedented operational challenges, with supply chain disruption risks increasingly growing. To address these challenges, more and more countries are responding to ESG (Environmental, Social, and Governance) issues and establishing related regulations. For instance, the European Union's Carbon Border Adjustment Mechanism (CBAM) will officially begin levying carbon tariffs on January 1, 2026; Taiwan requires listed and over-the-counter companies to prepare sustainability reports and declare carbon fees starting in 2025. Under such trends, corporate sustainability performance is no longer just a future vision but a critical factor directly impacting operational performance.

Moreover, sustainable investing has become a significant trend in capital markets. ETFs using sustainability as a stock selection indicator are showing notable performance. According to Bloomberg data, from October 2013 onwards, the "Emerging Markets Sustainable" and "Asia-Pacific Sustainable" indices have recorded approximately 13.54% and 4.62% excess returns, respectively, compared to the "Emerging Markets Stock" and "Asia-Pacific Stock" indices.

As sustainability issues increasingly gain attention, the correlation between corporate sustainability performance and stock price performance is gradually drawing focus. Many investors have incorporated ESG scores into their stock selection criteria, believing these can influence investment returns. Therefore, this report will explore whether corporate sustainability performance truly impacts company stock prices.

# Relative Research

According to research by Lasse Heje Pedersen, a professor at Copenhagen Business School, in his work 'Responsible Investing: The ESG-Efficient Frontier', the study explores the impact of ESG ratings on investors' efficiency frontier. The research methodology involves monthly sorting stocks into five quintile portfolios based on ESG scores, and processing them using equally-weighted (Panel A) and market capitalization-weighted (Panel B) approaches. The portfolios were then subjected to three-factor, five-factor, and six-factor models to analyze return differences between high and low ESG score portfolios.

The research results indicate that high ESG score portfolios may generate positive abnormal returns in most cases, but the final outcomes are influenced by weighting methods and the selection of control factors. Therefore, market participants should remain cautious when interpreting the impact of ESG scores on returns and consider the interactions between ESG scores and other risk factors.

After evaluation, we believe that risk factors are difficult to fully control, and different market factors may impact the results. To simplify the analysis and avoid overfitting, this report will randomly select 40 companies from the first and last-ranked intervals. This approach effectively focuses on companies with extreme ESG performance and provides a clearer comparison of results.

# Methodology

__Optimization and Risk-Return Analysis of Stock Portfolios Based on Corporate Governance Ratings__<br>

Designed for stock portfolio analysis, the specific purpose is to help investors select the most suitable investment portfolio based on the returns and risks of different stocks. The program covers stock data retrieval, statistical calculations, portfolio optimization, and visualization of the efficient frontier and capital allocation line. Below is a detailed analysis of each component:

__1. Download and import packages:__

__openpyxl__: Used for handling Excel files. In this program, this library is used to read and process the list of companies and related stock codes stored in Excel.<br>
__random__: Used for randomly selecting companies. During the analysis process, this might involve randomly choosing a certain number of companies for analysis.<br>
__pandas__: Used for data processing. This library is utilized to handle stock data in DataFrame format, conduct various statistical operations, and perform data cleaning.<br>
__numpy__: Provides mathematical computation functions, primarily used for matrix operations such as the weighted sum of mean returns and the calculation of covariance matrices.<br>
__yfinance__: This library is used for fetching stock data from Yahoo Finance, capable of automatically downloading historical price data for specified stocks.<br>
__matplotlib.pyplot__: Used for generating charts. In the program, this library is used to plot the efficient frontier, capital allocation line, and indifference curve.<br>
__scipy.optimize.minimize__: This tool is used for solving optimization problems. In this code, this function is used to calculate the portfolio with the maximum Sharpe ratio.<br>
