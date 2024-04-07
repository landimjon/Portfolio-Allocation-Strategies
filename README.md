<h1 align="center"> Portfolio-Allocation-Strategies</h1> 

The Equal Weight and Modern Portfolio Optimisation (MPT) portfolio allocation strategies are compared in this study. Its objectives are to evaluate their eligibility for investment management and analyse their performance using past financial data. While the MPT strategy uses mathematical optimisation techniques to maximise return or minimise risk, the Equal Weight strategy gives each asset in the portfolio an equal weight. The project analyses and visualises data to assess important performance indicators for each strategy, including return, volatility, and Sharpe ratio. The results will help with portfolio optimisation and investment management decision-making processes by offering insightful information to investors, financial experts, and researchers.
<br>

## Prequisities

<br>

Before proceeding, ensure that you have the following:

<br>

1. R and RStudio installed on your machine
2. The necessary R packages installed, including Shiny and any additional packages required by the scripts

### Required Packages 📦:

<br>

- `library(tidyquant)`
- `library(PerfomanceAnalytics)`

<br>

Please make sure to install the required packages before running the Shiny app.

## Installation and Setup

<br>

1. Download all the scripts related to this draft version of the Shiny app. 
2. Create a new directory for your Shiny project in RStudio. 
3. Move all the downloaded scripts into this directory.

<br>

## Dataset

<br>

The dataset includes monthly data on production, imports, exports, refinery output, stock levels, and prices of gasoil/diesel across European countries.

<br>

## Data Sources

-	Quandl

-	Yahoo Finance

-	Federal Reserve Economic Data (FRED)

-	Bloomberg

-	Reuters

## Data Structure

-  `year`: Year of the data record (2017-2024)
-  `month`: Month of the data record (1-12)
-  `country`: Name of the country
-  `Refinery_Output_kb`: in thousaud barrels per day 
-  `Import_kb`:Imports in thousaud barrels per day 
-  `Export_kb`:Exports in thousaud barrels per day 
-  `Demand_kb`:Demand in thousaud barrels per day 
-  `closing_stock_kmt`: Closing stock in thousaud metric tons 
-  `price_usd`: Price of gasoil in USD per ton

<br>

## Analysis

The analysis includes:

-  Based on your risk tolerance, the code creates a conservative portfolio comprising 10% REITs, 10% equities, and 80% bonds.
-  It downloads historical price data and calculates daily returns for each asset class.
-  The code uses metrics like annualized return, standard deviation, and Sharpe Ratio to analyze portfolio performance.
-  It offers a performance report and an optional plot of the portfolio's daily returns for visualization purposes.
- The results will offer insightful information to investors, financial experts, and researchers, helping them make informed decisions about portfolio optimization and investment management.

<br>

## Files 

-  `europe_gasoil_data.csv`: Main dataset file containing gasoil data for European countries.
-  `analysis_script`: R script file for performing data analysis and generating reports.
-  `monthly_stock_changes.csv`: Generated file with details of stock builds or draws for each month.
-  `price_trend_analysis`: Visualistion of price trends over time.  

## Execution Order

<br>

To properly run the Shiny app, execute the scripts in the following order:
1. `Heurst_PVC_Class_1.R`
2. `Heurst_PVC_Class_2.R`
3. `Heurst_PVC_Class_3.R`
4. `Heurst_PVC_Class_4.R`
5. `comparisons.R`
6. `decision.R` 
7. `function_cart_graph.R`
8. `decision_with_map.R `
9. `TSP.R` (Run this script last)

## Running the Shiny App

<br>

1. Once all the scripts have been executed successfully, locate and open the `TSP.R` script.
2. Run the `TSP.R` script and wait for approximately 2 minutes.
3. The Shiny app will progressively load and display a map, itinerary, and statistical tables for testing and comparing the heuristics used.

## To install the package 📦

```
library(devtools)

install_github("landimc8/tspHeuris")
```

<br>

## To load the Package 📦

```library(tspHeuris)```

<br>

## To run the app

```runMyApp()```

<br>

This Shiny app uses American bonds, REITs, and stocks to walk you through the analysis of a diversified and conservative portfolio approach. How can we use it? Let's explore!

## Using the Shiny App

-	Open the App: To start examining a diversified and conservative portfolio strategy, open the Shiny app.

-	Explore Allocation: The program first shows an 80/10/10 sample allocation (Bonds, REITs, and stocks).

-	Customise Allocation: Enter your preferred bond allocation (within a reasonable range) using the text box or slider that is provided.

-	Dynamic Analysis: The program recalculates performance indicators dynamically based on your selected bond allocation.

-	Performance Insights: Based on your input, view essential indicators, including the Sharpe Ratio, standard deviation, and annualized return.

-	Visualise Returns: A line chart shows the portfolio's daily returns over time to help you understand possible swings.

Alternatively, you can access the Shiny app directly using the following link:  [Shiny App Demo](https://tsp-heuristics.shinyapps.io/tsp1/)


Please note that this guide assumes basic familiarity with R and RStudio. If you encounter any issues or have further questions, refer to the documentation for the Shiny package or consult the developer of the Shiny app for assistance.

<br>

<div align="center">

  <a href="https://opensource.org/licenses/MIT">![License](https://img.shields.io/badge/License-MIT-yellow)</a>
  <a href="https://www.r-project.org/about.html">![Language](https://img.shields.io/badge/Language-R-blue)</a>
  <a href="https://tsp-heuristics.shinyapps.io/tsp1/">![Demo](https://img.shields.io/badge/App-Demo-indigo)</a>
</div>

The project's structure in RStudio follows a modular approach:

- `Capacity_world`: Contains R scripts and files for visualizing biodiesel capacity data on a refinery level. It includes scripts or functions to process and present information specific to individual refineries.
  
- `Capacity_regions`: Contains R scripts and files to explore biodiesel capacity trends across different regions.
  
- `Data`: Store relevant datasets used in the modeling process.
  
- `Results`: Save model outputs, reports, and visualizations.

<h1 align="center"> Data Sources 📰</h1>

- [Argus Biofuels Feedstocks](https://www.argusmedia.com/en/oil-products/biofuels)

<br>

<h1 align="center">Contributors </h1>

<br>

<div align="center">

Jonatas Nunes Landim
    <br>
    Zildete Landim Crausaz
  <br>
  
</div>

Enjoy using the Shiny app!
