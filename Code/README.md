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
