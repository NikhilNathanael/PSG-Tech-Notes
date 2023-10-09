---
Filetype: "Notes"
Subject: "Finite Element Analysis"
---

Determine the temperature distribution using the length of the rod shown in fig. with an insulated perimeter. The temperature at the left end is 311K and the free stream temperature is 261 K. Let j = 57 $W/m^2K$ and $K_{xx} = 32 W/mK$. Also find the rate of heat flow through element 1.

Answer:
The problem can be idealized in 1 dimension 

$$
\begin{align}
T_{\text{left}} &= 311 K \\
T_\infty &= 261 K \\
h &= 57 W/m^2K \\
K_{xx} &= 35 W/mK \\
l &= 1.016 m \\
\phi &= 0.0051 \\
\end{align}
$$


Stiffness Matrix

$$
\begin{align}
[K] = \dfrac{AK}{l}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix}
+ \dfrac{hpl}{6} 
\begin{bmatrix}
2 & 1 \\ 1 & 2
\end{bmatrix}
+ ha 
\begin{bmatrix}
0 & 0 \\ 0 & 1
\end{bmatrix}
\end{align}
$$

No convection because of insulated perimeter
$$
\begin{align}
[K] = \dfrac{AK}{l}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix}
+ ha 
\begin{bmatrix}
0 & 0 \\ 0 & 1
\end{bmatrix}
\end{align}
$$

Force Matrix

$$
\begin{align}
[F] = \dfrac{QAl + \dot{q}Pl + hT_0Pl}{2} \begin{bmatrix} 1 \\ 1 \end{bmatrix}
+ \dot{q} A \begin{bmatrix} 0 \\ 1\end{bmatrix}
\end{align}
$$

Split into 4 elements
Element 1
No convection at end of element
$$
\begin{align}
[K] &= \dfrac{AK}{l}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix} \\

K_1 &= 
\dfrac{\dfrac{\pi}{4}(0.0051)^2 \cdot 35}{\dfrac{1.016}{4}}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix} \\
K_1 &=
\end{align} 
$$

No heat generation, flux or outflow
$$
\begin{align}
F_1 = 0 \\
F_2 = 0
\end{align}
$$

Same for Element 2, 3, and 4 

$$
\begin{align}
K_1 = K_2 = K_3 = 
\dfrac{\dfrac{\pi}{4}(0.0051)^2 \cdot 35}{\dfrac{1.016}{4}}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix} \\
F_1 = F_2 = F_3 = F_4 = 0
\end{align}
$$

Element 5 
$$
\begin{align}
[K] &= \dfrac{AK}{l}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix}
+ ha 
\begin{bmatrix}
0 & 0 \\ 0 & 1
\end{bmatrix} \\

K_4 = 

K_1 &= 
\dfrac{\dfrac{\pi}{4}(0.0051)^2 \cdot 35}{\dfrac{1.016}{4}}
\begin{bmatrix}
1 & -1 \\ -1 & 1
\end{bmatrix} 
+ 57 \cdot \dfrac{\pi}{4}(0.0051)^2 \cdot 
\begin{bmatrix}
0 & 0 \\ 0 & 1
\end{bmatrix}


\end{align}
$$




















