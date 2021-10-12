# Advanced Stock Screening

![DBs](https://github.com/escapethegrip/MarketStructure/blob/main/images/double-bottoms.png)

This code is to detect advanced market structure patterns when screening for assets. For more detail about its motivation, see [here](https://escapethegrip.medium.com/revamping-stock-screening-with-precise-code-cc4b034d5ef8 "here").

------------

Virtually single every stock screener you come across online functions in essentially the same manner.

You create an account and choose from a selection of numbers pertaining to:
- ratios like P/E
- fundamentals like Market Cap
- technical indicators like the exponential moving average

This is not enough for me -- I want to be able to fully **customize** what I want my desired asset to *look* like.

## Double Bottom

A double bottom consists of four essential parts.

![DBEs](https://github.com/escapethegrip/MarketStructure/blob/main/images/double-bottom-essentials.png)

Such double bottom (or "W") patterns are spotted by the `advancedDoubleBottom` function.

I'd want to control for my own preferences, for things like:
- the distance/ratio between two legs of a double bottom
- the height/ratio between two legs of a double bottom
- the height/ratio of the breakout price to the mid-point price
- accounting for multiple bottoms, not just two
- accounting for specific candle patterns (i.e bullish hammer)
- double bottom on an upward trending price (trend continuation)
- double bottom on a downward trending price (trend reversal)

Just to name a few.

![DBC](https://github.com/escapethegrip/MarketStructure/blob/main/images/double-bottom-customize.png)


------------


You can see, quickly, how relying on someone else’s screening tool to arbitrarily define such parameters becomes a major limitation.

To have complete control over such parameters and more, I’d have to write my own code.

Plugging this code into a platform like QuantConnect, I can screen for the stocks that look like this:

![dlpn](https://github.com/escapethegrip/MarketStructure/blob/main/images/dlpn.png)
