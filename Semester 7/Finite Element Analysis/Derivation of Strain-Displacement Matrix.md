[[0 Finite Element Analysis Index]]
Displacement Function 
$$U=N_1 q_1 + N_2 q_2 + N_3 q_3$$ 

$$
u_i = N_i q_i
$$
Strain $\epsilon = \frac {du}{dx} (N_i q_i) = \frac {dN}{d\epsilon}, q^e = \frac {d}{d\epsilon} (N_1, N_2, N_3) q^e$

$$
\begin{align*}
\frac {du}{d\epsilon} &= [\frac{-1(1-2\epsilon)}{2}, \frac{-1(1-2\epsilon)}{2}, -2\epsilon] \cdot q^e \\

\end{align*}
$$
$$
\begin{align*}
K_{11} &= \frac {AEl_e}{2} \int^1_{-1} {\left[\frac {-1(1-2\epsilon)}{2}\right] \left[\frac {-1(1-2\epsilon)}{2}\right]d\epsilon \times (\frac {2}{l_e})^2}
\\
&= \frac {AEl_e}{2} \int^1_{-1} {\frac{1}{4} (1-2\epsilon)^2 d\epsilon \times (\frac {2}{l_e})^2} 
\\
&= \frac {AE}{2l_e} \int ^1_{-1} {(1-4\epsilon +4\epsilon^2) d\epsilon}
\\
&=\frac {AE} {2l_e} \left[\epsilon -2\epsilon^2 + \frac {4\epsilon^3} {3}\right] ^1_{-1}
\\
&=\frac {AE} {2l_e} \left(\left(1-2+\frac {4}{3}\right) -\left(-1-2-\frac {4}{3}\right)\right)
\\
K_{11} &= \frac {AE} {2l_e} \left(2+\frac {8}{3}\right)
\\
K_{11} &= \frac {7}{3} \cdot \frac {AE}{l_e} 
\end{align*}
$$
Apply this procedure to all elements in the matrix 

$$
[K] = \frac {AE} {3l_e} \left[\matrix {7&1&-8\\1&7&-8\\-8&-8&16}\right]
$$

#### Problem 1
![[Problem 1.excalidraw]]