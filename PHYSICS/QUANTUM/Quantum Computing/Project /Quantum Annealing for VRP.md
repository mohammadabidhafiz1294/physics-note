  **VRP and CVRP**
 
The **Vehicle Routing Problem (VRP)** is a classic optimization problem where the goal is to find the best routes for a fleet of vehicles to deliver goods or services to a set of customers. "Best" usually means the shortest, cheapest, or fastest route.

The **Capacitated Vehicle Routing Problem (CVRP)** is a version of the VRP where the vehicles have a limited capacity, like a certain number of packages they can carry or a maximum weight limit. This adds an extra layer of difficulty to the problem.
    
**QUBO**

**QUBO**, or **Quadratic Unconstrained Binary Optimization**, is a way of framing certain problems so they can be solved by quantum computers. It involves co    nverting the problem into a mathematical equation with binary variables (0 or 1). The quantum computer then finds the solution that gives the lowest possible value for the equation, which corresponds to the best solution to the original problem.

**TSP**

The **Traveling Salesperson Problem (TSP)** is a famous problem that's a simplified version of the VRP. It involves finding the shortest possible route for a salesperson to visit a set of cities and return to their starting point.

**Metaheuristic Strategy**
A **metaheuristic** is a high-level strategy for solving difficult problems. Metaheuristic algorithms for the TSP are used to find very good, but not necessarily perfect, solutions in a reasonable amount of time. Examples include **simulated annealing**, **genetic algorithms**, and **ant colony optimization**.

**Algorithms Introduced**

- **FQS** (Full QUBO Solver): A basic quantum algorithm for solving the VRP.

-  **AVS**(Average Partition Solver): A more advanced version of FQS that makes some simplifying assumptions to reduce the complexity of the problem.

- **DBSS**(DBSCAN Solver): A hybrid algorithm that uses a classical clustering method called **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise) to group customers together before using the quantum computer to find the best routes. This can handle VRP and CVRP with equal vehicle capacities.

-  **SPS** (Solution Partitioning Solver): Another hybrid algorithm that can solve the more complex CVRP with vehicles of different capacities. It breaks the problem down into smaller pieces that are easier to solve.

**CVPRTW**

**CVRTW** stands for the **Capacitated Vehicle Routing Problem with Time Windows**. It's a more complex version of the classic "traveling salesman problem" and a critical challenge in the fields of logistics and operations research.
The main goal of the CVRTW is to find the most efficient set of routes for a fleet of vehicles to serve a group of customers. This efficiency is usually measured by minimizing the total distance traveled or the number of vehicles used.

What makes the **CVRTW particularly challenging are its specific constraints**:

- **Capacitated Vehicles:** Each vehicle has a limited carrying capacity (e.g., weight or volume of goods) and cannot be overloaded.
- **Time Windows:** Each customer must be visited within a specific time frame. A vehicle may arrive early but must wait until the time window opens to begin service. Arriving after the time window closes is not allowed.
- **Depot:** All vehicles start their routes from a central depot and must return to it after completing their deliveries.
- **Customer Demand:** Each customer has a known demand that must be met.

**Constraints**

Constraints are limitations or restrictions imposed on a system or problem, defining the feasible space or allowed configurations. They can be expressed as equations or inequalities and play a crucial role in defining the behavior of systems and solving problems.

### Quantum Annealing

**Quantum Annealing** is a metaheuristic algorithm used for finding the optimal solution to a problem. It's a method that uses the principles of quantum mechanics to guide a system towards its lowest energy state, which corresponds to the best possible solution.

Think of it like trying to find the lowest point in a vast, hilly landscape in the dark. A classical approach (like simulated annealing) would be like rolling a ball and letting it settle in the nearest valley. It might get stuck in a small, local valley and never find the absolute lowest point.

Quantum annealing, however, leverages a quantum phenomenon called **quantum tunneling**. This is like allowing the ball to "tunnel" through the hills instead of having to climb over them. This ability to pass through energy barriers gives it a better chance of exploring the entire landscape and finding the true, global lowest point (the optimal solution). Specialized computers, like those built by D-Wave Systems, are designed specifically to perform this process.

### Quantum Annealing for CRP

Quantum annealing (QA) is being explored as a promising approach to solve the Vehicle Routing Problem (VRP), a complex optimization problem with numerous real-world applications. VRPs, which involve finding the most efficient routes for a fleet of vehicles to serve a set of locations, are known to be NP-hard, making them computationally challenging for classical computers, especially as the problem size increases. Quantum annealers, like those offered by D-Wave, leverage quantum mechanical phenomena to potentially find solutions to these problems more efficiently than classical algorithms.

**BQM**
Binary Quadratic Model
A **BQM** is a way of expressing a problem using only **binary variables** (like 0/1 or -1/1) where the goal is to minimize a **quadratic** function. It's the foundational language for quantum annealers.

**CQM**
Constrained Quadratic Model
A **CQM** is a more powerful and user-friendly model. It's an evolution of the BQM that allows you to define constraints directly, making it much easier to represent complex, real-world problems.

**Quantum Approximate Optimization Algorithm (QAOA)**


**Noisy Intermediate Scale Quantum (NISQ)**

**Euclidean distance**


