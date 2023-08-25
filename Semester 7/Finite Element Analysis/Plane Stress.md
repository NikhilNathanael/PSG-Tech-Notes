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
Basic Equation for strain

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