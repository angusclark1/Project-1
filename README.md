#Project-1

##New Age vs Old Age: what comes out on top?

###Background

###What You're Creating

This project aims to analyze and compare the performance of two portfolios:

Old Portfolio – made up of more traditional investments. Holdings include;

Walt Disney (DIS)
Coco-Cola (KO)  
CBA (CBA)
Berkshire Hathaway (BRK-B)
Johnson and Johnson (JNJ)
Gold (SPDR Gold Shares) (GLD)
 
New Portfolio – made up of new age investments. Holdings include;

Apple (AAPL)
Bitcoin (BTC)
Etherium (ETH_USD)
Lithium (Global X Lithium & Battery Tech ETF) (LIT)   
Tesla (TSLA)
Tether (USDT-USD)

###Project Analysis

This project aims to analyse and compare the New and Old portfolios through the following files:
·      Portfolio Data and Analysis (Jupyter Notebook) - Used to collate and analyse Old and New Portfolios against the Dow Jones over a historical two year period
·      Portfolio Value Calculation Tool (Jupyter Notebook) - Used to calculate the current AUD value of the Old and New Port
·      Monte Carlo Simulations (Jupyter Notebook) – Used to simulate the performance of the Old and New portfolios 5 years into the future 

###Portfolio Data and Analysis:

Tools used:
·      yfinance as yf
·      pandas as pd
·      numpy as np
·      datetime as dt
·      seaborn as sns
·      pathlib import Path
·      matplotlib.pyplot as plt
·      seaborn as sns
·      hvplot.pandas

Within this part of the project Yahoo Finance has been utilised to pull in historical data over a two year period to create two portfolios; Old Portfolio and New Portfolio.

A third portion of data has also been pulled in for the Dow Jones in order to compare the performance of the two portfolios against the performance of the Dow Jones Industrial Average, which consists of an index of 30 prominent companies listed on stock exchange in the United States. 
 
This data has then been used to create two grouped data frames consisting of the percentage change in the closing prices and the cumulative returns for the instruments held within the New and Old Portfolio’s and the closing prices of the Dow Jones over a two year period. 
 
This data can be manipulated by changing the set tickers at the beginning of the notebook.
 
From the data frames created a few factors have been used to analyse and compare the portfolios against each other and against the performance of the Dow Jones.
 
They have been compared using:
 
Standard Deviation
Cumulative Returns 
Percentage Change
Sharpe Ratios

##Monte Carlo Simulations:

Monte Carlo simulation performs risk analysis by building models of possible results by substituting a range of values—a probability distribution—for any factor that has inherent uncertainty. It then calculates results over and over, each time using a different set of random values from the probability functions.

Tools used: 
·      yfinance as yf
·      pandas as pd
·      numpy as np
·     from MCForecastTools import MCSimulation 
·      pathlib import Path
·      matplotlib.pyplot as plt
·      hvplot.pandas
·      import os

To further make analysis of the two portfolios, a MonteCarlo simulation has been used. We used Yahoo Finance to collect and combine recent data to create the two data frames. Next, the simulation was imported and the weights, number of simulations and number of trading days was set. By then using the calculated cumulative return function, we calculated the cumulative return of the two portfolios and plotted the simulation results. To easier understand the returns, an investment of $10,000 was calculated with the simulated returns. The old age portfolio performed positively based on the simulation and over the 1000 simulations, there was a 95% chance the portfolio would be worth between $9184 and $14953 from the $10,000 investment. The new age portfolio was run 1000 times and from a $10,000 initial investment our portfolio in a year would be worth between $15,524 and $30,491. The accuracy of the simulation may be slightly lessened due to the market bounce back after coronavirus. 

To assess furthermore the difference between Monte Carlo simulations and the results that can be received, we added a few different components to the task, the new age simulation was ran 1000 times and our old age simulation was ran 100 times; this can create a varied result whilst both are accurate it highlights the versatility of the Monte Carlo Simulation. Our old age simulation we plotted ‘Daily Returns Behaviour’ and in our new age portfolio we plotted ‘Cummulative Return Trajectories’, creating these multi-faceted takes on the MCS to see how versatile both the simulation and the portfolios can be. Due to the nature of the volatility and fluctuation in our new age portfolio, the projected possible returns are much higher than the old age portfolio but as we all know, high risk high reward; the simulation highlights this. The causes of the fluctuation in our new age portfolio is due to the general volatility of the crypto centric new age portfolio. Both portfolios have shown optimal performance and by utilising the risk analysis tool of Monte Carlo, we have a more clearer picture of the future of these two portfolios.

##Portfolio Value Calculation Tool

Tools used:
·      os
·      requests
·      json
·      pandas as pd
·      dotenv import load_dotenv
·      alpaca_trade_api as tradeapi
·      yfinance as yf
·      %matplotlib inline
 
Within this part of the project Yahoo Finance and Alpaca Trade API has been utilised to pull in current closing price data for all instruments held within the Old and New Portfolios in order to calculate the current AUD value of each portfolio.
The tool can be manipulated to calculate the current value of an adjusted portfolio but changing the set tickers and updating the set units held of each ticker and updating the chosen closing prices.
 
The tool calculates the current AUD value of both portfolios and prints a comparison statement of both values at the end of the Jupyter Notebook.
