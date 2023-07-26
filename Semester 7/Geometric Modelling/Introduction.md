---
Filetype: Notes
Subject: "Geometric Modelling"
---

# Overview
## Geometric Transformations
### Linear Transformations
$$
\begin{bmatrix}
x' \\ y'
\end{bmatrix}
= 
\begin{bmatrix}
a & b \\ c & d
\end{bmatrix}
\times
\begin{bmatrix}
x \\ y
\end{bmatrix}
$$
- Linear Transformations are combinations of 
  1. Scale
  2. Rotation
  3. Shear
  4. Mirror
#### Properties
  - Satisfies $T(s_1 p_1 + s_2 p_2) = s_1 T(p_1) + s_2 T(p_2)$
  - Origin maps to origin
  - Lines map to lines
  - Parallel lines remain parallel
  - Ratios are preserved

### Affine Transformations
- They are the generalizations of Euclidean transformation and combinations of 
  - Linear Transformations 
  - Translations

### Projective Transformations
$$
\begin{align}
\begin{bmatrix}
x' \\ y' \\ z'
\end{bmatrix}
=
\begin{bmatrix}
a & b & c \\ d & e & f \\ g & h & i
\end{bmatrix}
\times 
\begin{bmatrix}
x \\ y \\ z
\end{bmatrix}
\end{align}$$
- They are the most general linear transformations and require the use of homogeneous coordinates
#### Properties
- Origin does not necessarily map to origin
- Lines map to linear
- Parallel lines do not necessarily remain parallel
- Ratios are not preserved
- Closed under composition

### Transformation of Objects
- Basic transformations are:
  1. Translation
  2. Rotation
  3. Scaling
- They are represented as a matrix which is applied to a coordinate matrix
    $$
    [X'] = T_1 \times [X]
  $$
- To apply multiple transformations one after the other, each successive transformation matrix is applied to the left of the previous matrix
    $$
    [X'] = T_3 \times T_2 \times T_1 \times [X]
  $$
#### Application
- Animation
  - We use parametrized transformations that change over time t
  - Thus for each frame the object moves a little further, just like a movie
