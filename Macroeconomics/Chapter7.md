# Chapter 7 Economic Growth: Malthus and Solow
* ***Malthusian Model:***
  Any improvement in technology for producing goods leads to increased population growth, *so that in the long run there is no improvement in the standard of living.*
  
  ***Predicts that the only means for improving the standard of living is population control***

*  ***Solow Model:***

  A country's standard of living cannot continue to improve in the long run in the absence of continuing increases in total factor productivity. In the short run, the standard of living can improve if a country’s residents save and invest more, thus accumulating more capital.

> ***Solow growth model*** is an exogenous growth model.

## Economic Growth Facts

1. *Before the Industrial Revolution in about 1800, standards of living differed little over time and across countries.*
2. *Since the Industrial Revolution, per capita income growth has been sustained in the richest countries. In the United States, average annual growth in per capita income has been about 2% since 1900.*
3. *There is a positive correlation between the rate of investment and output per worker across countries.*
4. *There is a negative correlation between the population growth rate and output per worker across countries*
5. *Differences in per capita incomes increased dramatically among countries of the world between 1800 and 1950, with the gap widening between the countries of Western Europe, the United States, Canada, Australia, and New Zealand, as a group, and the rest of the world.*
6. *There is essentially no correlation across countries between the level of output per capita in 1960 and the average rate of growth in output per capita for the years 1960–2007.*
7. *Richer countries are much more alike in terms of rates of growth of real per capita income than are poor countries*.

## The Malthusian Model of Economic Growth

In the analysis we confine attention to the ***current period*** and the ***future*** period

### The model that formalizes Malthusian theory

* Aggregate production function

$$
Y=zF(L,N)
$$

> current inputs of land, L and current labor, N

* Basic assumption: ***as was the case in Western Europe in 1798***

  1. F is a function including constant returns to scale
  2. L is a fixed supply
  3. **Each person in this economy is willing to work at any wage and has one unit of labor to supply, so that N is both the population and the labor input**

* Population equation:
  $$
  N'=N+Births-Deaths
  $$
  or
  $$
  N'=N+N(birth\quad rate-death \quad rate)
  $$

