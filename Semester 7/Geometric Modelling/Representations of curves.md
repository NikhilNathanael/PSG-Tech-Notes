---
Filetype: "Notes"
Subject: "Geometric Modelling"
---

# Types
## Non-Parametric
The points that make up the curve are directly given
It is not used in any Software
### Explicit
The points used directly
### Implicit
## Parametric
### Analytic
They are curves that are represented by a standard function such as
- A Circle
- An Ellipse
- A line
- A Parabola
### Synthetic
They are curves which are defined by a set of control points
#### Interpolant Curve
The are curves which pass through all control points
##### Hermite Cubic Spline
#### Approximant Curve
They are curves which do not pass through all control points
##### Bezier Spline
##### B-Spline/NURBS
Non-Uniform Rational B-Spline

# Continuity of Curves
## Position Continuity ($C_0$)
The function representing the coordinates of the curve is continuous at all points
## Slope Continuity ($C_1$)
The function representing the slope of the function is continuous at all points
## Curvature Continuity ($C_2$)
The function representing the curvature of the curve is continuous at all points

# Parametric Representation 
## Parametric Representation of a line
Consider two points $P_1$ and $P_2$ 
A line segment connecting $P_1$ and $P_2$ can be represented as the set of all points which can be interpolated between them 

$$
\begin{align}
P &= P_1 + (P - P_1) \\
P - P_1 &= u(P_2 - P_1) \\
P(u) &= P_1 + u(P_2 - P_1) \\
\end{align}
$$
This equation is split between all the axes
$$
\begin{align}
x(u) &= x_1 + u(x_2-x_1) \\
y(u) &= y_1 + u(y_2-y_1) \\
z(u) &= z_1 + u(z_2-z_1) \\
\end{align}
$$
Differentiating, we get
$$
\begin{align}
P'(u) &= (P_2 - P_1)
\end{align}
$$
Unit vector is a vector in the direction of the second point from the first point
$$
\hat{u} = \dfrac{P_2 - P_1}{L}
$$

$$
P(u) = P_1 + L\hat{n} 
$$
## Parametric Representation of a Circle

## Generalized Parametric Representation

$$
\begin{align}
P(u) &= \begin{bmatrix} x(u) & y(u) & z(u) \end{bmatrix}^T \text { for all } u_{\text{min}} \le u \le u_{\text{max}} \\ 
P'(u) &= \begin{bmatrix} x'(u) & y'(u) & z'(u) \end{bmatrix}^T \text { for all } u_{\text{min}} \le u \le u_{\text{max}} \\ 
\end{align}
$$

$$
0 \le u \le 1
$$
