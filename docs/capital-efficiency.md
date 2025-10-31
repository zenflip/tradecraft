# Capital efficiency: doing more with less

**Note on cost efficiency:** When using leverage for capital efficiency, futures perpetual swaps are generally cheaper than margin trading due to lower fees. For a detailed cost comparison, see [trading-fees-margin-vs-futures.md](trading-fees-margin-vs-futures.md).

----

**Capital efficiency = how much work your capital does**

It measures how effectively you use your money to get exposure to an asset or trade. You're not changing the risk profile of the trade — you're just using less capital to get the same exposure.

## Example: spot vs leverage

Say you want $10,000 worth of BTC exposure:

| Method | How much you commit | Effective exposure | Capital efficiency |
|:-------|:-------------------|:-------------------|:-------------------|
| **Spot** | $10,000 | $10,000 | 1× |
| **2× leverage** | $5,000 margin + $5,000 borrowed | $10,000 | 2× efficient |
| **3× leverage** | $3,333 margin + $6,667 borrowed | $10,000 | 3× efficient |

**→ You get the same exposure with less of your own money.**

This frees up the rest of your cash for other trades, hedges, or yield — that's capital efficiency.

## Key point

**Capital efficiency ≠ more risk.**

*It's about deploying less capital for the same controlled risk.* If you manage stops and position sizing properly, you're not increasing your probability of ruin — you're increasing the productivity of your capital.

## When it becomes dangerous

Capital efficiency turns from **efficiency → gambling** when:

- You use leverage to **increase position size** instead of reduce capital used
- You skip stop-losses or hedge planning
- You let margin risk dictate your position instead of your plan

## In short

Capital efficiency is the **smart use of leverage to do more with less**, not reckless leverage to risk more than you should.

## Capital efficiency vs leverage: where it breaks down

Here's how capital efficiency scales with leverage, and where it stops being useful and starts getting fragile:

| Leverage | Own capital used | Effective exposure | Capital efficiency | Liquidation buffer | Risk profile | Comment |
|:---------|:----------------|:-------------------|:-------------------|:-------------------|:-------------|:--------|
| **1× (Spot)** | 100% | 1× | 1× | None | 🔵 Safe | Full exposure, no liquidation risk |
| **1.5×** | 67% | 1× | 1.5× | –66% | 🟢 Efficient | Still very safe, mild borrowing |
| **2×** | 50% | 1× | 2× | –50% | 🟢 Optimal | Efficient & robust swing zone |
| **3×** | 33% | 1× | 3× | –33% | 🟠 Tense | Noise can start hurting |
| **5×** | 20% | 1× | 5× | –20% | 🔴 Fragile | Normal daily swings can liquidate |
| **10×** | 10% | 1× | 10× | –10% | 🔴 High risk | Intraday volatility kills position |
| **20×+** | 5% or less | 1× | 20× | –5% or less | ⚫ Suicide | You're trading noise, not structure |

## Key insights

### Capital efficiency peaks around 2–3×

Beyond that, each extra turn of leverage gives you less safety than the marginal gain in efficiency.

**Example:** 2× doubles efficiency with –50% buffer; 5× only adds 2.5× efficiency but slashes buffer to –20%.

### Volatility eats margin nonlinearly

Every extra step of leverage increases the probability of ruin **exponentially, not linearly**.

### Past 3×, you're not efficient — you're fragile

You can't survive ordinary drawdowns. You start needing stops, constant monitoring, and emotional fortitude.

## Related: should you use stops at 2× leverage?

See [Does a stop-loss help?](does-a-stop-loss-help.md) for a detailed discussion on why 2× leverage changes your stop-loss strategy.

**Short answer:** At 2×, you're trading structure, not noise. Your liquidation buffer IS your stop — it's just 50% wide. This is often better than tight stops that get hit by normal volatility.
