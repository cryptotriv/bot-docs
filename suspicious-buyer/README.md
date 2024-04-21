# Triv's Suspicious Buyer Signal Bot
Detect and see the buys and sells of insiders, market makers, or scammers - use this to help your trading strategy, or trade using this info directly!

## How It Works

![image](https://github.com/cryptotriv/bot-docs/assets/101616032/b9f9076f-3c7f-40ea-8b91-d6db476c0db4)

There are two components:
  - Headset ON Picture: A Telegram Channel which continuously streams buys and sells by suspicious traders
  - Headset OFF Picture: A Telegram Bot where you can subscribe to specific tokens that you are monitoring

## How To Read The Data
Here is an example of a suspicious buy flow:

![image](https://github.com/cryptotriv/bot-docs/assets/101616032/4df1c463-6a8e-4a44-99f0-4600a00dfcb3)

- Buy/Sell: The first line can have different emojis alongside the token name and executed price:
  - 💰 Buy: This is the standard emoji for a token buy by the suspicious trader.
  - ✨ New: This is a new token which only has 2 suspicious buys. Useful for early entries.
  - 🌟 Good: This is a token which has 5 suspicious buys. This token is more likely to be continuously bought by the trader.
  - 😈 Sell: This is the standard emoji for a token sell by the suspicious trader.
  - 😡 First Sell: This is the first sell done by the suspicious trader for this token.
- 💵 Amount: The amount bought/sold in terms of ETH and USD
- 🧮 Count: Number of times the token has been bought or sold, as well as the number of users subscribed to this token
- 🏷️ Avg Buy Price: The average buy price
  - TIP: If the current price is above this average buy price, then be careful, as the trader is in profit and may dump on you
- 🔖 Avg Sell Price: The average sell price
- ⚖️ Last 10: The nett flow of buys/sells of the last 10 trades - positive means nett buying, while negative means nett selling
  - TIP: You can Ctrl+F the token contract address and look at every 10th trade while looking at the "Last 10" data to know if trader has been nett buying or selling
- 📈 Buys: Total ETH spent buying and average ETH spent per buy
- 💧 Buy Liq: Percentage of the total spent ETH and average ETH spent per buy in terms of the liquidity pool
  - EXAMPLE: If the LP has 100 ETH of liquidity, a 1 ETH buy is 1% Buy Liq
- 📉 Sells: Total ETH received selling and average ETH received per sell
- 🩸 Sell Liq: Percentage of the total received ETH and average ETH received per buy in terms of the liquidity pool
- 💱 Sell Progress: The percentage of tokens unsold based on the total amount of tokens bought
- 🛍️ Holdings: Current holdings in terms of token amount and USD
  - TIP: You can Ctrl+F the token contract address and look at the Holdings of older trades and newer trades to know if trader has been accumulating or distributing tokens
- 📝 CA: The token's contract address
- 👤 Trader: The trader's address 

## Buttons and Actions

- 📈 Chart: Look at the chart on DexScreener
- 🔍 Scan: Scan the token contract address with the SAFE Analyzer Bot
- 🐱‍👤 Trade: Trade using the Shuriken trading bot
- 🔔 Token: Subscribe to this token specifically (the bot will notify you in private chat)
- 🔔✨ New: Subscribe to new tokens (the bot will notify you in private chat)
- 🔔🌟 Good: Subscribe to good tokens (the bot will notify you in private chat)

## General Tips
- Avoid tokens with red contract scans (🔴), and be careful with orange or yellow contract scans (🟠,🟡)
- Be careful if the trader is in profit - either Sells is greater than Buys, or Current Buy Price is higher than Average Buy Price
- If the trader sold tokens that they never bought, Holdings will show a negative value and Sell Progress will be over 100%!

## Trading Strategies
### The Quick Insider
Insiders

















