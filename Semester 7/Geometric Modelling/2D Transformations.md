---
Filetype: "Notes"
Subject: "Geometric Modelling"
---
# 2D Transformations
- Basic 2D transformations
- Matrix representation
- Composite Transformation
- Computational Efficiency
- Homogeneous representation
- Matrix composition

The 3 basic transformations in 2D are [[2D Translations|Translations]], [[2D Scaling|Scaling]], and [[2D Rotations|Rotations]]
## 2D Translations
A Translation can be made by adding an offset value to each coordinate

$$
\begin{align}
x' &= x + t_x \\
y' &= y + t_y 
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
x \\ y
\end{bmatrix}
+ 
\begin{bmatrix}
t_x \\ t_y
\end{bmatrix}
\end{align}
$$

Unlike other transformation matrices which are multiplied to the coordinates, the translation matrix is added to the coordinates. A composite matrix involving all three types of transformations cannot be created in this form, so the translation matrix needs to be converted into a multiplicative matrix. To do this, an extra coordinate named $h$ which is always equal to 1 is added to both coordinate matrices

$$
\begin{align}
(x,y) &=> (x, y, h) = (x, y, 1) \\
(x',y') &=> (x', y', h) = (x', y', 1)
\end{align}
$$

The translation matrix can be multiplied with this extra coordinate to 

- [ ] Finish this Explanation


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
