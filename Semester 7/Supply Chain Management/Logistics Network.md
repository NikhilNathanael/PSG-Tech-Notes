---
Filetype : Notes
Subject : "Supply Chain Management"
---

# Network Planning

Three hierarchical Steps

- Network Design
  - Number and locations of manufacturing plants, warehouses
  - Assignment of retail outlets to warehouses
  - Major Sourcing decisions
- Inventory Positioning
  - Identifying stocking points
  - Selecting facilities that will produce to stock and thus keep inventory
  - Facilities that will produce to order and hence keep no inventory
  - Related to the inventory management strategies
- Resource Allocation
  - Determine whether production and packaging of different products is done at the right facility
  - What should be the plants' sourcing strategies?
  - How much capacity each plant should have to meet seasonal demand

## Network model terminology
- Node
      Points (Warehouses, factories, Retail outlets
- Edge
    Connections between nodes
- Network
    Collection of Nodes and Edges

## Network Design Tools
- Mapping
  Mapping allows you to visualize your supply chain and solutions
  Mapping allows you to better understand different scenarios
  Color-coding, sizing, and utilization indicators allow you for further analysis
- Data 
  Input data specifies the costs of the supply chain
  Cost data should match accounting data
  Output data quantifies changes to the supply chain
- Engine
  Optimization techniques used

## Types of network problems in SC
- Shortest Path
  - It is the shortest route from node i to node j
- Travelling salesman
  - It is the shortest route that visits each node exactly once
- Vehicle Routing
  - Least cost sets of tools for vehicle to distribute products from a source node to other demand nodes 
  - The algorithm used plays a major role in the output
- Minimum Cash flow
  - What are the least cash flow of a commodity that fulfills demand at certain sink nodes and does not exceed supply at certain source nodes

## Network Design: Key Issues
- Pick the optimal number, location, and size of warehouses and/or plants
- Determine Optimal Sourcing Strategy
  - Which plant/vendor should produce which product
- Determine Best distribution channels
  - Which warehouses should service which customers

## Types of Network Design Decisions

- Strategic
  - Capital Investment
  - No. of facilities
  - Size of plants
  - Size of Distribution centers
  - Acquisition of new production equipment
  - work center decision of plant
  - Design of transport facilities, communication data processing
- Tactical 
  - Allocation of resources
  - Work force size
  - Inventory policies
  - Defining distribution channel
  - Selection of mode of transportation
- Operational
  - Day-to-Day Operations
  - Assignment of customer order to individual
  - Dispatching, expediting processing order
  - Vehicle scheduling

# Logistics Network
- It is a network used to move goods from their raw state through production and to customers
- to create the most efficient and effective logistics networks, businesses must use logistics network modeling

## Objective
- To design or reconfigure the logistics networks, so as to minimize annual system wide costs, such as production costs, purchasing costs, subject to a variety of service level requirements

# Steps to perform Network Design
 - Data Collection
 - Data Aggregation
 - Transportation Rate
 - Mileage Estimation
 - Warehouse Costs
 - Warehouse Capacities
 - Potential Warehouse Locations
 - Service Level Requirements
 - Future Demand
 - Model and Data Validation

## Data Collection
- A typical network configuration involves a large amount of data
  - Locations of customers, retailers, warehouses, factories, suppliers etc.
  - All available products and their annual demands
  - Transportation costs
  - Warehousing costs
## Data Aggregation
- All these sources create too much data to be handled easily

- Customers located in close proximity to each other can be aggregated using a **grid network**, or **Clustering Techniques**
- All customers within a single cell or a single cluster are replaced by a single customer located at the geographic center of the cell
- Each cell is called a customer zone

### Impact of Aggregating customers
The customer zone balances 
- Loss of accuracy due to over aggregation 
- needless compexity
What affects the efficiency of the aggregation?
- The number of aggregated point, i.e. the number of different zones
- The distribution of customers in each zone

### Why Aggregate
- Reduces the cost of obtaining and processing data
- Changes the form in which data is available to a more palatable form
- Decreases the size of the resultant model
- Increases the accuracy of the forecast demand

### Recommended approach
- Use at least 300 aggregated points per zone
- Make sure each zone has a similar amount of demand
- Place the aggregated point at the center of the zone

### Product Grouping
- Companies may have hundreds or thousands of individual products for sale
- Collecting data for all the products may be impractical

#### Strategy for Product Aggregation
- Place all SKUs into a source-group
  - A source group is a group of SKI's all sourced from the same place
- Within each of the source groups, aggregate the SKUs by similar logistical characteristics
  - Weight
  - Volume
  - Holding Cost


## Transportation Rates
- Constructing an effective network design model is to estimate transportation costs
- Distinguish between transportation cost associated between internal fleets and external fleets
- Estimation of internal costs includes
  - Annual Cost/truck
  - Annual mileage/truck
  - Annual amount delivered
  - Truck's effective capacity
- Incorporating transportation costs for an external fleet is more complex and is separated into two categories
  - Full Truck Load
    - Each truck carries one shipment
    - The journey is reserved
  - Less than Full Truck Load
    - Each truck carries multiple items
    - Each shipment is arranged on a pallet and placed in the truck

## Mileage Estimation
- Estimate $\text{lon}_a$ and $\text{lat}_a$, the longitude and lattitude of point a (and similarly for point b) 
- Distance between a and b
  - For short distances
    - $D_{ab} = 69 \sqrt((\text{lon}_a-\text{lon}_b)^2 + (\text{lat}_a - \text{lat}_b)^2)$
  - For Long Distances
- Circuity Factor, $\rho$ 
  - Equations underestimate the actual road distance
  - Multiply $D_{ab}$ by $\rho$ 
  - Typical Values
    - Metropolitan areas
      - $\rho = 1.3$ 
    - Continental United States
      - $\rho = 1.14$ 
## Warehouse Costs
- Handling Costs
  - Labour and utility Costs
  - Proportional to Annual Flow through the warehouse
- Fixed Costs
  - All cost components not proportional to the amount of flow
  - Typically proportional to warehouse size, but is non-linear
- Storage Costs
  - Inventory holding costs 
  - Proportional to average positive inventory levels

## Warehouse Capacities
- Estimating Warehouse cost is fairly easy while estimating the other two cost values is quite difficult
- **The amount of space a warehouse needs $\propto$ Peak Inventory** 
- Inventory Turnover Ratio
  - $IT = \dfrac{\text{Annual Sales}}{\text{Avereage Inventory Level}}$
- We typically multiply the average storage level by a factor (> 1) 
  - This factor depends on the specific application and allows users to assess the amount of space available in the warehouse more accurately
  - A typical value for the factor is **3**. 

## Potential Warehouse Locations
- Geographical and Infrastructure conditions
- Natural resources and labor availability
- Local industry and Tax regulations
- Public Interest
- Not many will qualify based on all the above conditions

## Service Level Requirements
- Specify a maximum distance between each customer and the warehouse serving them
- A proportion of customers whose distance to their assigned warehouse is no more than a given distance

### Impact of Increasing the number of warehouses
- Improve service level due to reduction of average service time to customers
- Increase inventory costs due to a larger safety stock
- Increase overhead and set-up costs
- Reduce transportation costs in a certain range
  - Reduce outbound transportation costs
  - Increase inbound transportation costs

### Industry benchmarks
- High Margin Products
  - Low number of warehouses
  - Service not important
  - Inventory expensive relative to transportation
  - Example: Pharmaceuticals
- Low Margin Products
  - High number of warehouses
  - Service quality very important
  - Outbound Transportation costs expensive compared to inbound
  - Example: Chemical Supplies

## Future Demand 
- Strategic Decisions have to be valid for 3-5 year sin advance
- Consider scenario approach and net present values to factor in expected future demand over planning horizon

## Model Validation
- Reconstruct the existing network configuration using the model and collected data
- Compare the output of the model to existing data
- Compare to the company's accounting information
  - Often the best way to identify errors in the data, problematic assumptions, modeling flaw. 
- Make local or small changes in the network configuration to see how the system estimate impact on costs and service levels
  - Positing a variety of what-if questions?
    - Does the model make sense?
    - Are the data consistent?
    - Can the model results be fully explained?
    - Did you perform sensitivity analysis?






















