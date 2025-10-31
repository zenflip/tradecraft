# Set stop-loss and take-profit

## Short version

Always set your stop-loss. Take-profit depends on your style — but most traders should pre-plan it.

This document breaks the idea down into why stop-loss matters, when and how to plan take-profits by style, common beginner mistakes, a strong compromise strategy (what experienced traders actually do), and a short BTC example.

## Why you set a stop-loss (non-negotiable)

- Protects you from a single trade blowing up your account.
- Controls risk per trade (e.g., 1% or 2% of capital or equity).
- Removes emotion when things go wrong — you execute a risk plan, not a reaction.

**Stop-loss (SL) is mandatory. If you skip it, you are effectively gambling with undefined downside.**

## Should you set a take-profit (TP)?

Short answer: it depends on your objective and style.

Style -> Best practice

- **Swing / Trend trader**: Don’t hard-cap upside. Use trailing stops and partial profit-taking zones. Let trends run but protect unrealized gains.
- **Scalper**: Set fixed TPs (reward > risk) because trades are short and execution is discrete.
- **System trader**: Define R:R targets in advance (e.g., 1:2, 1:3) and code them into the system.
- **Discretionary trader**: You can manage by eye, but still pre-plan target zones and rules so emotion doesn't rule decisions.

## What most beginners get wrong

- **Take profits too early because fear kicks in.**
- **Let losers run because hope kicks in.**

This psychological inversion is the main killer of small accounts: winners cut short, losers grow.

## Best compromise (what strong traders do)

Use a planned structure + dynamic management. This combines discipline with the ability to capture large trends.

1. Set your stop-loss first (structural invalidation point or ATR-based distance).
2. Define R targets for the setup (1R, 2R, 3R) — calculate these before entry.
3. At +2R → move stop-loss to breakeven (or to a small profit) to remove risk.
4. At +3R → take a partial profit (e.g., sell 25%-50% of position).
5. Let the remainder ride with a trailing stop (ATR-based or structure-based) to capture continuation.

Why this works:

- Protects downside early.
- Locks in gains while leaving room for big moves.
- Removes emotion because trade management steps are pre-planned.

## How to choose R multiples (1R, 2R, 3R, etc.)

The question: **Do you just pick a number you like (e.g., "I always exit at 3R") or base it on chart structure?**

Short answer: **both**, and the best approach depends on whether you prioritize structure or systematic risk/reward targets.

### Structure-first approach (discretionary/professional)

This is what experienced traders do:

1. **Read the chart first** — identify the next logical resistance/support levels, previous swing highs/lows, Fibonacci extensions, or measured moves.
2. **Measure the R multiple** — calculate how many R that structural target represents given your stop distance.
3. **Decide if the R:R is worth it** — if the structure gives you 0.8R or 1.2R, the trade may not be worth taking. If it gives you 2.5R or 4R, that's attractive.

**Example:**
- Entry: $50,000
- Stop: $49,000 (1R = $1,000)
- Next resistance: $53,500 → that's 3.5R
- Decision: "The structure supports a 3.5R target, I'll take it."

**Why this works:** The market doesn't care about your arbitrary 2R or 3R target. It respects structural levels (supply/demand zones, previous breakout points, round numbers). Structure-based targets align with where other traders are likely to act.

### Fixed R multiple approach (systematic/algorithmic)

This is what system traders and beginners often use:

1. **Choose a fixed R target** (e.g., always exit at 2R or 3R) based on backtested expectancy or personal preference.
2. **Place the TP at that multiple** regardless of chart structure.
3. **Accept that sometimes you'll exit early** (before a bigger move) and sometimes you'll miss (price reverses before hitting your target).

**Why this works:** Simplicity and consistency. If your system has positive expectancy at 2R exits across many trades, you don't need to think — you just execute.

### Hybrid approach (best of both worlds)

What strong traders actually do:

1. **Start with structure** — identify 2-3 realistic structural targets.
2. **Map them to R multiples** — see which ones align with good R:R (e.g., 2R, 3R, 5R).
3. **Use partial exits at R milestones** — take 25-30% at 2R, another portion at 3R, trail the rest.
4. **Let structure guide final exits** — if the next major resistance is at 4.8R, don't arbitrarily exit at 5R just because it's a round number.

**Example:**
- Entry: $50,000, Stop: $49,000 (1R = $1,000)
- Structure shows:
  - Minor resistance at $52,000 (2R) → take 30% profit
  - Major resistance at $53,500 (3.5R) → take another 30%
  - Extended target at $55,000 (5R) → trail remainder

**Why this works:** You get the discipline of systematic R-based management combined with the realism of structural price behavior. You're not fighting the chart, and you're not overthinking every tick.

### Quick decision framework

- **If you're systematic/algorithmic**: use fixed R multiples (2R, 3R) and backtest to find what works.
- **If you're discretionary**: read structure first, then calculate R multiples and reject trades with poor R:R.
- **If you want the best of both**: identify structural targets, map them to R, and use partial exits at round R numbers (2R, 3R) with structure-based final targets.

**Bottom line:** Structure tells you where price is likely to stall or reverse. R multiples tell you if the reward justifies the risk. Use both.

## Practical rules and sizing

- **Stop placement**: use a structural invalidation point first (below support / above resistance), or a multiple of execution timeframe ATR (e.g., 1.0–1.5 ATR).
- **Position sizing**: Risk per trade (in $) / (Entry - Stop) = position size (units or contracts).
- **Partial exits**: plan percentages (e.g., 25% at 3R, 25% at 5R) so the remainder can convert into a free-runner.
- **Trailing stop**: ATR(14) × k (k between 1.0 and 3.0 depending on instrument and style) or move stop to last swing low/high on the higher timeframe.

## Example BTC trade (1:3 structure)

- Entry: defined by your setup (e.g., trade window entry or Heikin‑Ashi confirmation).
- Stop: structural invalidation or 1.0 ATR below entry.
- Targets:
  - 1R: first realistic target (e.g., nearest structure or an R-based projection).
  - 2R: secondary target — when price reaches this, move SL to breakeven.
  - 3R: take partial profit (e.g., 30% of position) and trail the rest.

**This is the professional-style approach: define risk first, define reward before emotions get involved, and execute the plan without hesitation.**

## Quick checklist

- [ ] Stop-loss set (location, distance, and sizing calculated).
- [ ] Position size computed from defined risk.
- [ ] R targets planned (1R, 2R, 3R) and partial-exit rules defined.
- [ ] Trailing stop method chosen (ATR or structural).
- [ ] Execution plan (limit vs market, slippage estimate) and fee check.

## Bottom line

- SL: Mandatory.
- TP: Planned in advance, flexible in execution.
- Partial exits + trailing stops give you the best of both worlds: protection and optional continuation.
