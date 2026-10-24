# Nexa Bot Rewards — static website starter

## Included
- Responsive dark/gold website
- TradingView XAU/USD embed
- Gold signal center placeholder (does not invent live signals)
- MT4/MT5 integration guidance (no live broker connection included)
- Memberships: $69 monthly, $399 yearly, $799 lifetime
- Proposed 2× internal reward point calculations: 138 / 798 / 1,598 points
- Checkout UI with BTC, ETH, SOL, and USDT BEP20 address display/copy
- Dashboard and referral-code preview
- Create Account / Sign In page UI
- Privacy and terms starter pages

## Deploy
1. Extract this ZIP.
2. In Netlify choose **Add new site → Deploy manually**.
3. Upload the extracted folder contents or drag the files into the deploy area.
4. Test `index.html`, `create-account.html`, `signin.html`, `dashboard.html`, `checkout.html?plan=yearly`, `signals.html`, and `integration.html`.

## Production work still required
This is a polished front-end starter, not a production trading/payment service.
- **Authentication:** Create Account and Sign In are intentionally simple demo pages with no authentication. The Create Account form does not save or send details; Sign In opens the demo dashboard. If you later collect real member details or payments, add appropriate secure backend controls.
- **Reward ledger:** 2× point values are UI calculations only. A trusted server must credit points once, only after verified payment; prevent duplicate/replayed transactions and use a database ledger.
- **Payment verification:** Checkout does not send transactions to a server, verify blockchain payments, or activate memberships. Build chain-specific verification (asset, amount, destination, confirmations, unique transaction) on the server. Independently verify the wallet addresses before publishing.
- **USD redemption:** Points are internal promotional points and have no guaranteed USD value in this starter. Do not promise conversion or withdrawal until there is real funding, published rules, security controls and legal review.
- **Signals:** No live signal engine is included. Connect a tested data/strategy provider and show timestamps/risk information.
- **MT4/MT5:** No orders are placed. Broker integration needs a broker-approved EA/API or secure bridge, test coverage, explicit consent, risk limits and a kill switch.
- **Referrals:** The visible demo code is not a real referral system. Server-side attribution, anti-abuse checks and reward eligibility rules are needed.
- Trading carries risk; never promise profits.
