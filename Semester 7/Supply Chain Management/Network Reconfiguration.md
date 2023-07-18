---
Filetype : Notes
Subject : "Supply Chain Management"
---
## Warehousing Costs
- Handling Costs
	- Labor and utility costs
	- Proportional to annual flow through the warehouse
- Fixed Costs
	- All cost components not proportional to the amount of flow
	- Typically proportional to warehouse size (capacity) but in an non-linear way
- Storage Costs
	- Inventory holding costs
	- Proportional to average positive inventory levels

Estimating warehouse costs is fairly easy while estimating the other tow costs value is quite difficult

The amount of space needed by a warehouse needs to account for its peak inventory

## Typical Network Design Model
### Solution Techniques
- Mathematical optimization techniques
	1. Heuristics :Find "Good" Solutions, not necessarily optimal
	2. Exact Algorithms : Find optimal solutions
- Simulation models 

![[Problems/Problem 1]]

![[Problems/Problem 2]]
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


# Steps to solve network problem as an LPP
1. Draw the network diagram and all of its flows
2. Describe the problem mathematically
    - $0(P_1W_1) + 4(P_2W_1) + 3 (W_1C_1) + 4(W_1C_2) + 5 (W_1C_3) + 5(P_1W_2) + 2(P_2W_2) + 2(W_2C_1) + 1(W_2C_2) + 2(W_2C_3)$
-  Subject to 
  - $(P_1W_1)+(P_1W_2) \le 200000$
  - $(P_2W_1)+(P_2W_2) \le 60000$
  - $(W_1C_1) + (W_2C_1) \ge 50000$
  - $(W_1C_2) + (W_2C_2) \ge 100000$
  - $(W_1C_3) + (W_2C_3) \ge 50000$

![[Problems/Problem 3]]