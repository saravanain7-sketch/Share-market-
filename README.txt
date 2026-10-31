CPR Market Intelligence Dashboard — Decision Engine Upgrade

Files: index.html

What changed:
- Added Bullish / Bearish / Sideways / Wait classification for NIFTY 50 and SENSEX.
- Added price-action confirmation selectors for both indices.
- NIFTY OI bias is derived from positive Call/Put OI changes when present, otherwise PCR is used as a limited contextual filter.
- SENSEX OI context is manually selected because the existing dashboard has no SENSEX option-chain table.
- Generates entry reference, stop-loss, Target 1 and Target 2 for confirmed directional setups.
- Uses existing CPR resistance/support levels; if no forward levels remain, uses 1R/2R projections.
- Does not connect to live market data or place orders.

Calculation integrity:
The existing CPR formula statements and calculations in calc() were retained. The new decision engine is a separate layer and reads the already-calculated values.

Use:
Open index.html in a modern browser. Enter market values, select price-action confirmation, update OI data, and review the classification.

Educational tool only; not investment advice. Verify values and risk with your broker before trading.
