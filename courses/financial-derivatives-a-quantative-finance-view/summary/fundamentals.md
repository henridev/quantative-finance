
# fundamentals

## dividends, convenience yields and storage

### stock

say we have a stock priced as $S(t)$, which pays dividends. These didvidens can be measured as dividend yield.
$$
\color{red}{
    y = \frac{\text{dividend per annuum}}{\text{stock prive}}
    }
$$
**dividend yield** can be modelled as continuously compounded yield $y$, which can be interpreted as interest rate.
we can represent the stock in our portfolio like below. given the assumption we reinvest our dividens into the stock holdings.
$$
\color{red}{
    \alpha e^{yt} S(t)
}
$$
$$
\color{red}{
    \alpha e^{yt}
}
$$
> this is structuraly equivalent to the foreign currency. it will be a time dependant allocation of our asset.
this type of modelling is not really done for a single stock. Rather it is done for groups of stocks or indexes. For single stocks lump sum payments can be used to value or portfolio.

### commodities

**convenience yields** can also be modeled as continuously compounded returns.

**storage cost** can also be modeled as continuously compounded costs.

$$
\color{red}{
    \alpha e^{(y-s)t} C(t)
}
$$
---
The two models just discussed are mainly used for pricing future and forward contracts.

## long and short positions

**long** = our portfolios value will rise when the asset value rises.

**short** = our portfolios value will rise when the asset value declines.

example of shorting a stock:

1. investor a borrows stock from other investor b.
2. investor a sells stock at market value
3. investor a is responsible for reimburcing any dividens that would have been earned before maturity
4. at maturity the investor a buys back the stock at market value and returns it to investor b.

### represent short positions in a portfolio

represented with a negative allocation

$$
V(t) = \alpha_{IBM}S_{IBM}(t) - \alpha_{GE}S_{GE}(t) \\

V(t) = 500S_{IBM}(t) - 300S_{GE}(t)
$$

example:

![image](./images/Screenshot%202023-04-29%20182738.png)
![image](./images/Screenshot%202023-04-29%20182803.png)

$$
V(t) = \alpha_{b}S_{b}(t) - \alpha_{a}S_{a}(t) \\

V(t) = 100S_{b}(t) - 80S_{a}(t) + Ne^{r_{d}t} \\

V(t) = (100 * 35) - (80 * 50) + 500 e^{(0.06)t} \\

V(t) = (100 * 70)- (80 * 20) + 500 e^{(0.06)t} \\
$$
$$
\text{needed to buy back shares of a => }(80 * 20)= 1600 \\
\text{current cash value => }500 e^{(0.06)} = 531\\
\text{needed to buy back a => }1600 - 531 = 1069\\
$$
$$
\text{sell stocks of b to buy back shares a => } \frac{1069}{70} \eqsim 16 \\
\text{this will give us cash => } 1120 \\
\text{our total cash will be => } 1120 + 531 = 1651 \\
\text{cash left after share a buyback and return => } 51 \\
\text{cash left after share a buyback and return => } 100-16 = 84 \\
$$
$$
V(t) = 84S_{b}(t) + 51e^{t-1} \\
$$
