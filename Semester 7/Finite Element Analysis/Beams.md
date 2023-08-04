---
Filetype: "Notes"
Subject: "Finite Element Analysis"
---

# Introduction
Each element in a beam has 2 degrees of freedom
The degrees of freedom in a beam are represented by the matrix 
$$
\begin{align}
[Q] &=
\begin{bmatrix}
Q_1 & Q_2 & ... & Q_{2n}
\end{bmatrix}
\end{align}
$$

where 
  n is the number of elements in the beam
  $Q$ is the global displacement 

The odd degrees of freedom ($Q_1$, $Q_3$, ..., $Q_{2j-1}$) represent the displacement of the beam at the node
The even degrees of freedom ($Q_2$, $Q_4$, ..., $Q_{2j}$) represent the slope of the beam at the node

# Local Coordinates

Consider a single element in the beam which contains two nodes
This element contains 4 degrees of freedom
  - The displacement of the first node ($q_1$)
  - The slope of the first node ($q_2$)
  - The displacement of the second node ($q_3$)
  - The slope of the second node ($q_4$)

This can be represented with the following matrix
$$
\begin{align}
[q] &= \begin{bmatrix} q_1 & q_2 & q_3 & q_4\end{bmatrix} \\
 &= \begin{bmatrix} v_1 & v_1' & v_2 & v_2'\end{bmatrix}
\end{align}
$$


# Shape Function
The Shape function used for beams is a Hermite Function
The interpolation term $\epsilon$ varies from -1 to 1 as $x$ moves from $x_1$ to $x_2$

Each Hermite function is given by the general form
$$
H_i = a_i + b_i \epsilon + c_i \epsilon^2 + d_i \epsilon^3 \text{ for } i = 1,2,3,4
$$
where $H_i$ is the interpolation function for $q_i$

The conditions in the following table must be satisfied for all the Hermite equations

|                 | $H_1$ | $H_1'$ | $H_2$ | $H_2'$ | $H_3$ | $H_3'$ | $H_4$ | $H_4'$ |
| --------------- | ----- | ------ | ----- | ------ | ----- | ------ | ----- | ------ |
| $\epsilon = -1$ | 1     | 0      | 0     | 1      | 0     | 0      | 0     | 0      |
| $\epsilon = 1$  | 0     | 0      | 0     | 0      | 1     | 0      | 0     | 1      | 

For $H_1$ 

$$
\begin{align}
H_1 = a_1 + b_1 \epsilon + c_1 \epsilon^2 + d_1 \epsilon^3 \\
H_1' = b_1 + 2c_1 \epsilon + 3d_1 \epsilon^2
\end{align}
$$
substituting
$$
\begin{align}
H_1 (-1) = 1 \\
H_1' (-1) = 0 \\
H_1 (1) = 0 \\
H_1' (1) = 0 \\
\end{align}
$$
we get 

$$ 
\begin{align}
1 &= a_1 - b_1 + c_1 - d_1 \\
0 &= b_1 - 2c_1 + 3d_1 \\
0 &= a_1 + b_1 + c_1 + d_1 \\
0 &= b_1 + 2c_1 + 3d_1 \\
\end{align}
$$

which results in 

$$
\begin{align}
a_1 &= \dfrac{1}{2}\\
  b_1 &= -\dfrac{3}{4} \\
c_1 &= 0 \\
d_1 &= \dfrac{1}{4}\\
\end{align}
$$
which can be represented as

$$
H_1 = \begin{bmatrix} a_1 & b_1 & c_1 & d_1 \end{bmatrix} = 
\begin{bmatrix}
\dfrac{1}{2} & -\dfrac{3}{4} & 0 & \dfrac{1}{4}
\end{bmatrix}
$$

Similiarly the other coefficients can be found

$$
\begin{align}
H_2 &= 
\begin{bmatrix}
\dfrac{1}{4} & -\dfrac{1}{4} & -\dfrac{1}{4} & \dfrac{1}{4}
\end{bmatrix}
\\
H_3 &= 
\begin{bmatrix}
\dfrac{1}{2} & \dfrac{3}{4} & 0 & \dfrac{1}{4}
\end{bmatrix}
\\ 
H_4 &= 
\begin{bmatrix}
-\dfrac{1}{4} & -\dfrac{1}{4} & \dfrac{1}{4} & \dfrac{1}{4} 
\end{bmatrix}
\end{align}
$$


```functionplot
---
title: Hermite Shape Functions
xLabel: epsilon
yLabel: H
bounds: [-1,1,-2,2]
disableZoom: true
grid: true
---
H_1 = 1/2 - 3x/4 + x^3/4
H_2 = 1/4 - x/4 - x^2/4 + x^3/4
H_3 = 1/2 + 3x/4 - x^3/4
H_4 = -1/4 - x/4 + x^2/4 + x^3/4
```
