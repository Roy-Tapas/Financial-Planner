# Financial-Planner

This repository contains the implementation of following two basic financial tools:  
* The first one is a personal finance planner that will allow users to visualize their savings composed by investments in shares and cryptocurrencies to assess if they have enough money as an emergency fund.  

* The second tool is a retirement planning tool that uses the Alpaca API to fetch historical closing prices for a retirement portfolio composed of stocks and bonds, then run Monte Carlo simulations to project the portfolio performance at 30 years. Monte Carlo simulated data is then used to calculate the expected portfolio returns given a specific initial investment amount.

---

## Following concepts are used:  
* API call to get external stock trading data into JSON format for a particular date
* Slicing JSON data to get the required information
* API call to get years of past stock trading data and load into Pandas DataFrame to run Monte Carlo simulation
* Monte Carlo simulation to predict portfolio performance at a specific confidence interval
* Plotting simulation result and corresponding probability distribution

---

### Resources

This implementation utilizes two APIs:

* The **Alpaca Markets API** will be used to pull historical stocks and bonds information.  
    
* The **Alternative Free Crypto API** will be used to retrieve Bitcoin and Ethereum prices.

The documentation for these APIs can be found via the following links:

* [Free Crypto API Documentation](https://alternative.me/crypto/api/)

* [AlpacaDOCS](https://alpaca.markets/docs/)
---

## How to run the script <br>
Clone the entire "whale-analysis" repository into a local folder by issuing the following command from gitbash  
```
$git clone https://github.com/Roy-Tapas/financial-planner.git
```

After successfully cloning the repository, change the directory to 'financial-planner'

open Jupyter lab by issuing the following command from gitbash:  
```
$Jupyter lab
```
Create a .env file and enter your API keys for the following:
* ALPACA_API_KEY = "enter your key here"
* ALPACA_SECRET_KEY = "enter your key here"

Open financial_planner.ipynb in jupyter notebook and run each cells one after another.

## Important points to note 
Retain the folder structure as cloned from github.  
Hierarchy inside financial-planner should look like the following:
```
financial-planner 
        |---------------> README.md 
        |---------------> financial-planner.ipynb 
        |---------------> MCForecastTools.py 
        |---------------> .env
```



<hr style="border:2px solid blue"> </hr>

## Tapas Roy

**Email:** rtapask@gmail.com