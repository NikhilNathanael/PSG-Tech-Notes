---
Filetype: "Notes"
Subject: "Finite Element Analysis"
---


# Introduction
In three dimensions, there are 6 degrees of freedom for the stress acting on an element
$$
\begin{matrix}
\sigma_x & \tau_{xy} \\
\sigma_y & \tau_{xz} \\
\sigma_z & \tau_{yz} \\
\end{matrix}
$$
Forces acting along the third dimension are negligible so the only stress that are non-zero are 

$$
\begin{matrix}
\sigma_x && \tau_{xy} \\
\sigma_y
\end{matrix}
$$


let $f_x$, $f_y$ be body force components per unit volume at $(x, y)$
# Basic Equation for strain

$$
\begin{align}
F &= \begin{bmatrix} f_x & f_y\end{bmatrix}^T \\
T &= \begin{bmatrix} T_x & T_y\end{bmatrix}^T \\

\epsilon &= \begin{bmatrix} 
\dfrac{\delta u}{\delta x} & 
\dfrac{\delta v}{\delta y} &
(\dfrac{\delta u}{\delta y} + \dfrac{\delta v}{\delta x})
\end{bmatrix}
\end{align}
$$

# Displacement Equations

$$
\begin{align}
u &= N_1 q_1 + N_2 q_3 + N_3 q_5 \\
v &= N_1 q_2 + N_2 q_4 + N_3 q_6 \\
\end{align}
$$
$$
\begin{align}
N_1 &= \epsilon \\
N_2 &= \eta \\
N_3 &= 1 - \epsilon -\eta 
\end{align}
$$


$$
\begin{align}
u &= (q_1 - q_5)\epsilon + (q_3-q_5)\eta +q_5 \\
v &= (q_2 - q_6)\epsilon + (q_4-q_6)\eta +q_6 \\
\newline
N &= \begin{bmatrix}
N_1 & 0 & N_2 & 0 & N_3 & 0 \\
0 & N_1 & 0 & N_2 & 0 & N_3 \\
\end{bmatrix}
\end{align}
$$

# Isoparametric Representation

$$
\begin{align}
x &= N_1 x_1 + N_2 x_2 + N_3 x_3 \\
y &= N_1 y_1 + N_2 y_2 + N_3 y_3 \\
\end{align}
$$

$$
\begin{align}
N_1 &= \epsilon \\
N_2 &= \eta \\
N_3 &= 1 - \epsilon -\eta 
\end{align}
$$

$$
\begin{align}
x &= (x_1 - x_3)\epsilon + (x_2 - x_3) \eta + x_3 \\
y &= (y_1 - y_3)\epsilon + (y_2 - y_3) \eta + y_3 \\
\end{align}
$$

let $x_{ij} = x_i - x_j$

$$
\begin{align}
x &= x_{13} \epsilon + x_{23} \eta + x_3 \\
y &= y_{13} \epsilon + y_{23} \eta + y_3 \\
\end{align}
$$

## Calculating Strain
$$
\begin{align}
\dfrac{\delta u }{\delta \epsilon} = \dfrac{\delta u}{\delta x} \dfrac{\delta x }{\delta \epsilon} + \dfrac{\delta u}{\delta y} \dfrac{\delta y}{\delta \epsilon} \\
\dfrac{\delta u }{\delta \eta} = \dfrac{\delta u}{\delta x} \dfrac{\delta x }{\delta \eta} + \dfrac{\delta u}{\delta y} \dfrac{\delta y}{\delta \eta} \\
\end{align}
$$

$$
\begin{align}
\begin{Bmatrix}
\end{Bmatrix}
\end{align}
$$

## Final Equation

$$
\begin{align}
B &= \dfrac{1}{\det J} 
\begin{Bmatrix}
y_{23} & 0 & y_{31} & 0 & y_{12} & 0 \\ 
0 & x_{32} & 0 & x_{13} & 0 & x_{21} \\ 
x_{32} & y_{23} & x_{13} & y_{31} & x_{21} & y_{12} \\
\end{Bmatrix}
\end{align}
$$


# Stiffness Derivation
$$
\begin{align}

\end{align}
$$

For Plane Stress conditions, The value of $D$ is given by 

$$
\begin{align}
D &= \dfrac{\epsilon} {1-\gamma^2} 
\begin{bmatrix}
\gamma & \gamma & 0 \\
\gamma & 1 & 0 \\
0 & 0 & \dfrac{1-\gamma}{2} \\
\end{bmatrix} \rightarrow \text{Plane Stress} \\

D &= \dfrac{\epsilon} {(1+\gamma) (1-2\gamma)} 
\begin{bmatrix}
1 - \gamma & \gamma & 0 \\
\gamma & 1 - \gamma & 0 \\
0 & 0 & \dfrac{1-\gamma}{2} \\
\end{bmatrix} \rightarrow \text{Plane Strain}  

\end{align}
$$
