# Margin for noise

**"Margin for noise" means the room your trade has to survive normal market fluctuations — the random, meaningless ups and downs that don't change the overall trend.**

Here's how it works:
- Every market has noise — little 0.5%–2% wicks, stop hunts, and random spikes.
- With low leverage, your liquidation price is far away, so those wicks don't touch you.
- With high leverage, your liquidation price is close, so even a small "noisy" move can wipe you out.

**Example:**
- You open a BTC long at $60,000.
- BTC wiggles ±2% every few hours.
- If you're on 10× leverage, your liquidation might be around $54,000 → a 10% drop kills you.
- But if BTC just dips 5% to $57,000, you're down 50% on margin — you panic or get liquidated.
- If you used 2× leverage, that same dip is only a 10% drawdown, and you can ride it out.

So:
**High leverage shrinks your margin for noise — it makes your position so fragile that normal market wiggles become lethal.**

## Example scenario

- You buy BTC at $60,000
- You use $10,000 of your own money
- You borrow the rest depending on leverage
- Ignore fees/funding

| Leverage | Position Size | Borrowed | Liquidation Price (approx.) | % Drop to Liquidation | Explanation |
|----------|--------------|----------|----------------------------|----------------------|-------------|
| 1× | $10,000 | $0 | No liquidation | – | No debt = no liquidation |
| 2× | $20,000 | $10,000 | $30,000 | −50% | You can lose 50% before margin = 0 |
| 3× | $30,000 | $20,000 | $40,000 | −33% | You can lose 33% before wiped |
| 5× | $50,000 | $40,000 | $48,000 | −20% | 20% move kills you |
| 10× | $100,000 | $90,000 | $54,000 | −10% | 10% move kills you |
| 20× | $200,000 | $190,000 | $57,000 | −5% | 5% move kills you |

At 2× leverage, half the position is your own capital, half is borrowed.
That means price can drop 50% before your equity is gone.

In summary:
2× = 50% buffer
3× = 33% buffer
10× = 10% buffer

**Price distance to liquidation (lower = more fragile)**

```
2× leverage:  |<------------ 50% ------------>|
              $60,000 --------------------> $30,000 (Liquidation)

3× leverage:  |<------- 33% ------->|
              $60,000 -------------> $40,000

5× leverage:  |<---- 20% ---->|
              $60,000 --------> $48,000

10× leverage: |<-- 10% -->|
              $60,000 ----> $54,000

20× leverage: |< 5% >|
              $60,000 -> $57,000
```

Each arrow is your margin for noise — how far price can move against you before liquidation.

See how it collapses as leverage rises?
- 2× gives you breathing room for swings and chop.
- 10× and above is basically scalping territory.
- The higher you go, the more you're betting that nothing random happens before your trade plays out.

## The key insight
**You need enough distance for volatility to pass without destroying your position over time.**

This isn't about surviving one price move, it's about surviving the repeated volatility that occurs during a multi-day or multi-week swing trade. TIme is what makes high leverage so dangerous — each hour gives volatility another chance to kill your position.
