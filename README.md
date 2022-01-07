# Commodity-Linked-Products
Best of n/Worst of n Structures

Rainbows are essentially puts and calls written on the best performing (or alternatively, worst performing) asset in a basket of n underlying assets.

* The literature on rainbows focuses on equities: they have the widest participation base, are exchange-traded and the data is easiest to obtain. Much of the general approach for equities can be adapted to FX and commodities. No closed form solution exists for rainbow options of >3 assets. Pricing is determined by Monte Carlo simulation.

* A rainbow option is intuitively more valuable the lower the correlations between underlying assets because of the greater variation in combined asset price paths. If constituent pair-wise correlations are negative and approach -1, the option should be in the money for at least one of the assets.

* Indeed, the pricing of these products is driven by the correlation structure. Correlation risk is time-dependent and difficult to manage: it is not directly observable in the market, cannot be hedged precisely, and relying on historical data is misleading- from one period to the next, pair-wise correlations may vary substantially. Applying multivariate GARCH models, researchers have found the number of required parameters increases rapidly for even moderate dimensionality.

* Practitioners generally use fixed historical correlation estimates and update them periodically.
