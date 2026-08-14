# 🚀 APLO Crypto Terminal

A lightweight, browser-based cryptocurrency portfolio and market analysis terminal built as a single HTML application.

APLO Crypto Terminal is designed to provide a compact, visual and interactive way to monitor cryptocurrency assets, portfolio values, price history, hypothetical scenarios, alerts and market information.

> ⚠️ **IMPORTANT**
>
> APLO Crypto Terminal is an experimental entertainment and educational project.
>
> It is **NOT** a financial service, investment platform, trading platform, financial adviser or investment recommendation system.
>
> Cryptocurrency markets are highly volatile and you can lose some or all of your capital.
>
> Use this terminal entirely at your own risk.

---

## 📌 What is APLO Crypto Terminal?

APLO Crypto Terminal is a self-contained web application designed around a simple idea:

**Put the information you personally want to monitor in one compact crypto terminal.**

The application runs directly in the browser and does not require a traditional backend, database or build system.

The terminal can be hosted as a static website, including through GitHub Pages, or opened locally as an HTML file.

---

# ✨ Main Features

## 💰 Portfolio

The portfolio section displays:

- Total portfolio value
- Individual asset values
- Asset quantities
- Average buy prices
- Current prices
- Profit/loss percentage where applicable
- 1H–6H portfolio performance tracking
- Asset management

Portfolio information is stored locally in the browser.

---

## 🪙 Asset Management

Users can add and remove assets directly from the terminal.

Supported asset types include:

### Binance-style trading symbols

Examples:

- BTCUSDT
- ETHUSDT
- SOLUSDT
- BNBUSDT

### DEX token contract addresses

The terminal can also accept token contract addresses such as:

```text
0x...
```

DEX assets are resolved through available market data from DexScreener.

---

# 📊 Action Menu

The terminal contains five main Action tools.

---

## 1. 📊 Price History

Price History records cryptocurrency prices over time.

The terminal stores approximately one price point per hour.

Historical data is stored locally in the browser and can contain up to approximately one year of hourly data per asset.

### Price History provides:

- Current price
- Average buy price
- Profit/loss percentage
- Historical price points
- Historical price list
- Price chart
- Buy-price reference
- Asset-specific history

The terminal does not invent missing historical points when it was closed.

If the terminal is not running, no artificial historical data is generated for that period.

---

# 🧠 2. ANTS Score

ANTS Score is an internal heuristic indicator created specifically for APLO Crypto Terminal.

It is **not a price prediction**.

The score is calculated from several available signals:

- 24H momentum
- Historical trend
- Current price relative to average buy price
- Amount of historical data available

The current weighting is approximately:

| Component | Weight |
|---|---:|
| 24H Momentum | 35% |
| History Trend | 30% |
| Position vs Average Buy | 20% |
| Historical Data Depth | 15% |

The result is displayed on a:

**0–100 scale**

Current score states include:

- `STRONG`
- `POSITIVE`
- `NEUTRAL`
- `WEAK`
- `HIGH RISK`

### Important

ANTS Score should not be interpreted as:

- a prediction
- a guaranteed signal
- a buy recommendation
- a sell recommendation
- financial advice

It is simply an experimental analytical feature.

---

# 🎯 3. WHAT IF?

WHAT IF? allows the user to experiment with hypothetical investment scenarios.

Example:

```text
Investment: €100
Current price: €0.50
Target price: €2.00
```

The terminal calculates:

- Hypothetical quantity purchased
- Hypothetical final value
- Hypothetical profit/loss
- ROI percentage

The calculation is mathematical and does not account for:

- Trading fees
- Slippage
- Taxes
- Liquidity
- Market impact
- Execution price differences

Therefore, the result is purely hypothetical.

---

# 🔔 4. Price Alerts

Users can create price alerts for tracked assets.

Two alert conditions are available:

```text
ABOVE
BELOW
```

Example:

```text
BTC
ABOVE
€100,000
```

or:

```text
ETH
BELOW
€2,000
```

Alerts are checked whenever the terminal updates its market data.

When an alert condition is reached, the terminal can:

- Mark the alert as triggered
- Display a browser alert
- Attempt device vibration where supported

### Important

Alerts only work while the terminal is running and receiving market updates.

This is **not a server-side notification service**.

Closing the browser or disabling the page may prevent an alert from being checked.

---

# 💎 5. Watchlist / Test

Watchlist / Test allows users to create hypothetical cryptocurrency purchases and follow how they would have performed.

