---
Filetype : "Derivation"
Subject : "Finite Element Analysis"
---
# Derivation of Stress

Force Matrix is given by 
$$
\begin {align*}
F &= KQ = \begin{bmatrix} F_{x_1} & F_{x_2} & F_{y_1} & F_{y_2} \end {bmatrix}
\end {align*}
$$

$$
\begin {align*}
\sigma &= E\varepsilon = E \dfrac {q_2' - q_1} {l_e} \\
\sigma &= \dfrac {E} {l_e}  \begin{bmatrix} -1 & 1 \end{bmatrix} Q' 
= \dfrac {E} {l_e} \begin{bmatrix} -1 & 1 \end{bmatrix} L Q \\
\sigma &= \dfrac {E} {l_e}  \begin{bmatrix} -1 & 1 \end{bmatrix} 
\begin{bmatrix} l & m & 0 & 0 \\ 0 & 0 & l & m \end{bmatrix} Q \\
\sigma &= \dfrac {E} {l_e}  \begin{bmatrix} -l & -m & l & m \end{bmatrix} Q
\end {align*}
$$