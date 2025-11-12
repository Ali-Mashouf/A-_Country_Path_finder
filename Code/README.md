# Graph 
____Graph is defined as a dictionary____

____Each key is a country name____

____Each value is a list of tuples representing neighbors and the cost to reach them____

<img width="1389" height="989" alt="image" src="https://github.com/user-attachments/assets/27e29327-cdcd-44ed-bc24-f854ea307065" />


# Heuristic Function
____Estimated cost from each country to the goal country____

____Zero for Iran (since it's the starting point)____

____These values help the algorithm prioritize promising paths____

# A_star Function

* *graph: Graph structure*

* *heuristic: Heuristic cost function*

* *start: Starting point (Iran)*

* *goal: Target point (user input)*

## Priority Queue (PriorityQueue)

____Elements are sorted based on priority____
* *Priority = Actual Cost + Estimated Cost*

## Path Storage (W_node)
____Used for path reconstruction____

____Stores which node we came from to reach the current node____

## Costs (S_cost)
____Actual cost to reach each node from the start____

* *Zero for the start node*

## Algorithm Steps
1. Initialization
Start node is placed in the queue with zero cost

2. Main Loop
Continues until the queue is empty

The node with the lowest priority is removed from the queue

3. Goal Check
If we reached the goal, we reconstruct the path

We reverse the path to go from start to goal

4. For each neighbor:
We calculate the new cost

If it's better than the previous path:

We update the cost

We calculate the priority

We place it in the queue

We store the path