Example:

```text
Asset: AKT
Investment: €100
Baseline price: €1.20
Date: 2026-08-12
```

The terminal then calculates the hypothetical current value and ROI.

This is especially useful for experimental comparisons such as:

> "What would have happened if I had invested €100 in this coin on this date?"

Test positions are stored locally in the browser.

---

# 📈 Asset Distribution

The Asset Distribution dashboard provides an interactive overview of the current portfolio composition.

It includes:

- Total portfolio value
- Number of positions
- Largest position
- Percentage held by each asset
- Visual donut chart
- Individual allocation bars
- Portfolio mix view
- Risk / concentration view
- Diversification indication

The concentration indicator currently classifies the portfolio approximately as:

- `Balanced`
- `Moderate`
- `High`

This is a simple mathematical concentration indicator.

It is **not a professional risk assessment**.

---

# 📰 Crypto News

The terminal provides a Global Crypto News section with links to external cryptocurrency news sources.

These currently include:

- CryptoPanic
- CoinDesk
- Cointelegraph
- Decrypt

The terminal does not create or verify the content published by those external websites.

Users should independently evaluate external information.

---

# 📊 Market Charts

For supported Binance-style assets, the terminal can display a TradingView chart.

Charts are intended for visual market analysis and monitoring.

The terminal does not execute trades directly.

The Binance trading link provided by the terminal takes the user to the external Binance website.

---

# 🌐 Market Data

APLO Crypto Terminal uses external market-data services.

Current integrations include:

### Binance

Used for market prices and 24-hour market changes for supported Binance-style symbols.

### DexScreener

Used for DEX token contract addresses and associated token/pair information.

### TradingView

Used to display market charts for supported Binance assets.

### Important

External services may:

- Change their APIs
- Experience downtime
- Return incomplete data
- Rate-limit requests
- Change market information
- Become temporarily unavailable

APLO Crypto Terminal does not guarantee the availability, correctness or completeness of third-party data.

---

# 🔄 Market Updates

The terminal periodically refreshes market data.

Market data is also used to update:

- Current asset prices
- Portfolio value
- Profit/loss
- Price history
- Portfolio performance
- Price alerts
- Watchlist/test positions
- ANTS Score

The terminal also supports a mobile pull-down gesture for manually refreshing market data.

---

# 🧠 Live Crypto Facts

Below the main terminal interface there is a continuously moving crypto-fact ticker.

It displays educational facts about cryptocurrencies including examples such as:

- Bitcoin
- Ethereum
- Solana
- BNB
- XRP
- Cardano
- Chainlink
- Dogecoin
- Avalanche

The ticker can be paused by interacting with it.

The facts are translated according to the selected terminal language.

---

# 🎨 Themes

APLO Crypto Terminal currently includes **14 visual themes**.

Available themes:

1. Black White
2. White Black
3. Terminal
4. Gold
5. Nando Gray
6. Forest
7. Retro
8. Midnight
9. Ocean
10. Violet
11. Crimson
12. Ice
13. Copper
14. Matrix

The selected theme is saved locally in the browser.

There is intentionally no user-created Custom Theme editor in the current version.

---

# 🌍 Languages

The terminal currently supports:

- 🇬🇧 English
- 🇪🇪 Eesti
- 🇪🇸 Español
- 🇷🇺 Русский

The language selection changes the terminal interface, analytical tools, information panels, legal information and crypto-fact ticker.

The selected language is stored locally in the browser.

---

# 💾 Local Storage

APLO Crypto Terminal is designed to work without a traditional backend.

The browser's `localStorage` is used for locally stored information such as:

- Asset list
- Asset quantities
- Average buy prices
- Token names
- Price history
- Portfolio hourly snapshots
- Selected language
- Selected theme
- Price alerts
- Watchlist/test positions

This means that much of the terminal's personal configuration is stored in the user's browser rather than on a central APLO server.

---

# 🔐 Privacy

APLO Crypto Terminal does not require users to create an account.

There is no built-in user registration system.

There is no built-in password system.

Portfolio information is stored locally in the browser.

However, the terminal communicates with external services to obtain market data and external content.

Users should therefore understand that requests to third-party services may expose information such as the requested asset symbol or token contract address to those services.

Do not enter passwords, private keys, seed phrases or other sensitive credentials into the terminal.

### NEVER enter:

```text
Seed phrases
Private keys
Exchange passwords
Wallet recovery phrases
API secret keys
```