**NP-hardness:**
A problem is NP-hard if it is at least as hard as the hardest problems in the complexity class NP (Nondeterministic Polynomial time). In simpler terms, if you could solve an NP-hard problem efficiently, you could solve all problems in NP efficiently. However, it's generally believed that no polynomial-time algorithm exists for NP-hard problems.


---
### Paper: Graph Coarsening Approach to the Vehicle Routing Problem: An Approximation Strategy 

 🧩 **Goal of the Paper**:

To solve large **Capacitated Vehicle Routing Problems (CVRP)** **faster** by using a technique called **graph coarsening**, making it easier for both **classical** and **quantum** solvers.

 🧠 What Is the CVRP?

- A vehicle must deliver goods to multiple **customers** (nodes/vertices).
- Vehicles have a **limited capacity**.
- Objective: Minimize total **distance** while satisfying all **constraints** (e.g., every customer is visited, no vehicle exceeds its capacity).

🧱 Key Components

|Term|Meaning|
|---|---|
|**Vertex (V)**|A location (customer or depot)|
|**Edge (E)**|Road/connection between two locations|
|**Graph (G)**|Set of all vertices and edges|
|**Coarsening**|Combining nearby vertices into one to reduce graph size|
|**Inflation**|Reversing coarsening to return to original detail|
|**ILP**|Integer Linear Programming — a method for solving exact optimization problems|
|**BQM/QUBO**|Binary Quadratic Models — used in quantum computing|


**Working Process: Step-by-Step**

1. **Start with the original graph**

	Each node = a customer. Each edge = road with distance (Euclidean).
 2. **Apply Graph Coarsening**
 
	- Sort edges by distance.
	- Pick a threshold (based on radius coefficient).
	- **Merge nearby vertices** into one "super-node" if they're close enough.
	- Update the graph.
	- Repeat until number of nodes is reduced (according to coarsening rate `P`).

	🔧 _Example:_ If `C` and `D` are close → merge to `C/D`.

3. **Solving CVRP on Coarsened Graph**

	They try **two approaches**:

	A. **ILP (Gurobi Solver)** – Precise Classical

	- Use mathematical model of CVRP.
	- Finds close-to-optimal solutions.
	- Slower on large graphs.

	 B. **BQM (Quantum/Hybrid Solvers)** – Approximate

	- Converts problem to a binary form suitable for D-Wave’s **quantum annealing**.
	- Uses **Leap Hybrid Sampler** (quantum-classical) and **Neal** (simulated annealing).

> Quantum solvers struggle with large graphs → coarsening helps them a lot!

 4. **Inflation (Reverse Coarsening)**
	
	- Reconstruct original solution from coarsened one.
	- For each merged node (e.g., C/D), decide best order (C→D or D→C) to keep total cost low.

 5. **Evaluation (Experiments)**

	They use **standard datasets** (Christofides CMT01–CMT12).
	
	Results:

	- **Gurobi (ILP)**: Performs best on full (uncoarsened) graphs.
	- **Quantum (Leap/Neal)**: **Works better on coarsened graphs** → improved quality and speed.
	- **Best combination**: Use coarsening + BQM + hybrid solver.

📊 Summary of Findings

| Item                     | Result                                                                  |
| ------------------------ | ----------------------------------------------------------------------- |
| Coarsening               | Reduces graph size, helpful for large problems                          |
| ILP + Gurobi             | Precise, best on original graphs                                        |
| Quantum BQM (Leap, Neal) | Much better on coarsened graphs                                         |
| Inflation                | Recovers full routes from coarsened solution                            |
| Overall                  | Graph coarsening enables VRP solving on limited hardware (esp. quantum) |


🧩 Real-World Benefit

This method allows:
- Using **limited classical or quantum hardware** to solve big routing problems.
- Getting results **faster**, especially with quantum or hybrid solvers.
- Keeping **solution quality high** using coarsening + inflation.

### Proposal:

**Spatio-Temporal Distance** :
**Spatio-Temporal Distance** is a custom metric designed to combine both the spatial and temporal aspects of the Vehicle Routing Problem. It helps in making more intelligent decisions during the graph coarsening process.

The proposed spatio-temporal distance, denoted as

$D_(ij)$​, is calculated using the following formula:

$$D_(ij)​=α⋅τ_(ij)​+β⋅ΔT_(ij)$$​
Here's a breakdown of its components:
- **$τ_(ij)​$**: This represents the **travel time** between two points, _i_ and _j_. It can be a simple value or a function that depends on the time of day, $τ_(ij)​​(t)$.
    
- $ΔT_(ij​)$: This term measures the **temporal separation** or incompatibility  between the time windows of nodes _i_ and _j_. One way to calculate it is by  determining the waiting time, if any, at node $j$ if a vehicle travels from $i$. For example:
    $$ΔTij​=max(0,e_j​−(t_i​+s_i​+τ_$ij$​))$$         , where $e_j$​ is the earliest start time at $j$, $t_i$ is the arrival time at _i_, and $S_i$​ is the service duration at _i_.
    
	- **α and β**: These are **weighting parameters** that allow for balancing the influence of the spatial (travel time) and temporal (time window difference) components in the overall distance calculation.