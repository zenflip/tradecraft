# Shorting with margin spot trading

**Note on cost efficiency:** While margin spot trading works for shorting, futures perpetual swaps are generally cheaper due to lower fees. For a detailed cost comparison, see [trading-fees-margin-vs-futures.md](trading-fees-margin-vs-futures.md).

----

Can you sell using margin to take a short position like shorting futures?

**Yes — exactly.**

On Kraken Pro, you can short using margin spot trading, and it works almost the same as shorting futures — just under the hood it's different.

## How shorting with margin works

When you click **Sell** while on margin:

1. **Kraken borrows the asset** (e.g., BTC or ETH) from the margin pool
2. **It sells it into USD** for you at current market price
3. **Later, when you close the trade**, Kraken buys back the asset at (hopefully) a lower price and repays the loan

**So you're effectively:**

Borrowing BTC → Selling it → Buying it back lower → Keeping the difference

✅ Works the same way as a futures short in profit/loss terms
🧩 The difference: you're dealing with real borrowed assets, not paper contracts

## Example: shorting BTC with 3× margin

**Scenario:**
- You short BTC at $60,000 using 3× margin
- BTC drops to $54,000 (–10%)
- Your equity rises +30% (3× amplified)

**When you close:**
- Kraken buys back the BTC using USD
- Repays the borrowed BTC
- The leftover USD is your profit

---

## Margin short vs futures short

| Feature | Margin spot short | Futures/perps short |
|:--------|:------------------|:-------------------|
| **Asset borrowed?** | Yes (real BTC/ETH) | No (synthetic contract) |
| **Funding fees** | Interest on borrowed coin | Funding rate between longs & shorts |
| **Liquidation** | When your equity can't cover the borrowed amount | When margin ratio hits limit |
| **Settlement** | Physical (buy/sell coin) | Contract-based |
| **Stop-loss type** | Buy stop-loss | Close stop (or reverse long) |

---

## Simple rule to remember

- **Long on margin:** set a **Sell Stop-Loss**
- **Short on margin:** set a **Buy Stop-Loss**

## The bottom line

You can absolutely short on Kraken Pro using margin spot, and it behaves 90% like shorting futures — just with different mechanics.

**Key advantages:**
- Real asset borrowing (transparent)
- Fixed interest rates (no funding rate volatility)
- Physical settlement (buy/sell actual coins)

**Key consideration:**
- You pay interest on the borrowed asset while the position is open (similar to holding costs)
