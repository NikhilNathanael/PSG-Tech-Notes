---
Filetype : "Derivation"
Subject : "Finite Element Analysis"
---
# Derivation of Strain Energy

#### Assumptions
1. All joints are pin Joints
2. Loads are applied at joints
3. Self weight is ignored

![[Attachments/Trusses.jpg]]

![[Attachments/Trusses 2.jpg]]
$$
q_1' = q_1 \cos {\theta} + q_2 \sin {\theta}
$$
$$
q_2' = q_3 \cos {\theta} + q_4 \sin {\theta}
$$

$$
\begin{bmatrix} 
q_1' \\ q_2'
\end{bmatrix} = 
\begin{bmatrix}
\cos{\theta} & \sin {\theta} & 0 & 0 \\
0 & 0 & \cos {\theta} & \sin {\theta}
\end{bmatrix} 
\times 
\begin{bmatrix}
q_1 \\ q_2 \\ q_3 \\ q_4 
\end{bmatrix} 
$$

$$
Q' = L\times Q
$$
where
$$
L = 
\begin{bmatrix}
\cos{\theta} & \sin {\theta} & 0 & 0 \\
0 & 0 & \cos {\theta} & \sin {\theta}
\end{bmatrix} 
$$

$L$ can be rewritten as 
$$
L = 
\begin{bmatrix}
l & m & 0 & 0 \\
0 & 0 & l & m
\end{bmatrix} 
$$

where

$$
\begin{align*}
l &= \cos {\theta} = \dfrac {x_2-x_1} {l_2} \\
m &= \sin {\theta} = \dfrac {y_2-y_1} {l_2}
\end{align*}
$$

and 

$$
l_e = \sqrt {(x_2 - x_1)^2 + (y_2-y_1)^2}
$$

Strain Energy in LCS : $U_e = \dfrac {1}{2} Q'^T K' Q'$
Strain Energy in GCS : $U_e = \dfrac {1}{2} Q^T L^T K' L Q$

$K' = \dfrac {AE} {l_e} \begin{bmatrix} 1 & -1 \\ -1 & 1\end{bmatrix}$

$$
\begin{align*}
K &=  L^T K' L \\
K &= 
\begin {bmatrix}
l & 0 \\ m & 0 \\ 0 & l \\ 0 & m
\end {bmatrix}
\times \dfrac {AE} {l_e}
\begin {bmatrix}
1 & -1 \\ -1 & 1
\end {bmatrix}
\begin {bmatrix}
l & m & 0 & 0 \\ 0 & 0 & l & m
\end {bmatrix} 
\\
K &=
\dfrac {AE} {l_e} 
\begin {bmatrix}
l & -l \\ m & -m \\ -l & l \\ -m & m
\end {bmatrix}
\times 
\begin {bmatrix}
l & m & 0 & 0 \\ 0 & 0 & l & m
\end {bmatrix} 
\\
K &= 
\dfrac {AE} {l_e}
\begin{bmatrix}
l^2 & lm & -l^2 & -lm \\
lm & m^2 & -lm & -m^2 \\
-l^2 & -lm & l^2 & lm \\
-lm & m^2 & lm & m^2 
\end {bmatrix} 
= \dfrac {AE} {l_e} B
\end{align*}
$$