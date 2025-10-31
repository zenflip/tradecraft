# Kraken Pro order types for take profit strategies

> **Archive Notice**: This document contains Kraken Pro-specific UI instructions. Archived as the main documentation now focuses on platform-agnostic trading concepts. The order types described here (take profit, trailing stop, conditional close) are common across most exchanges but may have different names and interfaces on other platforms.

## Platform-specific considerations: Kraken Pro

On Kraken Pro, you can implement hybrid approaches effectively:

**Use "Take Profit" orders**: Set your first target as a take profit order. This executes automatically when hit.

**Combine with "Trailing Stop"**: Kraken supports trailing stop orders. Set one on your remaining position after first TP hits.

**Or use "Conditional Close"**: Set multiple conditional close orders at different levels (50% at first target, 25% at second target, 25% trailing).

**Manual management option**: Keep some portion without any orders and manage it manually based on price action and support/resistance levels.

## Example Kraken Pro setup

**After entering long at $4,010 with stop at $3,960:**

1. Set take profit order: 50% at $4,110 (2R)
2. Set trailing stop: 50% with $30 trail distance
3. As price moves up, trailing stop moves up automatically
4. First TP captures guaranteed profit, trailing stop locks in gains on remainder

This gives you mechanical protection plus upside participation without needing to watch constantly.

## Context

This section was extracted from the main take-profit-or-not.md guide to keep that document platform-agnostic. The concepts remain valid, but refer to your specific exchange's documentation for equivalent order types and UI workflows.
