## 2D Scaling
### Uniform Scaling
Both coordinates are multiplied by the same value

$$
\begin{align}
x' = S \cdot x \\
y' = S \cdot y \\
\end{align}
$$
In matrix form

$$
\begin{align}
\begin{bmatrix}
x' \\ y' 
\end{bmatrix}
= 
S \cdot
\begin{bmatrix}
t_x \\ t_y
\end{bmatrix}
\end{align}
$$

### Non - Uniform Scaling 
Each component is multiplied by a different factor 
$$
\begin{align}
x' &= S_x \cdot x \\
y' &= S_y \cdot y \\
\end{align}
$$

In matrix form

$$
\begin{align}
\begin{bmatrix}
x' \\ y' 
\end{bmatrix}
= 
\begin{bmatrix}
S_x & 0 \\ 0 & S_y
\end{bmatrix}
\times 
\begin{bmatrix}
t_x \\ t_y
\end{bmatrix}
\end{align}
$$