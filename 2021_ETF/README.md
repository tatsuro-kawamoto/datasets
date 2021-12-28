![ETF (Exchange Traded Fund) dataset in 2021](./figures/logo.png)

This dataset is a weighted undirected bipartite network of the ETF (Exchange Traded Fund) in 2021. 


## Data construction details
The dataset was built based on the information on a webpage of MONEX Inc.: 
[https://mst.monex.co.jp/mst/servlet/ITS/ucu/UsSymbolListGST?etf=1](https://mst.monex.co.jp/mst/servlet/ITS/ucu/UsSymbolListGST?etf=1) (Japanese)

- The ETFs are listed on exchanges in the US (e.g., NASDAQ, NYSE Arca). 
- A bipartite network is constructed in which there are two types of nodes: i) ETFs (i.e., fund nodes) and ii) stocks and securities (i.e., asset nodes). A fund node and an asset node are connected by an undirected edge with weight `value` if the asset accounts for `value`% of the portfolio.
- Since the website of MONEX Inc only shows the top 10 assets for each ETF, in terms of the share in the portfolio, each fund node is connected to at most ten asset nodes. 
- We combined several individual stocks that apparently belong to the same group (e.g., BHP Group Ltd and BHP Group Plc). 
- The largest connected component is extracted.

## Contributors
- Tatsuro Kawamoto
- Teruyoshi Kobayashi
- Yoshitaka Ogisu

## Funding
This dataset was built as a part of the projects in JSPS KAKENHI No. 19H01506.

## Citation
When you use this dataset in your publication, please cite this web page.

