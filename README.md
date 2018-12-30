# JupyterTSP
TSP intance problem eil101,,The shortest path among all given cities (101 city) using Hill Climbing algorithm.

dist is the array of the distances ... each cell represent the distance between two cities , #for example to find the distance between city 2 and 7, we call the row index number 2 and the column index 7
``` Python 
dist[2][7] 
```
The initial solution should be a list of all cities (from 0 to 100), but we always should start from city 0 and end up at city 0 too .
 for example (this example will have only 6 cities to explin the problem):
 ``` python
TSPsol = [0, 3, 5, 4, 2, 1]
```
# to alculate the toal distance between these cities:
``` python
total_distance = dist[0][3] + dist[3][5] + dist[5][4] + dist[4][2] + dist[2][1] + dist[0][3] + dist[1][0]
```
# My code cotain the following classes :
getSolutionQuality: this class will take a TSP solution as alist and return its quality (total distances) ...


getRandomSolution: this class to creat a random solution (random list of cities from 0 to 100)...



Hill climbing algorithm : this class will take a TSP solution as an input and return the final solution
after conducting a 100,000 iteration.
 - Hill climbing Algorithm : 
--- 
random solution x
calculate the quality of x ->f(x)
best = f(x)
while i < iteration:
    generate new solution x`
    calculate the quality of x` ->f(x`)
    if f(x`)<f(x):
        replace solution list
        replace quality
        if new quality < best:
            best = new quality
            ---
            
            
# In the main body :

I call the classes and display the final solution quality and the final solution list. In addition,  I calculated the total time of the code .. 
 
