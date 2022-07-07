# Project-1

## New Age vs Old Age: what comes out on top?

## Background

### What You're Creating

For this Challenge assignment, you’ll need to create and submit the following deliverables:
A Jupyter notebook that contains an analysis of the portfolio of the new age of innovative businesses (such as buy now pay later, eco-technology and neo banks for example). Additionally, create another portfolio detailing the traditional financial businesses such as insurance and banking, in order to provide an analysis with professionally styled and formatted interactive visualizations and input. Remember to upload your Jupyter notebook for this assignment to the GitHub repository. Make sure to update the README.md file to explain the project and any information that’s needed to interact with the graphs and plots.


### Project Analysis 

- Use the Project1.ipynb notebook to visualize and analyze the new and old age financial entities which can be accessed within the Project Challenge files.

Note that this assignment requires you to create a Monte Carlo Simulation . 

- Use the project1.ipynb notebook to complete the following tasks:

Pull in data and analyze how the two portfolios track in the current market in comparison to each other. 

Compare how both portfolios performed in comparison to 2 years previously during the covid upswing in prices (particularly In tech). 

Compare the performance of both portfolios against more historical data in a 10-year time frame.

Analysis and describe the difference in performance. Suggest why one investment method may be preferable to the other. Taking into consideration the current economic climate of Australia and the world.

## Pull in the data and analyze how the two portfolios track in the current market.

For this part of the assignment, two portfolios will be used to analyze, in order to show how both portfolios compare to one another.

1. Import neccessary tools for analysis
- Pandas as pd
- MCSimulation from MCForecastTools
- yfinance as yf
- matplotlib.pyplot as plt
- seaborn as sns
- hvplot as hv
- streamlit as st

2. Identify and Set appropriate tickers for both Old Age and New Age Returns.
3. Create a DataFrame which includes tickers
4. Set start and end date within the df
5. Drop all null values from both Portfolio's
6. Visualise the data in order to confirm no values are missing (Using a Heatmap)

## Compare how both Portfolios performed in comparison to 2 years previously (Perform Quantitative Analysis)
For this part of the assignment, use the Old Age and New Age returns Dataframe to compare how both portfolios performed in comparison to both 2 years prior. To do so, complete the following steps:

- Note in order to visualise simulations, download MCS files.

1. Create a new DataFrame named MC_two_year, which includes the original DataFrame, as well as weights, number of trading days and number of simulations.
2. Using MCForecastTool.py, create a Monte Carlo Simulation for the DataFrame for a 2 year simulation. Be sure to do the following: num_simulation=1000, num_trading_days=252*2 and set weights to 0.1 respectively.
3. Using the calc.cumulative_return() function, calculate the Dataframes 2-year cumulative return.
4. Plot the MCSimulation and Distribution

- Note that your resulting Monte Carlo Simulation and Distribution Plot should appear similar to the following image

<img width="590" alt="Screen Shot 2022-07-07 at 8 27 42 pm" src="https://user-images.githubusercontent.com/102783432/177758341-2278b4b9-cb15-44bc-8858-85915339a31d.png">

<img width="468" alt="Screen Shot 2022-07-07 at 8 30 55 pm" src="https://user-images.githubusercontent.com/102783432/177758676-d8785c07-3b13-4fc2-94c1-439e287f066e.png">

## Compare the performance of both portfolios against more historical data in a 10-year time frame.
For this part of the assignment, use the Old Age and New Age returns Dataframe to compare how both portfolios performed in comparison to more historical data. To do so, complete the following steps:

1. Using the group_df, read in the Data Frame and display.
2. Using MCForecastTool.py, create a Monte Carlo Simulation for the DataFrame for a 10-year simulation. Be sure to do the following: num_simulation=300, num_trading_days=252*10 and set weights )
3. Using the cumulative_returns function, calculate the Dataframe’s 10-year cumulative return for the Dataframe
4. Plot the MCSimulation’s and the Distribution

## Compare and Analyse the plots in order to determine which portfolio may be most sensible.
Run Monte Carlos Simulations to compare and analyze how both portfolios differentiate to the future market.

## Analysis and describe the difference in performance.
Provide a detailed analysis and description on the differences in the performances of the portfolios against one another. 
Suggest why one Portfolio may be preferable to the other. 

Remember to take into account the current Economic Factors:

- Interest Rate fluctuations.
- Inflation Rate fluctuations.
- Probability of fluctuations in unemployment and wage growth failing to compete with inflation.
- The effects of Australia’s heavy investment in the property market during all-time low-interest rates.
- The possibility for the economy to hit an economical downswing.
- Human-related effects (e.g. failing to meet mortgage repayments).
