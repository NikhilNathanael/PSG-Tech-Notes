#SupplyChainManagement 
[[0 Refrigeration and Air Conditioning Index]]
### Warehousing Costs
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

#### Problem 1

Two Plants $P_1$ and $P_2$, two warehouses $W_1$, $W_2$ and three customers $C_1$, $C_2$, $C_3$ have the following price matrix.
Find the best way to distribute the goods

|   | $P_1$|$P_2$|$C_1$|$C_2$|$C_3$|
|---|-|--|--|--|--|
|$W_1$|0|4|3|4|5|
|$W_2$|5|2|2|1|2|

![[Attachments/Problem 1 2023-07-11 10.04.18.excalidraw]]

### Network Diagram
![[Attachments/Network Reconfiguration 2023-07-13 11.08.34.excalidraw]]
