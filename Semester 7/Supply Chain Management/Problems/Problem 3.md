---
Filetype : "Problem"
Topic : "Network Reconfiguration"
Subject : "Suppply Chain Management"
---

# Problem 3
A firm has three factories, namely A, E, and K. There are four major warehouses situated at B, C, D and M. The average daily production at A, E, and K are 30, 40, and 50 units respectively. The average daily requirement of this product is given by this table at B, C, D, and M are 35, 28, 32, and 25 units respectively. The transportation costs per unit of product from each factory to each warehouse is given in the table below

|           | Warehouse |     |     |     |        |
| --------- | --------- | --- | --- | --- | ------ |
| Factories | B         | C   | D   | M   | Supply |
| A         | 6         | 8   | 8   | 5   | 30     |
| E         | 5         | 11  | 9   | 7   | 40     |
| K         | 8         | 9   | 7   | 13  | 50     |
| Demand    | 35        | 28  | 32  | 25  | 120    |

Draw the network representation of this problem, formulate an LPP model to determine the least expensive shipping plan to fulfill the demands at the stores.

### Solution
Minimize 
  $$\begin{align*}
  Z &= 6(AB) + 8(AC) + 8(AD) + 5(AM) \\
    &+ 5(EB) + 11(EC) + 9(ED) + 7(EM) \\
    &+ 8(KB) + 9(KC) + 7(KD) + 13(KM)
  \end{align*}$$

Subject  to
  $$\begin{align*}
  (AB) + (AC) + (AD) + (AM) &\le 30 \\
  (EB) + (EC) + (ED) + (EM) &\le 40 \\
  (KB) + (KC) + (KD) + (KM) &\le 50 \\
  
  (AB) + (EB) + (KB) &= 35 \\
  (AC) + (EC) + (KC) &= 28 \\
  (AD) + (ED) + (KD) &= 32 \\
  (AM) + (EM) + (KM) &= 25 \\
  \end{align*}$$

