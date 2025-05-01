# Price and Real Effect Share (PRES) Model

Imagine that you are holding a basket, and often you put in a handful of balls. These balls come in only two colors: orange and blue. The size of each handful varies — sometimes it's small, sometimes large. But no matter the size, every ball you drop into the basket must be either orange or blue. Over time, as you keep adding more and more balls, the mix in your basket begins to tell a story. If the majority of your handfuls are filled with blue balls, your basket will start looking more and more blue. If orange dominates, then so will the color inside. The essence of this analysis is understanding a mix similar to this. Specifically, when new money comes into the economy, what’s the price effect share (leading to inflation) and what’s the real effect share (leading to real output growth)? I am pleased to introduce new approach for inflation analysis based on a framework that can effectively decomposes the additional money supply into price effect share (PES) - share of the monetary impulse on influencing prices, and real effect share (RES) -  share of the monetary impulse on influencing real output.

## Theoretical Framework

To simplify this analysis, but without losing its essence a bit, a crucial assumption has been introduced: (1) money functions primarily as a medium of exchange for goods and services. Meaning, it facilitates expenditures across all components of the GDP, i.e., money expenditures corresponds nominal GDP. So that we have:

M · V = P · Y

Where M is the level of the money supply, V is the velocity of money, P is the price level, and Y is the real GDP. Moving forward, it is assumed that (2) the velocity V is relatively stable and normalized to 1. Then, under these assumptions (V=1, ΔV≈0), if the money supply increases by an amount of ΔM the change in nominal GDP must match this additional money. Mathematically:

ΔM = Δ(P·Y)

Recall that nominal GDP is given by P·Y. Taking a differential (product rule for differentials) of both sides gives:

Δ(P·Y) = Y · ΔP + P · ΔY

This equation tells that the change in nominal GDP (or the additional money in the economy, ΔM) can be broken down into two components:

- Y · ΔP - The part of change due to an increase in prices (price effect).
- P · ΔY - The part of the change due to an increase in real output (real effect).

So we can write the additional money in the economy as:

ΔM = Y · ΔP + P · ΔY

Dividing both sides by ΔM gives these effects as proportions of the total monetary impulse (ΔM):

- Price Effect Share (PES) = Y · ΔP / ΔM
- Real Effect Share (RES) = P · ΔY / ΔM

Therefore, we can write: 

(Y · ΔP / ΔM) + (P · ΔY / ΔM) = 1

That is:

PES + RES = 1

In this framework the PES represents the share of monetary impulse attributed to price increases and RES represents the share of monetary impulse attributed to actual increases in real output, These shares sum to approximately one. Which tells that each additional money supply ΔM itself is allocated between influencing prices and being absorbed by real output. This decomposition helps understand how an increase in money supply affects the economy. If PES is larger for a greater number of years in a given period, then more of the monetary expansion is causing inflation. Conversely, if RES is larger for a greater number of years, then the economy is absorbing the extra money by producing more goods and services. This framework provides a clear way to conceptualize and quantify these shares and policy target goals as well. 

## The Empirical Model

The underlying framework suggests that an increase in money supply M, if not matched by increases in real output Y, will tend to put upward pressure on price level P, which posits a direct relationship between money supply and inflation. So, we can express the model as follows:

P = f(M)

It states that price level P is a function of the level of money supply M. But instead of looking at overall levels of money supply and prices, it’s better to focus on changes - how changes in money supply relate to changes in price level. By focusing on how they change from year to year we can better isolate the true relationship. So, we can rewrite the model as follows:

ΔP = f(ΔM)

However, the change in money supply ΔM, is not proportional to the change in price level ΔP. The coefficient ‘b’ can tell us, on average, how much prices go up when the money supply increases (b = ΔP / ΔM). It tells how sensitive prices are, on average, to changes in money supply. To imply, we can rewrite the model as follows:

ΔP = b · ΔM

However, there always exists a mild inflation in the economy, even though there is no additional money supply (ΔM=0). That is what we see that even during times of stable money supply, there exists a mild inflation. To account for this autonomous trend in price level changes, an intercept term 'a' is included. This leads to the final model specification:

ΔP = a + b · ΔM

## Linking the Model to the Theoretical Framework

The power of this model extends beyond just measuring the marginal impact of ΔM on ΔP. It provides a crucial link back to the theoretical framework where the monetary impulse was seen to split between price and output effects.

PES + RES = 1

Recall the coefficient b = ΔP / ΔM. Also recall the Price Effect Share (PES) = Y · ΔP / ΔM. Notice that ΔP / ΔM is in both! Hence, the theoretical PES can be directly estimateed by multiplying the regression coefficient ‘b’ by the real output Y:

PES = b · Y

Thus, we now have:

PES = b · Y = Y · ΔP / ΔM

Multiplying ‘b’ with the corresponding year’s real GDP Y we could easily estimate the average Price Effect Share (PES) for the year directly from the given relationship. Additionally, the average Real Effect Share (RES) can be estimated as:

RES = 1 - PES

The regression result of this model ΔP = a + b · ΔM, can be connected to the theoretical breakdown of how money growth is split into inflation and real output growth. That’s the power of the ‘b’ coefficient in the model, it doesn’t just tell the marginal effect of ΔM on ΔP; it gives a clean way to estimate the price effect and the real effect shares. 

## Interpreting Monetary Effects on Inflation

A key strength of the proposed empirical model lies in its direct applicability to analyzing inflation dynamics using readily available data. The model requires only time series data for the change in the price level (ΔP) as the dependent variable and the change in the money supply (ΔM) as the independent variable. Upon fitting this data via regression analysis, the estimated coefficient 'b' becomes crucial. As established, 'b' represents the average sensitivity of price level changes to changes in the money supply. This coefficient provides the essential link back to the theoretical framework's decomposition of monetary effects. By multiplying 'b' with the corresponding real GDP (Y), we can directly estimate the average Price Effect Share (PES≈b⋅Y) for that period.   

The interpretation of PES is central to understanding inflation dynamics within this framework. A larger PES value relative to RES (RES = 1 - PES) suggests that a greater proportion of the additional money supply (ΔM) is associated with increases in the price level (inflation) rather than being absorbed by real economic activity. If the analysis reveals that PES is significantly high for a sustained number of years, it indicates that monetary expansion during that period was predominantly inflationary, implying a stronger observable correlation between money supply growth and price level increases.

## Empirical Estimation for PES

<img width="1337" alt="Screenshot 2025-04-30 at 10 06 57 AM" src="https://github.com/user-attachments/assets/bd9afc44-f4c0-4e39-859f-dad8d0ac11b5" />

As established, Price Effect Share (PES) can be estimated for each year using the model's coefficient and corresponding real output. This plot represents this model-estimated PES against the actual PES calculated directly from the annual data within the theoretical framework. It visually demonstrates the utility of the empirical model. The relatively stable line, representing the PES estimated directly via the model's coefficient (b · Y), clearly tracks the central tendency of the more volatile line, which represents the actual year-by-year PES. It effectively identifies the underlying average relationship linking monetary changes to price level effects over the period. 

Despite its simplicity, the model can quantify the share that fuels inflation versus real growth, enabling central banks to target stimulus more effectively and control excess liquidity to preserve purchasing power. It can safeguard millions from high inflation and sustain the hard-won living standards. Refinements, critiques, and feedback on this proposal are encouraged and warmly welcomed.
