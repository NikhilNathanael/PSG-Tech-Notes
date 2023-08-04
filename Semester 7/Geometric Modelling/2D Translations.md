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
