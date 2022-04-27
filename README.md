# RiskEstimator
Question 1 and 2 solution and implementation could be found at
[Google Colab Run](https://colab.research.google.com/drive/1pXOhnbCG_tHUmtp6lOFY30H4_4tdWt4J?usp=sharing)

If you can't access Google Colab, the corresponding Jupyter Notebook File can also be found at:
[JupyterNotebook](https://github.com/zijianKING/RiskEstimator/blob/main/JupyterNotebook/Programming_and_Risk_Calculation.ipynb)

# Bonus Project:
## Project Description
Build an interactive website that does the following.

(1) Build a customized portfolio of equities (index ETFs or single names like AAPL) with a UI allowing users to pick and allocate weights to individual equities. The sample portfolio in Q1 above is an example.

(2) Pulls market data from Yahoo Finance (or your favorite financial market data vendor) for the equity portfolio constructed above.

(3) Perform risk calculation of your customized portfolio using the investment risk methodology established above.
The goal is to assess the market risk of any custom built portfolios (provided the required market data are available).

## Project Site: 
http://risk.zjtoronto.com:8000/

## Current Phase:
The current website is able to pull market data from Yahoo Fiance, and portfolio weight assignment as well as risk estimation function is still under development.

### Current Web app Details:
1) [Stock Porfolio Section](http://127.0.0.1:8000/stocks/):
  - This tab is designed to let user build up their own portfolio
  - The weight function is still in progress
 <img width="1153" alt="image" src="https://user-images.githubusercontent.com/31417311/165530436-8073fcb2-4e86-4035-b3ae-262dc9a734c8.png">

2) [Dashboard Section](http://risk.zjtoronto.com:8000/dashboard/)
  - The website is able to retreieve stock historical data from Yahoo Fiance in the  Section
  - However, the user need to save tickers data in a [Companylist.csv](https://github.com/zijianKING/RiskEstimator/tree/main/data) file
  <img width="1101" alt="image" src="https://user-images.githubusercontent.com/31417311/165529613-0c9ee935-1db3-4eda-92d9-647eb1f934d1.png">
  
3) [Stock Look Up](http://127.0.0.1:8000/)
  - Look up the stock price and info on Yahoo Finance 

## Libraries and Dependencies
werkzeug==2.0.3<br/>
dataframe-image<br/>
pandas~=1.1.5<br/>
numpy~=1.21.1<br/>
matplotlib~=3.4.2<br/>
DateTime~=4.3<br/>
requests<br/>
dash<br/>
django-mathfilters<br/>
channels<br/>
yfinance<br/>
channels-redis<br/>
pandas_datareader<br/>

## Development Note
1. Install [Django](https://www.stanleyulili.com/django/how-to-install-django-on-windows/) Web Framework

2. Download all dependencies in requirements.txt by running `pip install -r requirements.txt` in command line.
Notice that the website is developed on MacBook with M1 chip, there may be some diffences when installing on a Windows or Mac with Intel Chip.

3. A virtual environment is preferred. You can, for example, build it on [PyCharm](https://www.jetbrains.com/zh-cn/pycharm/) with "Add Python Interpreter" -> "Virtualenv Environment".

4. Run the website locally by input `python manage.py runserver` on the terminal

Shoot me an email if anything doesn't work for you

## Technical Specification
I used Python Django Framework and build up a quick web app to track stock ticker information and price. Then using Dash apps the information is graphed with multiple tickers in an interactive graphic.

Plotly Dash (with Django)
Creates an interactive dashboard where you can select the dates and stocks to compare the share price history. Share price information is gathered from Yahoo through the Pandas Data Reader tool. By using Plotly Dash, the user can hover and interact with each stock, updating the tickers live.

graph_dashboard
![image](https://user-images.githubusercontent.com/31417311/165445444-977fe769-4217-4996-a684-f141c9bcf2d0.png)

Users can also add & remove stocks to a table of their favourites to easily have on hand.
![image](https://user-images.githubusercontent.com/31417311/165445471-68c8352a-c6df-4596-933f-5e2c3de95b4b.png)

stock_favourites

Individual information about the company and share data can be looked up, which is connected to the IEX API for the latest company information.

stock_lookup
![image](https://user-images.githubusercontent.com/31417311/165445494-ec797362-512b-4e01-8cfd-92a9abc67fc4.png)

## Contact
email utzijian.wang@mail.utoronto.ca
