# Position sizing formula for margin trading (archived)

> **Note**: This document contains Kraken margin-specific position sizing guidance. Due to high margin costs compared to futures, this information is archived for reference but is no longer recommended for active use. See [trading-fees-margin-vs-futures.md](../trading-fees-margin-vs-futures.md) for cost comparison.

## Platform-specific considerations: Kraken Pro

Kraken Pro offers up to 10X margin on many pairs, but you don't have to use all available leverage. In fact, using less than the maximum available leverage is often the prudent choice for most traders.

### Using 3X leverage on a 10X platform

**The question**: If Kraken allows 10X but you want to limit yourself to 3X, how do you calculate position size to risk only 1% of your account?

**The answer**: Use 3X in your position sizing formula, not 10X. The platform's maximum leverage is irrelevant—you choose your actual leverage by your position size.

### Why use less than maximum leverage?

**Breathing room**: A 3X position can handle more volatility than 10X without liquidation.

**Safety margin**: Kraken's 10X maximum doesn't mean it's optimal. Most professional traders use 2X-5X even when 10X+ is available.

**Flexibility**: Lower leverage means you can add to positions or hold through temporary adverse moves without liquidation risk.

**Sleep factor**: A 3X position won't keep you up at night worried about liquidation on normal market swings.

### How Kraken margin works

**Clear example:**

You have a $10,000 account but only want to put $1,000 to work at 3X effective leverage (keeping $9,000 safe):

**Option 1: What most people think (WRONG)**
- "I'll open a $1,000 position (10X platform requires $100 margin)"
- Margin required at 10X: $1,000 / 10 = $100
- Actual leverage: $1,000 / $1,000 allocated = 1X (not 3X!)
- You're using spot leverage, not 3X

**Option 2: What actually works (RIGHT)**
- "I want $1,000 at 3X leverage, so my position should be $1,000 × 3 = $3,000"
- Margin required at 10X: $3,000 / 10 = $300
- Actual leverage: $3,000 / $1,000 allocated = 3X ✓
- This is true 3X leverage on your allocated capital

**Breaking it down:**
- Margin required: $300 (what Kraken takes from your account)
- Position size: $3,000 (what you control in the market)
- Effective leverage: 3X (on your $1,000 allocation)
- Platform leverage: 10X (what Kraken offers)

**The math that matters:**
- Effective Leverage = Position Size / Capital You're Allocating
- NOT: Effective Leverage = Platform Leverage / Some Number

If the price moves 1% against your position:
- Option 1 loss: $1,000 × 1% = $10 (1% of your $1,000 allocation)
- Option 2 loss: $3,000 × 1% = $30 (3% of your $1,000 allocation)

Option 2 gives you the 3X leverage you wanted on your $1,000. Option 1 is just a spot position using no leverage.

**Key insight**: Your $3,000 position only requires $300 margin from Kraken (10X platform), so you're well within your $1,000 allocation. The remaining $700 isn't locked by Kraken—it stays in your account as available buffer for volatility or drawdowns.

**Important note on margin modes**: If using Kraken's cross margin mode (default), your other $9,000 can be used to prevent liquidation on this position. If using isolated margin mode, the $9,000 is truly separated and only your allocated $1,000 (minus the $300 margin) backs this specific position.

### The key insight about margin and leverage

*You don't control effective leverage through margin—you control it through position size relative to your account.* The 10X platform leverage just means you only need to put up 1/10th of the position as collateral. Your actual dollar risk is determined by your position size and how far the price moves—the leverage only affects how much margin you need to hold that position.

Kraken offering 10X doesn't mean you must use 10X. By choosing a smaller position size, you effectively use lower leverage even though the platform allows more.

### Understanding how leverage affects losses

**What really happens:**

When you have a $10,000 position and the price moves 1% against you:
- Your loss = $10,000 × 1% = **$100**

That's it. The loss is based on your **position size**, not your margin.

**The leverage part:**