APLO Crypto Terminal does not need any of these.

---

# ⚠️ Limitations

APLO Crypto Terminal is intentionally lightweight and experimental.

It should not be treated as a professional trading terminal.

Potential limitations include:

- Third-party API downtime
- Incorrect or delayed market data
- API rate limits
- Network failures
- Browser limitations
- Local storage deletion
- Device/browser changes
- Missing historical data
- DEX liquidity differences
- Price discrepancies between exchanges
- No guarantee of trade execution
- No tax calculations
- No fee calculations
- No slippage calculations
- No guaranteed alerts when the browser is closed

---

# 🛡️ Security Notice

Never use this application to store or transmit cryptocurrency credentials.

The terminal does not need access to:

- Private keys
- Seed phrases
- Wallet passwords
- Exchange passwords

If somebody asks you to enter a seed phrase or private key into APLO Crypto Terminal, **do not do it**.

---

# 💡 Example Use Cases

APLO Crypto Terminal can be used for:

### Portfolio monitoring

```text
How much is my crypto portfolio worth right now?
```

### Historical tracking

```text
How has this asset moved since I started tracking it?
```

### Hypothetical investing

```text
What would €100 invested at this price be worth at my target?
```

### Experimental comparisons

```text
Which of my watchlist coins would have performed best since August 12, 2026?
```

### Portfolio concentration

```text
How concentrated is my current portfolio?
```

### Personal research

```text
Which assets currently show stronger or weaker heuristic signals?
```

---

# 🚫 What APLO Crypto Terminal Is NOT

APLO Crypto Terminal is NOT:

- A cryptocurrency exchange
- A brokerage
- A wallet
- A custody service
- A payment service
- A financial adviser
- An investment adviser
- A trading bot
- An automated trading system
- A guaranteed price prediction system
- A professional risk-management platform
- A tax calculator
- A source of guaranteed financial information

No trade is executed by APLO Crypto Terminal.

---

# 🧮 Calculations

The terminal performs calculations locally in the browser.

Examples include:

### Portfolio value

```text
Quantity × Current Price
```

### Profit/Loss

```text
(Current Price - Average Buy Price) / Average Buy Price × 100
```

### WHAT IF?

```text
Hypothetical Quantity = Investment / Current Price

Hypothetical Final Value =
Hypothetical Quantity × Target Price

Profit =
Final Value - Investment

ROI =
Profit / Investment × 100
```

These calculations are mathematical estimates and may differ from real-world trading results.

---

# 🏗️ Technical Structure

APLO Crypto Terminal is intentionally simple.

The current application is primarily contained in a single HTML file with:

- HTML
- CSS
- JavaScript
- Browser local storage
- External market-data APIs
- External chart widgets

No traditional package installation is required.

No Node.js environment is required to run the basic terminal.

No database is required.

No server-side application is required for the core functionality.

---

# 🚀 Running the Terminal

## Option 1 — GitHub Pages

The simplest way to publish the terminal is through GitHub Pages.

1. Create or use a GitHub repository.
2. Upload the terminal HTML file.
3. Make sure the main page is named:

```text
index.html
```

4. Enable GitHub Pages.
5. Open the generated GitHub Pages website.

The terminal requires an internet connection for external market data and external services.

---

## Option 2 — Run Locally

Download the HTML file and open it in a modern browser.

For example:

```text
index.html
```

Open the file using:

- Chrome
- Edge
- Firefox
- Safari
- another modern browser

Internet access is required for live market data.

---

# 📱 Mobile Support

The interface is designed with mobile use in mind.

The terminal uses:

- Responsive layout
- Touch interaction
- Mobile-friendly modals
- Swipe/pull refresh support
- Compact information cards
- Touch-friendly controls

It can also be used on desktop browsers.

---

# 🔬 Project Philosophy

APLO Crypto Terminal is not intended to compete with professional trading platforms.

The project is built around experimentation.

The goal is to create a personal crypto dashboard that combines:

```text
Market Data
      +
Portfolio Tracking
      +
Historical Data
      +
Simple Analytics
      +
Hypothetical Scenarios
      +
Alerts
      +
Visualisation
      +
Experimentation
```

The project may evolve over time.

Features, calculations, APIs, themes and interface elements may change between versions.

---

# 🧪 Experimental Nature

This project is intentionally experimental.

Some features are heuristic rather than scientific.

In particular:

