# Stop-loss orders on margin: sell stop vs sell limit

If I'm using margin, should I use a sell stop-loss or sell limit order?


## Use a sell stop-loss order, not a sell limit

### 1. Stop-loss (sell stop)

- **Triggers only** when price falls to your chosen level (e.g., $3,839)
- **Once triggered**, it becomes a market order (or stop-market), instantly selling your ETH to close the long
- **Protects you automatically** if price dumps fast

That's exactly what you want when you're long on margin — you're holding borrowed exposure, so you need a stop that fires automatically when price falls.

**✅ Correct use:**

"Close ETH/USD (10x)" with stop-loss at $3,839
→ Triggers a market sell once ETH hits $3,839


### 2. Sell limit

- **Executes only** if price rises to your target
- **Used for taking profit**, not protection
- A sell limit above current price closes your long in profit
- A sell limit below current price will fill instantly, closing your trade right now

That's why if you accidentally use sell limit instead of sell stop, it'll either execute immediately or not protect you at all.


## For your margin long

- **To protect downside:** use sell stop-loss (stop-market)
- **To take profit:** use sell limit

**You can use both at once** — Kraken lets you bracket your position:
- Stop at $3,839
- Limit take-profit at, say, $4,250


## Margin spot vs futures: different stop types

Because you're holding spot with margin, you need to sell a stop-loss order — this is different from using futures.

### When you're using margin spot trading

You're **borrowing funds to buy the underlying asset** (like ETH or BTC). So you're literally holding the asset — not a contract.

That means to exit or protect the position, you must **sell the actual asset**. That's why your stop must be a **sell stop-loss order**.

**Example:**
- You're long ETH (borrowed or leveraged spot)
- If price drops to your stop, you sell ETH back into USD — repaying the borrowed margin

**✅ Correct type:** Sell stop-market (stop-loss) — triggers when price falls to your chosen level


### When you're using futures or perpetuals

You're trading **contracts, not the asset**. Your stop is then a **close stop** on the contract itself. You don't "sell" your ETH — you close a long contract with an opposite short.

**Summary:**
- In futures: it's "close position stop"
- In margin spot: it's "sell stop order"

---

## Key takeaway

| Type | What you hold | Stop type you need | What it does |
|:-----|:--------------|:------------------|:-------------|
| **Margin spot (Kraken Pro)** | Borrowed BTC/ETH | Sell stop-loss | Sells your coins to repay loan |
| **Futures/perpetuals** | Contract | Close stop order | Offsets position instantly |


## The bottom line

Because you're on margin spot, you need to use **sell stop-loss** (not futures-style close order).
