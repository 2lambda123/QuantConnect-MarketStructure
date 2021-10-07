# Market Structure

![DBs](https://github.com/escapethegrip/MarketStructure/blob/main/images/double-bottoms.png)

This code is to detect advanced market structure patterns when screening for assets.

Virtually single every stock screener you come across online functions in essentially the same manner.

You input numbers pertaining to ratios like P/E, maybe some fundamentals like Market Cap, maybe some technical indicators like the EMA, and you hope for some promising results.

I want to be able to screen for advanced market structure patterns, like the double bottom, but have the ability to <b>customize</b> the parameters to my liking.

## Double Bottom

A double bottom consists of four essential parts.

![DBEs](https://github.com/escapethegrip/MarketStructure/blob/main/images/double-bottom-essentials.png)

Such double bottom (or "W") patterns are spotted by the `advancedDoubleBottom` function.

I'd want to control for my own preferences, for things like:
- the width of the between two legs of a double bottom
- the ratio of the breakout price to the mid-point price
- multiple bottoms, not just "double"
- specific candle patterns (i.e bullish hammer)
- double bottom on an upward trending price (trend continuation)
- double bottom on a downward trending price (trend reversal)

Just to name a few.

![DBC](https://github.com/escapethegrip/MarketStructure/blob/main/images/double-bottom-customize.png)
