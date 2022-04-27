# RiskEstimator
Question 1 and 2 solution and implementation could be found at JupyterNotebook/Programming_and_Risk_Calculation.ipynb

## Bonus Project:
Link: http://risk.zjtoronto.com:8000/

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