* **Particularly before the *Industrial Revolution*, birth rate would be an increasing function of consumption per capita**

  this implies the following equation:
  $$
  \frac{N'}{N}=g(\frac{C}{N})
  $$

  > g: an increasing function
  > $$
  > \frac{N'}{N}: 1+growth \quad rate
  > $$

* In equilibrium, all goods produced are consumed (because I=G=NX=0), so that C=Y.
  $$
  C=zF(L,N)
  \Rightarrow\\
  \frac{N'}{N}=g(\frac{zF(L,N)}{N})
  $$

  > given that the constant-returns-to-scale property

  $$
  xzF(L,N)=zF(xL,xN)
  $$

  > for any x>0, take that 
  > $$
  > x=\frac{1}{N}
  > $$

  we can rewrite the constant-returns-to-scale property as
  $$
  \frac{zF(L,N)}{N}=zF(\frac{L}{N},1)
  $$
  so that
  $$
  N'=g[zF(\frac{L}{N},1)]N
  $$
  The diagram is as follows, N* is the ***steady state***
  ![image-20211106120030197](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211106120030197.png)



### Analysis of the Steady State

$$
Y=zF(L,N)\\
\Rightarrow\\
\frac{Y}{N}=\frac{zF(L,N)}{N}=zF(\frac{L}{N},1)
$$

*let* **y** be output per worker, **l** be land per work, **c** be consumption per worker
$$
y=\frac{Y}{N},l=\frac{L}{N},c=\frac{C}{N}\\
rewrite \quad the \quad above \quad equation:\\
y=zf(l)
$$
this is the ***per-worker production function***,which describes the quantity of output per worker *y* that can be produced for each quantity of land per worker *l*, with the function *f* defined by 
$$
f(l)=F(l,1)
$$
Note that c=y, we get
$$
c=y=zf(l)
$$
We can also rewrite
$$
\frac{N'}{N}=g(zF(\frac{L}{N},1))
$$
as 
$$
\frac{N'}{N}=g(c)
$$

The steady state N* implies that N=N', so that g(c*)=1 and l\* determined by c\*. Also N\*=L/l\*.

#### The Effects of an Increase in z on the Steady State

$$
z \uparrow \\
\Rightarrow c^* \quad in \quad the \quad end \quad remains \quad the \quad same \quad satisfying  \\
\frac{N'}{N}=g(c)=1\\
\Rightarrow l^* \downarrow\\
N^*=\frac{L}{l^*}\uparrow
$$

* The economy does not move to the new steady state instantaneously, as it takes time for the population and consumption to adjust.

* Initially, the effect of this is to increase output, consumption, and consumption per worker, as there is no effect on the current population at time *T*.

* However, because consumption per worker has increased, there is an increase in population growth.

* consumption per worker falls (given the fixed quantity of land), until consumption per worker converges to *c\**, its initial level, and the population converges to its new higher level *N\**.

  ![image-20211106135846914](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211106135846914.png)
  

#### Population Control

Reducing the rate of population growth has the following effect
$$
g_1(c) \rightarrow g_2(c)\\
\forall c,g_1(c)\ge g_2(c)\\
s.t.c_2^*>c_1^*,where \quad g_1(c_1^*)=g_2(c_2^*)=1\\
\Rightarrow\\
l_2^*>l_1^*\\
\Rightarrow\\
N_2^*=\frac{L}{l_2^*}<N_1^*=\frac{L}{l_1^*}
$$


### Comments on the Malthusian Model

1. Malthus did not allow for the effect of increases in the capital stock on production. Having more capital implies that there is more productive capacity to produce additional capital. In other words, capital can reproduce itself.
2.  Malthus did not account for all of the effects of economic forces on population growth. While it is clear that a higher standard of living reduces death rates through better nutrition and health care, there has also proved to be a reduction in birth rates.



## The Solow Model: Exogenous Growth

* Two periods: ***current*** and ***future***

### Consumers

In contrast to Malthusian model, Solow model supposes that the population grows exogenously.
$$
N'=(1+n)N
\quad n>-1
$$

> N' is the population in the future period

* ***Assumption***: 
  1. In each period, a given consumer has one unit of time available, assuming that consumers don't value leisure gives that they supply their one unit of time as labor in each period.
  
  2. All members work and no unemployment gives that population(N)=labor force
  
  3. Consumers receive all current real output Y as income.
  
  4. ***Consumers here face a decision concerning how much of their current income to consume and how much to save.***
  
     Thus
     $$
     C=(1-s)Y,C+S=Y\\
     \Rightarrow\\
     S=sY
     $$
  
     > ***S is aggregate savings, s is the aggregate saving rate***

### The Representative Firm

As in the Malthusian model, production function F has the property of constant-returns -to-scale.
$$
\frac{Y}{N}=zF(\frac{K}{N},1)
$$

> Y/N output per worker
>
> K/N capital per worker

Rewriting the above function as 
$$
y=zf(K)\\
where \quad f(k)=F(k,1)
$$
Its slope is the marginal product of capital.

We also assume that some of the capital stock wears out through each period with the depreciation rate a constant d.
$$
K’=(1-d)K+I, 0<d<1
$$

> K': the future capital stock,
>
> K: current capital stock
>
> I: investment



### Competitive Equilibrium

Two markets in the current period:

1. First market: current consumption goods are traded for current labor.
2. Second market: current consumption goods are traded for capital.

***Capital is the asset in this model and consumers save by accumulating it. The labor market and the capital market must clear in each period.***

**In the labor market, the quantity of labor is always determined by the inelastic supply of labor, which is *N*. That is, because the supply of labor is *N* no matter what the real wage, the real wage adjusts in the current period so that the representative firm wishes to hire *N* workers.**

Capital market is in equilibrium in the current period if 
$$
S=I
$$
since
$$
S=Y-C
$$
the equilibrium condition can be written as
$$
Y=C+I
$$
since
$$
C=Y-S=(1-s)Y\\
K'=(1-d)K+I
$$
we get
$$
Y=(1-s)Y+K'-(1-d)K\\
\Rightarrow\\
K'=sY+(1-d)K=S+(1-d)K
$$

> The capital stock in the future period is the quantity of aggregate savings in the current period plus the capital stock left over from the current period.

also
$$
Y=zF(K,N)\\
\Rightarrow\\
K'=szF(K,N)+(1-d)K
$$
In per-worker terms:
$$
\frac{K'}{N}=sz\frac{F(K,N)}{N}+(1-d)\frac{K}{N}\\
\Rightarrow\\
\frac{K'}{N}\frac{N'}{N'}=sz\frac{F(K,N)}{N}+(1-d)\frac{K}{N}\\
\Rightarrow\\
k'(1+n)=szf(k)+(1-d)k\\
\Rightarrow\\
k'=\frac{szf(k)}{1+n}+\frac{(1-d)k}{1+n}
$$

The diagram looks as follows, ***k\**** is the steady state.

![image-20211106194055810](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211106194055810.png)

In the long run, therefore, if the savings rate, the labor force growth rate, and total factor productivity are constant, then growth rates in aggregate quantities are determined by the growth rate in the labor force. This is one sense in which the Solow growth model is an exogenous growth model. ***In the long run, the Solow model tells us that growth in key macroeconomic aggregates is determined by exogenous labor force growth when the savings rate, the labor force growth rate, and total factor productivity are constant.***

### Analysis of the Steady State

 For the steady state k\*, we have
$$
k^*=\frac{szf(k^*)}{1+n}+\frac{(1-d)k^*}{1+n}\\
\Rightarrow\\
szf(k^*)=(n+d)k^*
$$
It takes the following form:

![image-20211106202659470](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211106202659470.png)

#### The Steady State Effects of an Increase in the Savings Rate

$$
s\uparrow:s_1\rightarrow s_2 \quad where \quad s_2>s_1\\
k^*,y^* \quad increases
$$

However, the growth rate of the aggregate output Y remains n.

#### Consumption per Worker and Golden Rule Capital Accumulation

The consumption per worker in the steady state is given by
$$
c^*=zf(k^*)-(n+d)k^*
$$
As is shown in the diagram below

![image-20211106211730670](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211106211730670.png)
$$
k^*_{gr}:golden \quad rule \quad quantity \quad of \quad capital \quad per \quad worker\\
c^{**}:the\quad maximum \quad consumption\quad per \quad worker
$$

* ***Golden rule quantity of capital per worker:*** a quantity of capital per worker for which consumption per worker is maximized.

* ***Property of the golden rule:*** the slope of the per-worker production function of k*=k\*gr is equal to the slope of the function (n+d)k\*.

* ***Golden rule savings rate***: achieves the golden rule quantity of capital per work in a competitive equilibrium steady state.

  That is, at the golden rule steady state we have
  $$
  MP_K=n+d
  $$
  <img src="C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211107002218779.png" alt="image-20211107002218779" style="zoom: 200%;" />

  From the figure above, we can tell that

  * If the steady state capital stock per worker is less than *k*∗*gr*,then an increase in the savings rate *s* increases the steady state capital stock per worker

    and increases consumption per worker.

  * However if k*>k\*gr, then an increase in the savings rate increases k\* and causes a decrease in consumption per worker.

#### The Steady State Effects of an Increase in Labor Force Growth

![image-20211107101050173](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211107101050173.png)

***An increase in the labor force growth rate causes a decrease in the steady state quantity of capital per worker.***

Note that ***aggregate output, aggregate consumption, and aggregate investment grow at the labor force growth rate n in the steady state.***Therefore, when the labor force growth rate increases, growth in all of these variables must also increase.

#### The Steady State Effects of an Increase in Total Factor Productivity

* If we take real income per worker to be a measure of the standard of living in a country, what we have shown thus far is that, in the Solow model, an increase in the savings rate or a decrease in the labor force growth rate can increase the standard of living in the long run. 
* However, increases in the savings rate and reductions in the labor force growth rate cannot bring about an ever-increasing standard of living in a country
*  The Solow model predicts that a country’s standard of living can continue to increase in the long run only if there are continuing increases in total factor productivity

The changes in z are shown as below:

![image-20211107102412621](C:\Users\Junzhe Li\AppData\Roaming\Typora\typora-user-images\image-20211107102412621.png)



## Growth Accounting

* **Definition**:.A useful exercise is to measure how much of the growth in aggregate output over a given period of time is accounted for by growth in each of the inputs to production and by increases in total factor productivity.

Consider
$$
Y=zF(K,N)
$$
Using the wide-used Cobb-Douglas production function
$$
F(K,N)=K^aN^{1-a}
$$

* ***Solow residual***
  $$
  \hat{z}=\frac{\hat{Y}}{\hat{K^{0.3}}\hat{N^{0.7}}}\\
  where \quad \hat{Y},\hat{K},\hat{N} \quad are \quad measures \quad of \quad aggregate \quad output,\quad capital \quad input, \quad labor \quad input
  $$
  

