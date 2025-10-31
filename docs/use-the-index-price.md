# Use index price for stop-loss orders

Understanding the difference between last price and index price is crucial for setting effective stop-losses.

## Last price

**This is the most recent trade on the market.**

- It's what you see on the main chart
- Can spike briefly because of low liquidity or a single large order
- Random wicks can trigger your stop even if the broader market hasn't actually moved there

**Problem:** Using "last" for your stop means a temporary wick can trigger it, taking you out of a good trade.

## Index price

**This is a weighted average of major exchanges' prices.**

- Much more stable and reflects the true market value
- Liquidations and margin calls on Kraken use index price
- If your stop-loss is set on index, it'll behave consistently with liquidation logic — fewer fakeouts

**Advantage:** Only a real market move — not a single exchange wick — can trigger your stop.

## Rule of thumb

| Trade type | Price to use | Why |
|:-----------|:-------------|:----|
| **Swing trades** | Index price | Safer and fairer — filters out noise and wicks |
| **Scalps or short-term trades** | Last price (optional) | Tighter precision, but more false hits |

## For swing trading with wide buffers

Since you're running 6H–12H swing trades with wide buffers:

**Use index price for your stop-losses.**

That way, only a real market move — not a single exchange wick — can take you out of your position.

## The bottom line

- **Index price** = stable, consensus market value across exchanges
- **Last price** = single exchange's most recent trade (can be noisy)

For swing trading with margin, **index price is the professional choice** — it aligns with how exchanges calculate liquidations and filters out manipulation.