At 1X (spot): You need $10,000 margin for a $10,000 position
- $100 loss / $10,000 margin = 1% of your margin

At 10X: You need $1,000 margin for a $10,000 position
- $100 loss / $1,000 margin = 10% of your margin

**Key principle**: *The leverage doesn't "multiply" your losses—it just means you're controlling a larger position with less margin.* The same dollar movement becomes a bigger percentage of your margin, but the actual dollar loss is identical.

With 10X leverage, that $100 loss represents:
- 10% of your $1,000 margin
- 1% of your $10,000 account

**This is why position sizing relative to your total account matters more than thinking about margin requirements.**

### Kraken Pro trading fees

Kraken uses a volume-based fee structure with maker/taker fees:

| 30-day volume | Maker fee % | Taker fee % |
| :--- | :--- | :--- |
| $0 USD | 0.25% | 0.40% |
| $10,001 USD | 0.20% | 0.35% |
| $50,001 USD | 0.14% | 0.24% |
| $100,001 USD | 0.12% | 0.22% |
| $250,001 USD | 0.10% | 0.20% |
| $500,001 USD | 0.08% | 0.18% |
| $1,000,001 USD | 0.06% | 0.16% |
| $2,500,001 USD | 0.04% | 0.14% |
| $5,000,001 USD | 0.02% | 0.12% |
| $10,000,001 USD | 0.00% | 0.10% |

**For most traders**: You'll pay 0.25% maker / 0.40% taker fees (lowest tier).

**Maker vs Taker**:
- **Maker**: Limit orders that add liquidity (enter below market for longs, above for shorts)
- **Taker**: Market orders or limit orders that cross the spread (immediate execution)

**Round-trip cost** (entry + exit with taker fees): 0.40% + 0.40% = **0.80% total**

### Accounting for fees in position sizing

The basic formula assumes perfect execution. In reality, fees reduce your effective gains and increase your effective losses.

**Fee impact on a $10,000 position**:
- Entry fee (taker): $10,000 × 0.40% = **$40**
- Exit fee (taker): $10,000 × 0.40% = **$40**
- Total round-trip fees: **$80**

**Adjusting for fees in risk calculation**:

If you want your actual risk to be $150 after fees:
```text
Adjusted Risk = Desired Risk + Expected Fees
Adjusted Risk = $150 + $80 = $230
```

For more conservative sizing, use $230 in your position size formula instead of $150. This ensures after paying fees, your stop loss still represents only 0.5% actual account loss.

**Practical approach**: Most traders don't adjust position size for fees. Instead, they accept that a "1% risk" trade actually risks ~1.2-1.3% after fees on a typical setup. If you're being very precise, add 0.2-0.3% buffer to your risk tolerance.

### Risk management on Kraken

**Set your personal maximum leverage** (e.g., 3X or 5X) and stick to it regardless of what Kraken allows.

**Calculate positions using your limit**: Use 3X in the formula even though 10X is available.

**Monitor your actual leverage**: Check your position size vs. margin used to verify you're at your intended leverage.

**Don't be tempted by higher leverage**: Just because you can use 10X doesn't mean you should. Most blown accounts come from using maximum available leverage.

**Use the buffer**: The gap between your 3X usage and Kraken's 10X maximum gives you safety margin against liquidation during volatile moves.

### Example comparison: 3X vs 10X on same setup

**Same setup, different leverage choices:**
- Account: $10,000
- Risk: 1% ($100)
- Stop: 2% from entry

**Using 3X (disciplined approach)**:
- Position size: $1,667
- Margin required: $556
- Liquidation distance: Much further from entry
- Can handle volatility: Yes

**Using 10X (maximum available)**:
- Position size: $5,000
- Margin required: $500
- Liquidation distance: Very close to entry
- Can handle volatility: No, tight liquidation

**Result**: Both risk $100 if stop is hit, but the 3X position has far more room to breathe and won't get liquidated by normal market noise.
