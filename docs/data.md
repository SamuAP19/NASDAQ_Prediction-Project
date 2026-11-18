# Description of raw data and all transformations 

## Input / raw-Data

- All features : 
    # --- INDICES ET VOLATILITY ---                    
    "^IXIC": "Nasdaq_composite",              # Broad tech market index
    "^VXN": "Nasdaq_volatility",              # Nasdaq-100 implied volatility (Tech fear index)
    "^VIX": "Volatility",                     # S&P 500 implied volatility (Market fear index)

    # --- interest ---
    "^IRX": "3month_treasury_yield",          # 3-month Treasury yield
    "^FVX": "5y_treasury_yield",              # 5-year Treasury yield
    "^TNX": "10y_treasury_yield",             # 10-year Treasury yield (Tech discounting rate)
    "^TYX": "30y_treasury_yield",             # 30-year Treasury yield

    # --- Base materials- ---
    "DX-Y.NYB": "US_dollar",                  # US dollar index (DXY)
    "CL=F": "crude_oil",                      # WTI crude oil futures
    "GC=F": "gold",                           # Gold futures
    "SI=F": "silver",                         # Silver futures
    "BTC-USD": "Bitcoin",     

- All Stocks in Nasdaq 100 as features : 
'ADBE','AMD','ABNB','ALNY','GOOGL','GOOG','AMZN','AEP','AMGN','ADI','AAPL','AMAT','APP','ARM', 'ASML', 'ALAB', 'ADSK', 'ADP', 'AXON','BKR', 'BKNG', 'AVGO', 'CDNS', 'CTAS', 'CSCO', 'CCEP', 'CMCSA', 'CEG', 'CPRT', 'CRWV 'COST','CRWD', 'CSX', 'DDOG', 'DXCM', 'FANG', 'DASH', 'EXC', 'FAST', 'FER','FTNT', 'GEHC', 'GILD', 'HONA', 'HON', 'IDXX', 'INTC','INTU', 'ISRG', 'KDP', 'KLAC', 'LRCX', 'LIN', 'LITE', 'MAR', 'MRVL', 'MELI', 'META', 'MCHP', 'MU', 'MSFT', 'MSTR', 'MRNA', 'MDLZ', 'MPWR', 'MNST', 'NBIS', 'NFLX', 'NVDA',
'NXPI', 'ORLY', 'ODFL','PCAR', 'PLTR', 'PANW', 'PAYX', 'PYPL', 'PDD', 'PEP', 'QCOM', 'REGN', 'RKLB', 'ROP', 'ROST', 'SNDK','STX','SHOP',SPCX','SBUX','SNPS','TMUS','TTWO','TER','TSLA','TXN','TRI','VRTX','WMT','WDC','WDAY','XEL'


## Transformations : 
Removal of the weekends (Nasdaq is Null during weekends since it is closed)
