# Triv's Suspicious Buyer Signal Bot
Detect and see the buys and sells of insiders, market makers, or scammers - use this to help your trading strategy, or trade using this info directly! This bot has a 1 week free trial and my [friendtech](https://www.friend.tech/0x0592eb9664666aa8463fda75de5592101952a7c3) keyholders have unlimited access. Contact me [here](https://t.me/cryptotriv) for free trials or special arrangements.

DISCLAIMER: Not financial advice.

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
  - 🤖 Botted: This token has a history of being suspiciously sniped by the deployer's own addresses.
- 💵 Amount: The amount bought/sold in terms of ETH and USD
- 🧮 Count: Number of times the token has been bought or sold, as well as the number of users subscribed to this token
- 🏷️ Avg Buy Price: The average buy price
- 🔖 Avg Sell Price: The average sell price
- ⚖️ Last 10: The nett flow of buys/sells of the last 10 trades - positive means nett buying, while negative means nett selling
- 📈 Buys: Total ETH spent buying and average ETH spent per buy
- 💧 Buy Liq: Percentage of the total spent ETH and average ETH spent per buy in terms of the liquidity pool
  - EXAMPLE: If the LP has 100 ETH of liquidity, a 1 ETH buy is 1% Buy Liq
- 📉 Sells: Total ETH received selling and average ETH received per sell
- 🩸 Sell Liq: Percentage of the total received ETH and average ETH received per buy in terms of the liquidity pool
  - EXAMPLE: If the LP has 100 ETH of liquidity, a 1 ETH worth of tokens sold is 1% Sell Liq
- 💱 Sell Progress: The percentage of tokens sold based on the total amount of tokens bought
- 🛍️ Holdings: Current holdings in terms of token amount and USD
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
- You can Ctrl+F the token contract address and look at every 10th trade while looking at the "Last 10" data to know if trader has been nett buying or selling. You can do this with Holdings data as well.
- Avoid tokens with red contract scans (🔴), and be careful with orange or yellow contract scans (🟠,🟡)
- Be careful if the trader is in profit - either Sells is greater than Buys, or Current Buy Price is higher than Average Buy Price
- If the trader sold tokens that they never bought, Holdings will show a negative value and Sell Progress will be over 100%!

## Example Trading Strategies
### The Quick Insider (Short Duration, Small Size)
Insiders rushing to buy a token expecting it to pump based on new news or trends - you follow them.

1. Subscribe to New tokens
2. On a New token signal, scan the contract to make sure it is green 🟢
3. Check the token chart to see that you haven't missed any big pump
4. Buy a small amount. OPTIONAL: Check for any new news or emerging trends first for that token
5. If no price movement after some time, sell
6. If it pumps, sell (partially or fully based on discretion) when the insider sells a big chunk
    - TIP: Usually, resistances don't mean much in these setups

See this [example](https://twitter.com/twitter/status/1781591568069394495).
  
### The Slow Insider (Long Duration, Normal Size)
Insiders accumulating a token slowly, expecting it to pump based on news or trends in the future - you follow them.

1. Look for token signals with a Buys amount greater than Sells - this means the insider is accumulating
2. Use Ctrl+F with the token contract address to check the history - usually the frequency of trades is low, maybe once or twice everyday, with gaps in between
3. Check the chart to see if it is near bottom prices and volume is low
4. Scan the contract to make sure it is green 🟢
5. Check fundamentals such as website, socials and group chat activity
6. If favourable, enter a position or start accumulating alongside the insider (e.g. when they buy, you buy)
7. Exit or rotate at some point based on insider activity, profit, or any invalidation

### The Accumulating Market Maker (Mid Duration, Normal Size)
Market makers are nett accumulating at the current price point - you follow them.

1. Look for token signals with a Buys amount greater than Sells - this means the market maker is accumulating
2. Use Ctrl+F with the token contract address to check the history - usually the frequency of trades is high, and check if the market maker is mostly only buying at the current price point
3. Check the chart to see that the price is stagnating
4. Scan the contract to make sure it is green 🟢
5. Check fundamentals such as website, socials and group chat activity
6. If favourable, enter a position or start accumulating
7. Exit or rotate at some point based on market maker activity, profit, or invalidations

### The Mean Reversion (Short Duration, Big Size)
There has been a big dump on the price for whatever reason, yet the market maker is heavily buying at the lows - you follow them.

1. Look for tokens signals where the token experienced a huge dump in price 
2. Use Ctrl+F with the token contract address to check the history - see if the market maker is nett buying at which price.
3. Check the chart to see any correlation in terms of lows and wicks vs the price the market maker is accumulating
4. Scan the contract to make sure it is green 🟢
5. If favourable, enter a position or start accumulating at the lows
6. Exit at some point based on market maker activity, profit, or invalidations

See this [example](https://twitter.com/cryptotriv/status/1781698400167272664).














