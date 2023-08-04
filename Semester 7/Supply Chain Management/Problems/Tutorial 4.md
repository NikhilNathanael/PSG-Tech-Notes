---
Filetype: "Problem"
Subject: "Supply Chain Management"
---

# Problem 1
Consider a distributor of TV set that order from manufacturer and sells to retailer. Suppose the distributor of the TV sets is trying to set inventory policies at the warehouse for one of the TV models. Assume that whenever the distributor places an order for TV sets, there is a fixed ordering cost of Rs 4500/- which is independent of the order size. The cost of a TV set to the distributor is Rs. 250 and annual inventory holding cost is about 18% of the product cost. Replenishment **lead time** is about **2 weeks**. The table provided below has the data on the number of TV sets sold to retailers in each of the last 12 months. Given the distributor would like to ensure 97% (Z=1.88) service level. What is the order level and the order quantity that the distributor should use.

| Month | Sept | Oct | Nov | Dec | Jan | Feb | Mar | Apr | May | Jun | July | Aug |
| ----- | ---- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ---- | --- |
| Sales | 200  | 152 | 100 | 221 | 287 | 176 | 151 | 198 | 246 | 309 | 98   | 156 | 

Average demand per month = 
$$
\dfrac{200+152+100+221+287+176+151+198+246+309+98+156}{12}= 191.1666666667
$$
Average Demand per week = 
$$191.1666666667/(52/12) = 44.1153846154$$
Standard Deviation = 

$$
\sqrt {\dfrac {\sum_1^{12} (x_i-\bar{x})^2} {12}}
= 41.7197162289
$$

$$
\begin{align}
ROP &= D\times L + Z\times \sigma \times \sqrt{L} \\
L &= 2\space \text{weeks} \\
D &= 44.1153846154 \space \text{per week} \\ \\
ROP &= 44.1153846154 \times 2 + 1.88 \times 41.7197162289 \times \sqrt {2} \\
ROP &= 199.1192021442
\end{align}
$$

Average Inventory Level = $\dfrac{Q}{2} + SS$
