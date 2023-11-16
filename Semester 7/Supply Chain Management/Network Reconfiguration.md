---
Filetype : Notes
Subject : "Supply Chain Management"
---
## Typical Network Design Model
### Solution Techniques
- Mathematical optimization techniques
	1. Heuristics : Find "Good" Solutions, not necessarily optimal
	2. Exact Algorithms : Find optimal solutions
- Simulation models 

![[Problems/Problem 1]]

# Problem 2
### Network Diagram
![[Attachments/Formulating LPPs.excalidraw]]

The formulated LPP is 
Minimize 
$$\begin{align*}
Z = 0x_1 + 4x_2 + 5y_1 + 2y_2 + 3u_1 + 2u_2 + 4v_1 + 1v_1 + 5w_1 + 2w_2)
\end{align*}$$
Subject to
$$\begin {align*}
x_1 + x_2 \le 200000\\
y_1 + y_2 \le 60000\\
u_1 + u_2 \ge 50000\\
v_1 + v_2 \ge 100000\\
w_1 + w_2 \ge 50000
\end {align*}$$


![[Problems/Problem 3]]

## Simulation Models
- Useful for a given design and a micro-level analysis. Examine
  - Individual Ordering pettern.
  - Specific inventory policies
  - Inventory movements inside the warehouse
- **Not and Optimization Model**
- Can only consider very few alternate models

## Which model to use?
- Use Mathematical Optimization for static analysis
- Use a 2-step approach when dynamics in a system needs to be analysed