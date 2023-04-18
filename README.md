# UMSI_SI699WIN23_Tesla_Stock_and_News
Predict Tesla stock price trends with news articles

1. `Data`: Codes to Collect Data and some Raw Data collected through downlowading from website
   1. `raw_data`: Store collected raw data and data collected by codes
      - `Europe_Brent_Spot_Price_FOB_modified.csv`: Oil price data downlowded from https://www.eia.gov/dnav/pet/hist/RBRTED.htm
      - `Dow Jones Automobiles & Parts Historical Data.csv`: Automobile market data download from https://www.investing.com/indices/dj-automobiles---parts-historical-data
         
   2. `stock_data.ipynb`: Codes to collect stock price data through `yfinace API`, combine them and existing data in `raw_data` into `stock_price_all.pkl`
     
   3. `news_scraping_api`.ipynb: Codes to collect news articles through `geporigon API` (https://www.goperigon.com/account/api-key) and store collected data into `output.csv`
     
   4. `news_sen_final`.ipynb: Codes to calculate sentiment scores for those news articles through NLP Python Package `nltk` and `flair`, and then store results in `news_sen_score.pkl` 
   
   5. `EDA_plots.ipynb`: Codes to draw plots of collected data.
     
2. `Non_NLP_Model.ipynb`: Codes to implement CNN and GRU models not using the sentiment scores, perform experiments, and store results in the `results` directory

3. `NLP_Model.ipynb`: Codes to implement CNN and GRU models using the sentiment scores, perform experiments, and store results in the `results` directory
