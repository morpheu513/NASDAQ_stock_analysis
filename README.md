# Stock Analysis

This project deals with understanding how covid-19 has impacted the stock market. For our analysis we have considered 50 companies from various secotrs.
All 50 stocks are dealt in NASDAQ/NYSE market
which are of mostly large & mid cap stocks and a few small caps as well
and we have tried to study the impact of 2007-09 economic recession and the current pandemic on all the following stocks. And predict the nature of the stocks if not for the pandemic.

## Table Of Contents:
* [List of Sectors](#list-of-sectors)
* [List of Companies](#list-of-companies)
* [Directory Structure](#directory-structure)
* [Requirements](#requirements)


## List of Sectors 

There are stocks from all categories:
```
Energy
Materials
Industrials
Utilities
Healthcare
Financials
Consumer Discretionary
Consumer Staples
Information Technology
Communication Services
Real Estate
```


## List of Companies
```
'AXP'-American Express Financial services
'AAPL'-Apple Technology
'AMZN'-Amazon.com E-commerce
'ADBE'-Adobe Computer software
'ADS'-Alliance Data Systems Corporation
'BA'-Boeing Aerospace
'BAC'-Bank of America Investment banking
'CAT'-Caterpillar Inc. Construction machinery and equipment
'CVX'-Chevron Corporation Oil industry
'CSCO'-Cisco Systems Networking hardware
'COST'-Costco Retail
'DIS'-The Walt Disney Company Mass media
'FB'-Facebook Social Media
'GE'-General Electric Multinational conglomerate
'GS'-Goldman Sachs Investment banking
'GOOGL'-Alphabet Inc. Multinational conglomerate
'HD-The Home Depot Home improvement'
'HDB'-HDFC Bank Financial services
'HOG'-Harley-Davidson motorcycle manufacturer
'IBM'-IBM Computer hardware
'INTC'-Intel Semiconductor
'INFY'-Infosys Information technology consulting
'JNJ'-Johnson & Johnson Medical device
'JPM'-JPMorgan Chase Investment banking
'JBHT'-J.B. Hunt Transportation and Logistics
'KO'-The Coca-Cola Company Beverages
'KEX'-Kirby Corporation Transportation
'MCD'-McDonald's Fast food
'MSFT'-Microsoft Corporation Technology
'MMM'-3M Multinational conglomerate
'MRK'-Merck & Co. Pharmaceutical
'NFLX'-Netflix Production
'NKE'-Nike Footwear manufacturing
'NVDA'-Nvidia Computer Hardware and Software 
'PFE'-Pfizer Pharmaceutical
'PG'-Procter & Gamble Consumer Goods
'PEP'-PepsiCo Food
'REGN'-Regeneron Pharmaceuticals Biotechnology
'SBUX'-Starbucks Coffeehouse
'TRV'-The Travelers Companies Insurance
'TGT'-Target Corporation Retail
'T'-AT&T Telecommunications
'UTX'-Raytheon Technologies Corporation Aircraft manufacturing
'UNH'-UnitedHealth Group Managed care
'UPS'-United Parcel Service Logistics
'UNP'-Union Pacific Corporation Transport
'VZ'-Verizon Communications Telecommunications
'WMT'-Walmart Retail
'XOM'-ExxonMobil multinational oil and gas
'YUM'-Yum! Brands Fast food
```

## Directory Structure:
```
.
|-- data
|   |-- ..  
|-- src
|   |-- data_collection.ipynb
|   |-- eda.ipynb
|   |-- arima.ipynb
|   |-- rnn.ipynb
|   |-- arima_lstm_hybrid.ipynb
```
```src``` contains all notebooks which contain the source for the project. 
3 models have been used to analysie and make predictions for the dataset.All models used can be found under the ```src``` directory.
The naming convention for the models are as follows : ```<model_name>.ipynb```


## Requirements:
This project has multiple requirements which need to be installed in order to run the source files.
Most of the requirements can be installed by using the ```requirements.txt``` file. To install these requirements type:
```
pip install -r requirements.txt
```
Another library we have used is the Technical Analysis library. Sometimes this gives an error if we directly try to install it via ```pip```. Hence follow the steps to install the TA-Lib:
```
wget https://launchpad.net/~mario-mariomedina/+archive/ubuntu/talib/+files/libta-lib0_0.4.0-oneiric1_amd64.deb -qO libta.deb
wget https://launchpad.net/~mario-mariomedina/+archive/ubuntu/talib/+files/ta-lib0-dev_0.4.0-oneiric1_amd64.deb -qO ta.deb
dpkg -i libta.deb ta.deb
pip install TA-Lib==0.4.17
```
All notebooks were created and executed on [Google Colab](https://colab.research.google.com/) and the contained source code can be executed.
<br>

**Note:** Before executing the soruce code on google colab make sure you have uploaded the [data](https://github.com/morpheu513/NASDAQ_stock_analysis/tree/master/data) onto your drive. 