> **ANTS Score is an experimental heuristic indicator and should never be interpreted as a prediction of future cryptocurrency prices.**

The same applies to portfolio concentration indicators and hypothetical investment calculations.

They are tools for exploration and visualization.

---

# 📚 Data and Information Disclaimer

Market prices and other data shown by the terminal may come from third-party services.

Data can be:

- Delayed
- Incomplete
- Incorrect
- Temporarily unavailable
- Different between exchanges
- Different from the price available to an individual user

Always verify important information directly with the relevant exchange, blockchain explorer, project documentation or other authoritative source before making decisions.

---

# ⚖️ Legal & Responsibility Disclaimer

APLO Crypto Terminal is provided strictly for entertainment and educational purposes.

The creator of APLO Crypto Terminal accepts no responsibility or liability for:

- Financial losses
- Trading losses
- Investment losses
- Missed opportunities
- Incorrect decisions
- Incorrect calculations
- Incorrect market data
- API failures
- Service outages
- Lost local browser data
- Losses caused by third-party websites
- Losses caused by third-party APIs
- Any other direct or indirect consequence resulting from the use of this application

Nothing in APLO Crypto Terminal constitutes:

- Financial advice
- Investment advice
- Trading advice
- Legal advice
- Tax advice

You are solely responsible for your own decisions.

Always perform your own research and independently verify important information.

By using APLO Crypto Terminal, you acknowledge that you understand and accept these limitations.

---

# 🤝 Contributions

Suggestions, bug reports and improvements are welcome.

If you find a problem:

1. Check whether it has already been reported.
2. Open an issue with a clear description.
3. Include steps to reproduce the problem where possible.
4. Include screenshots when useful.
5. Describe your browser/device if the problem appears platform-specific.

Please do not publish:

- Private keys
- Seed phrases
- Passwords
- API secrets
- Personal financial information

in issues or pull requests.

---

# 🐛 Bug Reports

Useful bug reports should include:

```text
Browser:
Device:
Operating system:
Terminal version:
Selected theme:
Selected language:
Asset involved:
Steps to reproduce:
Expected result:
Actual result:
Screenshot:
```

---

# 📈 Project Status

**Status: Experimental / Active Development**

APLO Crypto Terminal is a personal experimental project and may continue to change.

There is no guarantee that:

- APIs will remain unchanged
- External services will remain available
- Historical data will always be preserved
- Features will remain identical
- Future versions will be backwards compatible

---

# ❤️ About the Project

APLO Crypto Terminal was created as an experimental personal crypto-monitoring project.

The idea is simple:

> **Build a crypto terminal that is useful, visual, customizable and fun to use — without pretending to be a professional financial system.**

If you find the project useful, interesting or entertaining, feel free to explore the code and experiment with it.

---

# 📌 Quick Feature Overview

| Feature | Available |
|---|:---:|
| Portfolio tracking | ✅ |
| Asset management | ✅ |
| Average buy price | ✅ |
| Profit/Loss | ✅ |
| Price history | ✅ |
| Historical chart | ✅ |
| 1H–6H portfolio performance | ✅ |
| ANTS Score | ✅ |
| WHAT IF calculator | ✅ |
| Price alerts | ✅ |
| Watchlist / Test positions | ✅ |
| Interactive asset distribution | ✅ |
| Concentration indicator | ✅ |
| Crypto fact ticker | ✅ |
| External crypto news | ✅ |
| TradingView charts | ✅ |
| Binance market data | ✅ |
| DexScreener DEX data | ✅ |
| Multiple themes | ✅ |
| 14 themes | ✅ |
| English | ✅ |
| Eesti | ✅ |
| Español | ✅ |
| Русский | ✅ |
| Local browser storage | ✅ |
| User accounts | ❌ |
| Built-in wallet | ❌ |
| Private key storage | ❌ |
| Direct trading | ❌ |
| Guaranteed price prediction | ❌ |
| Server-side alerts | ❌ |

---

# 📜 License

Please see the repository for the applicable license and usage terms.

If no explicit license has been added to the repository, do not assume that the code is automatically free to copy, modify or redistribute.

---

## ⚠️ Final Reminder

**APLO Crypto Terminal is an experimental entertainment and educational project.**

**It is not financial advice.**

**It does not guarantee market data accuracy.**

**It does not guarantee alerts.**

**It does not execute trades.**

**It does not store private keys or seed phrases.**

**Use it at your own risk.**
