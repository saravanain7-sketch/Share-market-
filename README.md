# CPR Market Intelligence Dashboard

## Run
Open `index.html` in Chrome, Edge, Firefox, or a mobile browser. No installation or server is required.

## Features
- Responsive NIFTY 50 and SENSEX dashboards
- CPR: TC, Pivot, BC, width, relationship (when prior CPR is entered)
- R1/R2/S1/S2 and previous-day high/low
- VWAP position and conditional intraday interpretation
- Option-chain Call OI / Put OI totals, PCR, highest-OI strikes
- India VIX context
- CSV report export and illustrative demo values

## Important data limitation
This version is a standalone dashboard and does not fetch live exchange data or connect to a broker. Enter values manually or build a secure server-side integration with a licensed market-data provider. Never expose broker/API secrets in browser JavaScript. Demo values are illustrative and are not current market data or trade recommendations.

## Calculations
Pivot = (Previous High + Previous Low + Previous Close) / 3  
BC = (Previous High + Previous Low) / 2  
TC = 2 * Pivot - BC  
CPR width (%) = abs(TC - BC) / Pivot * 100  
R1 = 2 * Pivot - Low; S1 = 2 * Pivot - High  
R2 = Pivot + (High - Low); S2 = Pivot - (High - Low)  
PCR = Total Put OI / Total Call OI

Educational use only. Verify all inputs and market levels with your exchange/broker.
