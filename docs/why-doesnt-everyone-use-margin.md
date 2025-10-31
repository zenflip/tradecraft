# Why doesn't everyone use margin over futures?

**Note on cost efficiency:** While margin spot trading has many advantages discussed below, futures perpetual swaps are generally cheaper for leveraged trading due to lower fees. For a detailed cost comparison, see [trading-fees-margin-vs-futures.md](trading-fees-margin-vs-futures.md).

---

Margin spot seems cleaner and safer than perpetuals. So why isn't everyone using it?

You're right to notice this. Here's why most people don't use margin — and why smart traders often do.

## Why margin spot is actually great

### 1. You hold the real asset

- You're borrowing BTC or ETH, not a contract
- Easier to understand and transparent
- Not subject to funding rate manipulation

### 2. No funding rate volatility

- Perps have funding every 8 hours that can destroy profit in choppy markets
- Margin has fixed borrowing interest (Kraken's is clear and predictable)
- Funding rates can swing wildly, adding unpredictable costs

### 3. No cascading liquidations

- Futures engines liquidate in milliseconds when price spikes
- Margin gives you more buffer because you hold the asset itself, not a derivative contract
- Less vulnerable to coordinated liquidation hunts

### 4. Better alignment with spot charts

- Price action and indicators are "real"
- Futures often get distorted by liquidation hunts and short squeezes
- What you see is what you get

## So why doesn't everyone use margin spot?

Because of these trade-offs:

| Limitation | Explanation |
|:-----------|:------------|
| **Lower available leverage** | Usually 2×–5× max (vs 100× on futures) |
| **Borrow interest** | You pay hourly/daily interest on borrowed funds, even if price doesn't move |
| **Limited pairs** | Kraken and others only offer margin on top pairs (BTC, ETH, etc.) |
| **Less flashy** | Perps attract gamblers and influencers because of big liquidation moves |
| **Execution slower** | Not as "fast and synthetic" as futures for scalpers or HFT bots |

## Margin vs futures: different tools for different traders

**Margin = "Investor leverage"**
- For people trading real trends, swing setups, or longer-term positions
- Requires patience and structure
- Safer for directional conviction

**Futures/Perps = "Speculator leverage"**
- For people trying to scalp volatility
- High risk of getting wiped out
- Better for short-term tactical plays

## The verdict

If you can manage position sizing (like a 2×–3× buffer approach), **margin spot is the superior way to trade directionally** — safer, cleaner, and far less likely to blow up an account.

## Detailed comparison: margin spot vs perpetual futures

Let's compare a real-world scenario:

**Assumptions:**
- You're long BTC at $100,000
- With $10,000 equity
- Using 3× leverage (≈ $30,000 position)
- BTC moves +10% or –10%

### Feature comparison

| Feature | Margin spot (Kraken) | Perpetual futures (Bybit/BitMEX) |
|:--------|:--------------------|:---------------------------------|
| **Underlying asset** | Real BTC borrowed and held | Synthetic contract only |
| **Leverage** | Usually up to 5×–10× | Up to 100× |
| **Funding cost** | Fixed interest (e.g. 0.02–0.05% per day) | Dynamic funding every 8h (can be 0–1%/day) |
| **P&L if BTC +10%** | +30% gain (3×) | +30% gain (3×) |
| **P&L if BTC –10%** | –30% loss (3×) | –30% loss (3×) |
| **Liquidation buffer** | ~33% drop at 3× (more conservative leverage typical) | ~33% drop at 3×, but users often use 10-50× (5-10% protection) |
| **Stop-loss type** | Sell stop (real coin) | Close stop (synthetic contract) |
| **Interest clock** | Always ticking until repaid | No interest, just funding payments |
| **Execution risk** | Low — actual spot liquidity | High — can slip or wick you out |
| **Market manipulation risk** | Very low | Very high (funding flips, liquidations) |
| **Emotional danger** | Boring, steady | Addictive, high dopamine |
| **Best use case** | Swing or trend trading | Scalping and hedging |
| **Settlement** | Physical (buy/sell BTC) | Virtual (contract P&L only) |

---

## Example outcome: 10% BTC move

| Move | Margin spot (3×) | Perpetual futures (3×) |
|:-----|:-----------------|:-----------------------|
| **+10%** | +$3,000 profit | +$3,000 profit |
| **–10%** | –$3,000 loss | –$3,000 loss |
| **–33%** | Liquidated (3× equity gone) | Liquidated sooner (depends on platform) |
| **+10% then sideways 10 days** | +$3,000 – $30 borrow cost | +$3,000 – $200 funding fees (approx.) |

*Note: The key difference emerges over time. Holding a position for 10 days costs ~$30 with margin but potentially $200+ with perpetuals due to volatile funding rates.*

## Summary

| Verdict | Explanation |
|:--------|:------------|
| **Margin spot = conservative power** | Safer, cleaner, predictable — best for swing trades, and you can hold longer |
| **Perps = casino leverage** | Great for quick tactical plays, but highly vulnerable to liquidation and funding costs |

## The bottom line

If your strategy is a swing trade where you "buy exhaustion, hold until resistance," **margin spot (2×–3×) is absolutely the right tool** — especially when you've got clear structure and risk limits.

You hold the real asset, avoid funding rate roulette, and get more breathing room against liquidation.
