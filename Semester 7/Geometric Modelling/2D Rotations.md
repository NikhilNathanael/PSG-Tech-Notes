## 2D Rotations
All coordinates in the matrix are rotated by an angle $\theta$ around the origin

$$
\begin{align}
x' &= x\cos {\theta} + y \sin {\theta} \\
y' &= x\sin {\theta} + y \cos {\theta} \\
\end{align}
$$
In matrix form 

$$
\begin{bmatrix}
x' \\ y' 
\end{bmatrix}
= 
\begin{bmatrix}
\cos {\theta} & \sin {\theta} \\
\sin {\theta} & \cos {\theta}
\end{bmatrix}
\times
\begin{bmatrix}
x \\ y
\end{bmatrix}
$$