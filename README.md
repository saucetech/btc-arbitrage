# btc-arbitrage
This project retrospectively analyzes potential arbitrage opportunities in Bitcoin across Bitstamp and Coinbase in several months of 2018. Pandas is used to apply three phases of financial analysis to determine if any arbitrage opportunities exist in historical trade data for Bitcoin. The three phases are data collection, data preparation, and data analysis. The data 


## Technologies
This project leverages Python 3.7 with Pandas and Matplotlib Inline in Jupyter Lab. 


## Installation Guide
This project does not require any additional packages. 

## Usage
To review the analysis, simply clone the repo and open the notebook in Jupyter Lab.

## Analysis Summary
This project analyzes Bitcoin prices using CSV data from January to April of 2018 across the Bitstamp and Coinbase exchanges. 

In the data collection phase, the data is imported from the Resources folder into the notebook using a datetime format.

In the data preparation phase, the data is then cleaned by dropping all missing values and duplicates, removing the dollar sign in the Close column, and converting the resulting string into a float.

In the data analysis phase, the closing price from both exchanges are narrowed down into three dates: early (January 16), middle (February 24), and late (March 26) in the dataset in order to observe any patterns or trends in arbitrage opportunities.

Statistical summaries are created for the data across the three dates. The price graph is plotted and the prices across both exchanges are overlayed against each other in order to visualize price discrepancies.

The arbitrage spread across the two exchanges are also calculated and visualized as a box plot. 

The spread return is then calculated across all three dates.The profitable trades are then calculated to determine the number of times the trades returned positive returns with a minimum 1% threshold needed to cover costs. The potential profit per trade is also calculated as well as the cumulative sum of profitable trades. 

According to the data analysis, the arbitrage opportunities, profit per trade, and cumulative profits decreased as time progressed. In January 16, 2018, the average profit per trade was 193.80. The average profit per trade decreased to 110.02 on February 24, 2018, and then to 0.00 on March 26, 2018. On January 16, the cumulative profits were 14147.17. This decreased to 330.07 on February 24, and to 0 on March 26. There were 73 profitable trades on January 16, 3 on February 24, and 0 on March 26. Thus, the potential arbitrage opportunities decreased over time in Q1 of 2018.

## Contributors
Brought to you by Austin Do. Email: austindotech@gmail.com

## License
MIT