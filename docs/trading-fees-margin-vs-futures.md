# Trading fees: margin vs futures

## The hidden cost killer

Trading fees are the silent killer of trading accounts. You can have perfect entries, tight stops, and hit your targets — but if you're using the wrong instrument, fees will eat 50-80% of your profits before you even notice.

**The core insight: Futures are almost always cheaper than margin trading, especially for swing trades lasting more than a day. For scalp trades (minutes to hours), the difference is smaller but futures still win due to lower maker/taker fees — you just avoid most holding costs since you close before funding or rollover charges.**

## Quick comparison

**Margin trading:**
- You borrow the asset (USD or BTC)
- You pay rollover/interest every 4-8 hours
- Higher maker/taker fees on most exchanges
- Costs stack up badly on multi-day holds

**Futures trading:**
- You don't borrow anything
- No interest — only funding between longs & shorts
- Much lower maker/taker fees
- Funding can flip against you but usually small

## Kraken: margin vs futures breakdown

### Kraken margin costs

**Trading fees**:

Starter tier ($0-100k volume):
- Maker: 0.25%
- Taker: 0.40%
- Round-trip: 0.80% (entry + exit)

High-volume tier ($1M+ volume):
- Maker: 0.06%
- Taker: 0.16%
- Round-trip: 0.22% (entry + exit)

**Rollover fees** (both tiers):
- 0.02% every 4 hours (example rate — actual rates are dynamic and vary by currency pair)
- 0.12% per day
- 0.84% per week

**Note**: Kraken uses dynamic margin fees that fluctuate based on market conditions. The rate is locked in when you open your position and displayed in the order form.

Using 0.02% as an average is sensible for illustrative purposes, especially since most traders do both long and short positions over time — it provides a realistic middle-ground estimate rather than cherry-picking the lowest or highest rate.

**Total cost for 3-day swing trade**:

Starter tier:
- Trading fees: 0.80%
- Rollover: 0.36% (3 days × 0.12%)
- **Total: 1.16%**

High-volume tier:
- Trading fees: 0.22%
- Rollover: 0.36% (3 days × 0.12%)
- **Total: 0.58%**

### Kraken futures costs

**Trading fees**:
- Maker: 0.02%
- Taker: 0.05%
- Round-trip: 0.10% (entry + exit)

**Funding rate**:
- Typically 0.01% every 8 hours
- Only charged if you're on crowded side
- 0.03% per day (if charged)

**Total cost for 3-day swing trade**:
- Trading fees: 0.10%
- Funding: ~0.09% (3 days × 0.03%, if charged)
- **Total: ~0.19%**

### The damage: real numbers

**Example: $10,000 BTC position, 3-day hold**

| Cost | Kraken Margin (starter) | Kraken Margin (high-volume) | Kraken Futures | You Save (starter) | You Save (high-volume) |
|------|-------------------------|------------------------------|----------------|--------------------|-----------------------|
| Entry fee | $40 | $16 | $5 | $35 | $11 |
| Exit fee | $40 | $16 | $5 | $35 | $11 |
| Rollover/Funding | $36 | $36 | $9 | $27 | $27 |
| **Total** | **$116** | **$68** | **$19** | **$97** | **$49** |

**Example: $50,000 BTC position, 3-day hold (3X margin)**

| Cost | Kraken Margin (starter) | Kraken Margin (high-volume) | Kraken Futures | You Save (starter) | You Save (high-volume) |
|------|-------------------------|------------------------------|----------------|--------------------|-----------------------|
| Entry fee | $200 | $80 | $25 | $175 | $55 |
| Exit fee | $200 | $80 | $25 | $175 | $55 |
| Rollover/Funding | $180 | $180 | $45 | $135 | $135 |
| **Total** | **$580** | **$340** | **$95** | **$485** | **$245** |

**You're losing $49-97 per trade ($10k) or $245-485 per trade ($50k) by using margin instead of futures.**

Even with high-volume discounts, margin still costs 3× more than futures.

Over 20 trades at $50k: **$4,900-9,700 in unnecessary costs.**

## When to use each

### Use futures when:

✅ Swing trading (2+ day holds)
✅ Trade window setups (6H/15m style)
✅ Scalp trading and intraday trading
✅ You want lower fees
✅ You understand liquidation risk
✅ You're comfortable with perpetual contracts

### Use margin when:

⚠️ You need to borrow actual asset (rare use case)
⚠️ Your exchange doesn't offer futures
⚠️ You're uncomfortable with perpetual contracts

**Reality**: For most traders doing 1-5 day holds, futures are dramatically cheaper.

## Understanding funding rates

Funding rates are how futures markets stay balanced. When too many traders are long, longs pay shorts. When too many are short, shorts pay longs.

**Typical funding rate**: 0.01% every 8 hours

**How it works**:
- If rate is positive: longs pay shorts
- If rate is negative: shorts pay longs
- Only charged if you hold through funding time (every 8 hours)

