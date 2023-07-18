---
FileType : "Problem"
Topic : "Network Reconfiguration"
Subject : "Suppply Chain Management"
---
A firm has three factories, namely A, E, and K. There are four major warehouses situated at B, C, D and M. The average daily production at A, E, and K are 30, 40, and 50 units respectively. The average daily requirement of this product is given by this table at B, C, D, and M are 35, 28, 32, and 25 units respectively. The transportation costs per unit of product from each factory to each warehouse is given in the table below

|           | Warehouse |     |     |     |        |
| --------- | --------- | --- | --- | --- | ------ |
| Factories | B         | C   | D   | M   | Supply |
| A         | 6         | 8   | 8   | 5   | 30     |
| E         | 5         | 11  | 9   | 7   | 40     |
| K         | 8         | 9   | 7   | 13  | 50     |
| Demand    | 35        | 28  | 32  | 25  | 120    |

```HTML
<table>
  <thead>
    <tr>
      <th><\th>
      <th>Warehouse<\th>
      <th><\th>
      <th><\th>
      <th><\th>
      <th><\th>
    <\tr>
  <\thead>
  <tbody>
    <tr>
      <td columnspan=4>L1 Name</td>
      <td columnspan=2>L2 Name A</td>
    </tr>
  <\tbody>
<\table>
```

Draw the network representation of this problem, formulate an LPP model to determine the least expensive shipping plan to fulfill the demands at the stores.

### Solution
Minimize $Z = 6(AB) + 8(AC) + 8(AD) + 5(AM) + 5(EB) + $