# RiskEstimator
Question 1 and 2 solution and implementation could be found at
[Google Colab Run](https://colab.research.google.com/drive/1pXOhnbCG_tHUmtp6lOFY30H4_4tdWt4J?usp=sharing)

For this repo, the Jupyter Notebook File can be found:
[JupyterNotebook](https://github.com/zijianKING/RiskEstimator/blob/main/JupyterNotebook/Programming_and_Risk_Calculation.ipynb)

# Bonus Project:
## Project Scope
Build an interactive website that does the following.
(1) Build a customized portfolio of equities (index ETFs or single names like AAPL) with a UI allowing users to pick and allocate weights to individual equities. The sample portfolio in Q1 above is an example.
(2) Pulls market data from Yahoo Finance (or your favorite financial market data vendor) for the equity portfolio constructed above.
(3) Perform risk calculation of your customized portfolio using the investment risk methodology established above.
The goal is to assess the market risk of any custom built portfolios (provided the required market data are available).

## Project Site: 
http://risk.zjtoronto.com:8000/

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
1. Download all dependencies in requirements.txt by running `pip install -r requirements.txt` in command line.
Notice that the website is developed on MacBook with M1 chip, there may be some errors when installing on a Windows or Mac with Intel Chip.
2. A virtual environment is preferred. You can, for example, build it on [PyCharm](https://www.jetbrains.com/zh-cn/pycharm/) with "Add Python Interpreter" -> "Virtualenv Environment".
3. Run the website locally by input `python manage.py runserver` on the terminal

Shoot me an email if anything doesn't work for you

## Details
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