**Checking funding rates**:
- Kraken Futures: shown on each contract page
- Usually between -0.05% to +0.05% per 8 hours
- Extreme: can spike to ±0.1% during mania/panic

**Pro tip**: If funding is heavily negative and you're long, you get paid to hold. If it's heavily positive and you're long, you pay — but it's still usually cheaper than margin rollover.

## Fee impact on your strategy

### Trade window approach (6H/15m)

**Typical hold time**: hours to 4 days

**Margin cost on $10k position**:
- Fees: $80
- Rollover: $24-48
- **Total: $104-128 (1.04-1.28%)**

**Futures cost on $10k position**:
- Fees: $10
- Funding: $6-12
- **Total: $16-22 (0.16-0.22%)**

**Result**: You need 1% less price movement to break even on futures. On a 3% winner, margin takes 35% of your profit in fees. Futures takes only 7%.

## Calculating total trade cost

### The formula

```
Total Cost = Entry Fee + Exit Fee + Holding Costs
```

**Margin holding cost**:
```
Holding Cost = Position Size × 0.02% × (Hours Held / 4)
```

**Futures holding cost**:
```
Holding Cost = Position Size × Funding Rate × (Hours Held / 8)
```

### Example calculation

**$10,000 position, 72 hours (3 days)**

**Margin**:
- Entry: $10,000 × 0.40% = $40
- Exit: $10,000 × 0.40% = $40
- Holding: $10,000 × 0.02% × 18 = $36
- **Total: $116**

**Futures**:
- Entry: $10,000 × 0.05% = $5
- Exit: $10,000 × 0.05% = $5
- Holding: $10,000 × 0.01% × 9 = $9
- **Total: $19**

## Fee minimization strategies

### 1. Use maker orders when possible

**Maker vs taker** on Kraken Futures:
- Maker (limit orders that add liquidity): 0.02%
- Taker (market orders or crossing spread): 0.05%

**Savings**: Using maker orders saves 0.03% per side = 0.06% round-trip

On $10k position: **$6 saved per trade**

### 2. Close before funding times

Funding on Kraken Futures occurs every 8 hours (00:00, 08:00, 16:00 UTC).

**Strategy**: If you're on the paying side and planning to exit soon anyway, close 1-2 minutes before funding time to avoid the charge.

**Savings**: 0.01-0.03% per funding period avoided

### 3. Trade higher volumes for fee discounts

Kraken's fee tiers improve with 30-day volume. As you trade more, fees decrease.

| 30-day volume | Futures Taker | Futures Maker |
|---------------|---------------|---------------|
| $0-$100k | 0.05% | 0.02% |
| $100k-$1M | 0.04% | 0.015% |
| $1M-$10M | 0.035% | 0.01% |
| $10M+ | 0.03% | 0.00% |

**Pro traders at $1M+ volume**: Pay 0.035% taker, 0.01% maker (vs 0.05%/0.02% starting tier)

### 4. Account for fees in position sizing

Don't ignore fees when calculating risk/reward.

**Example without fees**:
- Entry: $50,000
- Target: $51,500 (3% gain)
- Stop: $49,500 (1% loss)
- R:R = 3:1

**Example with fees** ($50k position, futures):
- Entry fee: $25
- Exit fee: $25
- Holding cost: $50
- Total fees: $100 (0.2% of position)

**Adjusted returns**:
- Winner: 3% - 0.2% = 2.8% net
- Loser: 1% + 0.2% = 1.2% net
- R:R = 2.8:1.2 = 2.3:1 (not 3:1)

**Lesson**: Always calculate R:R after fees, not before.

### 5. Reduce trade frequency on choppy days

Every time you enter and exit, you pay fees. If you're getting chopped out repeatedly:

**5 failed entries on margin**:
- 5 × $80 (round-trip fees) = **$400 lost to fees**
- Before you factor in stop losses

**Solution**: Trade less frequently. Wait for clearer setups. Use the trade window framework to avoid chop.

## Platform comparison

### Quick reference table

| Exchange | Type | Maker | Taker | Funding/Rollover | 3-Day Cost ($10k) | 3-Day Cost ($50k) |
|----------|------|-------|-------|------------------|-------------------|-------------------|
| Kraken Margin (starter) | Margin | 0.25% | 0.40% | 0.12%/day | $116 | $580 |
| Kraken Margin (high-volume) | Margin | 0.06% | 0.16% | 0.12%/day | $68 | $340 |
| Kraken Futures | Futures | 0.02% | 0.05% | ~0.01%/8h | $19 | $95 |
| BitMEX Futures | Futures | 0.05% | 0.05% | ~0.01%/8h | $19 | $95 |
| Bybit Futures | Futures | 0.02% | 0.055% | ~0.01%/8h | $20 | $100 |

**Key insight**: Even with high-volume discounts (0.06% maker / 0.16% taker), margin trading costs 3× more than futures for multi-day holds. On a $50k position, you're losing **$245-485 per trade** by using margin instead of futures.

### Kraken (what we've covered)

