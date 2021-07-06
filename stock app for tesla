import streamlit as st
import yfinance as yf
import pandas as pd

st.write("""
         # Simple stock price app
         
         shown are the stock **closing price and volume** of tesla!
         
         """)

tickerSymbol = 'TSLA'

tickerData = yf.Ticker(tickerSymbol)

tickerDf = tickerData.history(period='1d', start='2016-7-11', end='2020-7-6')

st.write("""
### Closing Price
""")
st.line_chart(tickerDf.Close)

st.write("""
###  Volume of the stock
""")
st.line_chart(tickerDf.Volume)

