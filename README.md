# TSP-SA
Solving TSP problem with simulated annealing
# explanation
- solved TSP problem with simulated annealing algorithm(a half physic algorithm.) which is very good and find the best path for berlin59 dataser that the path's length is 1610.
- I put the analysis for each parameter but it is is persian.
# executation
run with python3.
# algorithm
We put each point as a permutation of all the answers, which always starts from zero. At each stage the temperature and the neighbor and probability function are updated as follows. Initially, it also creates a random permutation.
- Temperature: At each stage, the temperature is equal to (i +1) / iteration, which decreases with each iteration.
- Neighbor: Takes two cities and swaps them.
- Probability function (P): If the neighbor fit is better, he must choose it, otherwise:
‫‪p‬‬ ‫=‬ ‫‪e‬‬ ^ (‫‪|E(s‬‬ ‫‪new‬‬ ‫‪)−E(s)|/temperature)‬‬
- Energy function (E): is equal to the same fitting function in the genetic algorithm. That is, the cost of a permutation.
- End of algorithm: The algorithm terminates after iteration.