**Margin**:
- Fees (starter): 0.25%/0.40%
- Fees (high-volume): 0.06%/0.16%
- Rollover: 0.02% per 4h
- Max leverage: 5X

**Futures**:
- Fees: 0.02%/0.05%
- Funding: ~0.01% per 8h
- Max leverage: 50X

**Note**: High-volume tier applies at $1M+ 30-day trading volume. Even with this discount, futures still cost 3× less due to rollover fees.

### Binance

**Margin**:
- Fees: 0.10%/0.10%
- Interest: ~0.02% per day
- Max leverage: 10X

**Futures**:
- Fees: 0.02%/0.04%
- Funding: ~0.01% per 8h
- Max leverage: 125X

### Bybit

**Spot Margin**:
- Fees: 0.10%/0.10%
- Interest: ~0.02% per day

**Futures**:
- Fees: 0.02%/0.055%
- Funding: ~0.01% per 8h
- Max leverage: 100X

**Total cost for 3-day swing trade** (futures):
- Trading fees: 0.075% (entry + exit)
- Funding: ~0.09% (3 days × 0.03%)
- **Total: ~0.165%** ($17 on $10k position)

**Notable**: Bybit has competitive futures fees (0.02% maker is tied with Kraken for lowest), but taker is slightly higher at 0.055% vs Kraken's 0.05%. Overall costs are nearly identical to Kraken and BitMEX futures.

**Pattern**: Futures are cheaper across all major exchanges for swing trading.

### BitMEX

**Perpetual futures**:
- Maker: 0.05%
- Taker: 0.05%
- Funding: ~0.01% per 8h

**Total cost for 3-day swing trade**:
- Trading fees: 0.10% (entry + exit)
- Funding: ~0.09% (3 days × 0.03%)
- **Total: ~0.19%**

**BTCUSDT and ETHUSDT**: Same fees (0.05%/0.05%), both are linear perpetual contracts settled in USDT.

**Notable**: BitMEX charges the same maker/taker fee (0.05%), unlike most exchanges where maker is lower. This means you don't benefit from using limit orders vs market orders on BitMEX. Costs are similar to Kraken Futures.

## Common mistakes and fixes

### Mistake 1: "I'm only holding 2 days, fees don't matter"

**Reality**: On a $10k position, 2 days on margin costs $104. On futures: $16. That's a **$88 difference** — nearly 1% of your position.

**Fix**: Switch to futures for any hold over 4 hours.

### Mistake 2: "Market orders are faster, the 0.03% extra doesn't matter"

**Reality**: 0.03% on $10k = $3. Do this 50 times = **$150 lost** to impatience.

**Fix**: Use limit orders. Place them slightly inside the spread. You'll get filled quickly and save 0.03% per side.

### Mistake 3: "I'll trade through funding, it's only $10"

**Reality**: If you're on the wrong side of funding and it happens 3× per day for a week, that's **21 funding charges** = $210.

**Fix**: If funding is heavily against you, close before funding times or flip to the other side.

### Mistake 4: Ignoring fees when calculating win rate

**Example**: You think you won 60% of trades, but after fees:
- 60% winners: average 2% gain - 0.2% fees = 1.8% net
- 40% losers: average 1% loss + 0.2% fees = 1.2% net

**Reality**: Your expectancy is lower than you think because you're not accounting for 0.2% friction on every trade.

**Fix**: Track net return after fees, not gross price moves.

### Mistake 5: Trading on margin because "that's what I started with"

**Reality**: You're losing $100+ per trade out of habit.

**Fix**: Migrate to futures. It takes 30 minutes to learn the interface. You'll make that time back in 1-2 trades through saved fees.

## How to switch from margin to futures

### Step 1: Open futures account

On Kraken:
1. Log into Kraken
2. Navigate to "Futures" section
3. Enable futures trading (requires verification)
4. Transfer funds from spot to futures wallet

**Important**: Futures and margin are separate wallets. You'll need to transfer capital.

### Step 2: Learn the interface

**Key differences**:
- Perpetual contracts (no expiry)
- Mark price vs last price (liquidation uses mark)
- Funding times shown (every 8 hours)
- Leverage slider (use 3-5X, not maximum)

**Practice**: Place a small position ($100) and hold for a day. Watch funding charges. Get comfortable with interface.

### Step 3: Execute same strategy

Your trade window approach (6H/15m) works identically on futures:
- Same entry rules
- Same stop loss placement
- Same target calculation
- Just way lower fees

### Step 4: Monitor total costs

Track your fees for 10 trades on futures vs what you paid on margin.

**You'll see**: Savings of $50-100 per trade add up to $500-1000 over 10 trades.

## The bottom line

**For a typical 3-day trade:**
- Margin costs 0.58-1.16% per trade (high-volume to starter tier)
- Futures costs ~0.19% per trade
- **You save 0.39-0.97% per trade**

**Per-trade savings:**
- $10k position: $49-97 saved per trade
- $50k position: $245-485 saved per trade

**The math is simple**: Use futures for swing trades. Use margin only if you have a specific reason. Default to the cheaper option and keep more of your gains.
