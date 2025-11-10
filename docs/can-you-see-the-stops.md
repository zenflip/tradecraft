# Can you see where the stops are?

You can't see the stop themselves, however you can get pretty close to where a lot of people (including retail) are likely to have stops.

Here's how to think about it.

## 1. You can't see actual stop orders

- Stops are usually hidden on the exchange until triggered
- So there's no public "stop order book"

## 2. But you can see where stops are probably sitting

Traders are predictable. They put stops:
- Just below/above obvious swing highs/lows
- Around round numbers (BTC 70,000, 69,500, etc.)
- Around daily/weekly opens
- Just beyond equal highs/lows/liquidity pools
- Below key support levels (longs) or above key resistance levels (shorts)
- At common Fibonacci retracement levels (50%, 61.8%, etc.)
- Just outside recent consolidation ranges

So if you can see the obvious levels, you can guess a stop pocket.

**Why this matters:** Smart money knows where retail stops cluster. They'll often push price just far enough to trigger those stops, collect the liquidity, then reverse. This is why you see those "fake-out" moves that wick into a level and immediately snap back.

## 3. Tools that infer it

Some platforms map out "liquidity" or "liquidation levels" and that ends up being a proxy for where a bunch of retail/leveraged players will get tagged:

- Hyblock / Laevitas / Coinalyze / Kingfisher / TensorCharts type tools
- They show clusters of liquidations or resting liquidity
- Big cluster above price = likely buy-side liquidity (stops of shorts)
- Big cluster below price = likely sell-side liquidity (stops of longs)

It's inferred, not the raw stop list.

## 4. Perps make it easier

On Binance/Bybit/OKX perps, lots of people use leverage. Leveraged players = tighter, more obvious stops. That's why you get those quick wicks into a level and straight back up/down — it's a stop run/liquidity grab.

**The mechanics:**
- High leverage (10x+) means liquidation points are much closer to entry
- Exchange liquidation engines execute instantly when price hits the level
- This creates cascading liquidations: one liquidation triggers the next
- The result: violent wicks that look like "manipulation" but are really just math

**Stop hunting vs liquidation hunting:**
- Stop hunting: deliberate push to trigger manual stops
- Liquidation hunting: targeting leveraged positions that auto-liquidate
- Both create the same price action, but liquidations are more predictable because they're forced by the exchange

## 5. What you actually see on the book

- You can see limit orders (bid/ask walls) on order book/heatmap (ExoCharts, Bookmap, TensorCharts)
- Stops aren't limit orders, so they won't show
- But a wall just past an obvious stop zone can be a MM waiting to fill when everyone's stops puke

## 6. Liquidation data ≠ stop data

- Liquidations are forced closes of leveraged positions
- Stops are voluntary exits
- They often cluster in similar places, so people use liq maps as a proxy

**Key difference:**
- Liquidations happen at predictable price levels based on leverage
- Stops can be moved, cancelled, or tightened at any time
- Liquidation clusters are more reliable for predicting where liquidity sits

## 7. How to use this information

**Defensive:**
- Don't put stops at obvious levels (just below support, just above resistance)
- Give your stops breathing room beyond the obvious zones
- Consider using mental stops or time-based exits instead of hard stops on obvious levels

**Offensive:**
- Look for setups where price taps obvious liquidity then reverses
- Wait for the stop run to complete before entering
- Enter after the wick, not before it
- Watch for volume spikes at key levels (stops triggering = volume)

**Example trade setup:**
1. Identify obvious equal lows with likely stops sitting below
2. Price drops to sweep those stops (quick wick)
3. Volume spike confirms stops were hit
4. Price immediately reverses back into range
5. Enter long on the reversal with tight stop below the sweep low

This is the classic "liquidity grab" or "stop hunt reversal" pattern.

## 8. Put your limit order where the stops are

This is the "trade into liquidity" approach — place your entry limit order at the exact level where you expect stops to cluster, then let price come to you.

**The logic:**
- Stops create liquidity (forced selling/buying)
- That liquidity creates temporary supply/demand imbalance
- Price often reverses sharply after absorbing the liquidity
- Your limit order gets filled at the best price (the raid level)

**How to execute:**

1. **Identify the liquidity pool:**
   - Equal lows (stops below) or equal highs (stops above)
   - Obvious support/resistance where retail places stops
   - Round numbers with clustered stops

2. **Place your limit order at or just beyond the liquidity:**
   - Buying: set limit slightly below the equal lows
   - Selling: set limit slightly above the equal highs
   - You're positioning to get filled when stops trigger

3. **Let price raid the stops:**
   - Don't chase — wait for price to come to you
   - The wick into your level fills your order
   - If it doesn't hit your level, you don't get filled (that's fine)

4. **Manage the position:**
   - Stop goes beyond the raid (if price keeps going, you're wrong)
   - Target the opposite side of the range or next liquidity pool

**Who teaches this:**

- **ICT (Inner Circle Trader):** Most explicit about "find the liquidity pool, let price raid it, have your limit sitting there at a discount/premium"
- **Tom Dante (Trader Dante):** Talks about stop-runs/liquidity grabs and fading them
- **Al Brooks:** Buy below bars/swing lows where stops get hit (same concept, different language)
- **Wyckoff:** "Buy the shakeout" = price just ran the stops

**The advantage:**
- Better entries: you're buying at the sweep low, not chasing the reversal
- Less emotion: limit order removes FOMO
- You're positioned with smart money, not against them

**The risk:**
- Price might not reverse (you catch a falling knife)
- Requires patience — many setups won't hit your limit
- Need tight risk management if the raid continues through your stop

## Bottom line

You can't see "Bob's stop at 68,742" — but you can see that "a lot of people will get blown out if price trades 0.5–1% below this equal low," and that's usually enough to plan a stop-hunt/liquidity-tap trade.

**The real edge:** Everyone sees the same obvious levels. The question is: are you trading with the crowd (getting stopped out) or trading against the crowd (catching the reversal after the stop run)?

Smart money uses retail's predictability against them. You can too.
