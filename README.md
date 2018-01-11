# DJIA Company Data
##  Using Wikipedia and Quandl

Gathers tickers from Wikipedia and data from Quandl to get a pandas dataframe of the adjusted
closes for all the companies in the DJIA. This script will download the 30 companies individual
data into a directory named *DJIA_Data* which is located in the same directory as where the script is ran. This uses Jupyter Notebook

### Quandl to gather data
Uses Quandl's API to gather data for the individual companies.
  * The relatively small amount of calls to Quandl were fine without an API key. Quandl has an anonymous user limit of 50  calls per day. (Sometimes there is an 20 call limit within 10 minutes) However,
    if you do create an account, you are given a key and won't be restricted to the amount of calls you make to their API.

### Packages
* _Pandas_ - for data analysis
* _Requests & BeautifulSoup_ - for web scraping
* _Matplotlib & Seaborn_ - for plotting
* _os_ - making directory
* _datetime_ - for boolean indexing
* Will need Jupyter Notebook to run script
