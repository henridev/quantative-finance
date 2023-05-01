# Arbitrage

The rough idea:

- a riskless profit.
- investment oportunity in which have a chance of making a profit and no chance of losing money.

Mathematical definition:

- portfolio with value $V(t)$
- satisfying $V(0) \leq 0$
  - you can enter in to the portfolio without spending money
  - this means there is no possiblity to lose money from $T$ onwards
- and for some time $T > 0$ in the future
- $\color{red}{Prob(V(T)< 0) = 0\text{ and } Prob(V(T) > 0) > 0}$
  - from $T$ there will definitly be profit

> a portfolio can be entered into at no cost and it will yield a certain and positive profit at some time $t>0$

How to apply arbitrage:

- principle: arbitrage cannot exist
- if we make assumptions and those assumptions imply that an arbitrage portfolio exists we can rule out those assumptions (contradiction)

arbitrage for pricing:

1. assume two assets do not have the same price
2. show that that assumption allows for the construction of an arbitrage portfolio
3. conclude that 2 assets have the same price because we said arbitrage does not exist

## example of arbitrage

### example 1

![example](../images/Screenshot%202023-04-30%20164202.png)
![values](../images/Screenshot%202023-04-30%20164319.png)

if we add row one of the table to two times the second row we will end up with the third row.

$P_{a}(1) + 2P_{b}(1) = P_{c}(1)$

if we use this relationship at $t=0$

$P_{a}(0) + 2P_{b}(0) =25 + (20 * 2)$

$P_{a}(0) + 2P_{b}(0) =65$

$65 < 80$

this shows that stock c is overpriced at $t=0$

procedure to construct an arbitrage when you suspect 2 assets ate mispriced relative to eachother.

> long the underpriced asset and short the overpriced asset.

here this becomes:

- long assets a and b
- short asset c

at time $t=0$ we will enter in the following portfolio

cost of entering in long position.

$P_a(0)+2P_b(0) = 25 + 2 * 20 = 65\$$

cash received from short position.

$P_c(0) = 80$$

the cash received will cover the long positions. Next to that there is still 15$ left than can be invested in the risk free rate

$V(0) = + 15e^{r_{d}t}$

holding the positions until t=1 we know certainly that the following relation will hold.

$P_{a}(1) + 2P_{b}(1) = P_{c}(1)$

we will need to sell because one share of c needs to be returned to the owner. We do this by selling shares a and b

$P_{a}(1) + 2P_{b}(1) = P_{c}(1)$

this will make us able to close out the short and long position.

> in the end we still have the $\color{green}{\$15}$ profit realized at $t=0$

this portfolio was riskless and we did not spend anything to enter in it.

Therefore this is an arbitrage portfolio.

### example 2

![example](../images/Screenshot%202023-05-01%20090450.png)

$FairValue = \frac{600}{(1+0.0-75)} + \frac{600}{(1+0.015)^{2}} + \frac{10600}{(1+0.02)^{3}} = \$11166.55$

so this bond is underpriced. Arbitrage will involve taking a long position in the bond.

$\frac{600}{(1+0.0-75)} = 595.53$

$\frac{600}{(1+0.015)^{2}} = 583.40$

$\frac{10600}{(1+0.02)^{3}} = 9988.62$

we can borrow these amounts of money and set their corresponding debt payments equal to the coupon payments. this way the bond payments will finance the debt.

> this can be seen as equivalent to selling 3 zero coupon bonds with the bond paymenrs as the par values.

This means we will borrow 595.53 over 1y, 583.40 over 2 y, 9988.62 over 3y.

thsi will mean in our portfolio $595.53 + 583.40 + 9988.62 = \$11166.55$ cash. $\$ 10000$ of it will be used to buy our bond. This holding will be invested at risk free rate.

<span style="color:red;">
This portfolio does not require any entry costs
</span>

</br>

$V(t)= 11166.55 + 595.53 - 583.40 - 9988.62 +(1166.55 * (1.02)^{3})$

$V(t)= (1166.55 * (1.02)^{3})$

value of cash = $(1166.55 * (1.02)^{3}) = \$1237.95$

</br>

<span style="color:red;">
This portfolio has a positive and certain profit
</span>

## Law of one price

Say we have assets A and B where Prices $P_{a}(t)$ and $P_{b}(t)$ are prices at time $t$. Then there is $Prob(P_{a}(t) = P_{b}(t)) = 1$ for some time $t>0$.

Then one of two things has to be true.

- $P_{a}(0) = P_{b}(0)$
- There is an arbitrage.

Justification of the law of one price:

Suppose $P_{a}(0) \neq P_{b}(0)$:

- these are the prices known today so not random.
- This means one had to be bigger than the other $P_{a}(0) > P_{b}(0)$ or $P_{a}(0) < P_{b}(0)$. Let's assume $P_{a}(0) > P_{b}(0)$.

now let's construct an arbitrage.

- short position in A
- long position in B

long position would be buying asset B. A short position could be borrowing asset A selling it and promissing to return it on a future date.

