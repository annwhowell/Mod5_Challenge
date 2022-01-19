# Mod5_Challenge

#Overview
This notebook contains two parts.
    Part 1 - Evalutes a portfolio that includes crypto currency and stocks and bonds to determine if the client has enough money for a solid emergency fund. 
    Part 2 - Uses Monte Carlo simulations for the stocks and bonds part of the same portfolio to consider performance of the portfolio in 30 years and ten years. 
    
    
#Inputs
This noteboks requires importing several python libraries

import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation

%matplotlib inline


#Data retrieval
For Part 1: Use Python Requests library to pull data for Bitcoin (BTC) and Ethereum (ETH)

For Part 1 and Part 2, use the Alpaca SDK to pull data on stock (SPY) and bond (AGG) prices
    You must create a .env file for your Alpaca_key and Alpaca_secret_key in order to pull needed data from Alpaca
    Call the .env file using load_dotenv()
    Use the Alpaca tradeapi.REST object

