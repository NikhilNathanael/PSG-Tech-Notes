---
filetype: "Notes"
Subject: "Finite Element Analysis"
---

# Limitations of 1D Elements
- It cannot model stress concentrations due to sudden change in shape
- Poisson effect (Change in area due to axial forces) is not accounted for

# Types of elements in 2 dimensions
## Triangular Elements
### Constant Strain Triangular Element (CST) 
It is a three noded element in which there is displacement in the X-direction and the Y-direction
The size of the stiffness matrix is 6x6
There is a constant strain ($\epsilon$) through the entire element

$$
\begin{align}
\epsilon &= c_1 \\
\dfrac{du}{dx} & = \epsilon = c \\ 
u & = \text{linear} \\
\end{align}
$$
therefore, 
$$
\epsilon = c, \sigma = c
$$
### Linear Strain Triangular Element (LST) 
There are 6 nodes in the LST element. One in each corner and one at the midpoint of each edge
The size of the stiffness matrix is 12x12
The strain varies linearly along a single edge

$$
\begin{align}
  \dfrac{du}{dx} = \epsilon &= a_0 + a_1 x \\
u &= a_0 x + a_1 x^2 + a_2 \\
\sigma & = \text{linear}
\end{align}
$$

This type of element is more computationally intensive but it is more accurate

## Quadrilateral element
### Constant Strain Quadrilateral Element (CSQ)
It contains 4 nodes, one at each corner
Similar to the Constant strain triangular element, the strain is constant throughout a single edge
### Linear Strain Quadrilateral Element (LSQ)
It contains 8 nodes, one at each corner and one at the midpoint of each edge
Similar to the linear strain triangular element, the strain increases linearly throughout an edge



