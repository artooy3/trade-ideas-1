# Dan Gershenson's "Box Skate" Around Index Rebalances

This is a niche options strategy that attempts to exploit assignment inefficiencies around index rebalances.

## Background

Many equity indices implement constituent changes after the close. When a stock is added to a major index, passive funds tracking that index must buy shares to match the new benchmark weights. This can create significant buying pressure during the closing auction and immediately afterward.

At the same time, listed equity options face an important operational deadline. While the rebalance may be completed around the close, holders of expiring options generally have only a limited window afterward to submit contrary exercise instructions.

This creates a small but interesting market inefficiency.

## Trade Construction

The trade is typically established using a box spread between strikes K1 and K2.

The position is initially close to delta-neutral and is not primarily intended to express a directional view.

The key is choosing the upper strike, K2, such that it is slightly out-of-the-money prior to the rebalance but has a realistic chance of becoming in-the-money if rebalance-related buying pushes the stock higher.

## The Opportunity

Suppose a newly added index constituent rallies after the rebalance and finishes above K2.

Economically, long holders of the K2 call should exercise.

However, exercise is not automatic in every circumstance. Some market participants may:

* Forget to submit instructions.
* Submit contrary exercise decisions.
* Lack sufficient capital to carry the resulting stock position.
* Be retail traders who simply fail to act within the available window.

As a result, some calls that "should" be exercised may never be exercised.

## Why This Matters

If you are short calls that become in-the-money, you would normally expect assignment.

But if assignment rates are lower than expected, you can occasionally avoid being assigned on contracts that were economically worth exercising.

The result is that a position that began as a largely neutral box spread can unexpectedly acquire long stock exposure.

In effect, the trader receives a chance at upside participation that was not fully priced into the original trade structure.

## Risk / Reality Check

This is not a pure arbitrage.

Most of the time, assignment outcomes will behave as expected and there will be little or no edge.

The trade relies on operational frictions, exercise behavior, and assignment randomness. Those effects can be difficult to forecast and may be inconsistent through time.

For that reason, the strategy is often viewed as more of a specialized "lottery ticket" embedded inside a neutral options structure than a repeatable directional trade.

That said, when the setup aligns with a large index rebalance and a strike sitting near the exercise boundary, the payoff can be surprisingly attractive relative to the capital at risk.

## Intuition

The trade can be summarized as:

"Use a mostly delta-neutral options structure to position for the possibility that rebalance-driven price movement pushes an option through the exercise threshold, then hope assignment frictions allow you to keep upside exposure that the market would normally expect to be neutralized."
