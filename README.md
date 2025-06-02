# Solving Travler salesman problem
A **Genetic Algorithm (GA)** is a type of **evolutionary algorithm**, which belongs to the broader class of **metaheuristic optimization algorithms**. It is a stochastic, population-based optimization algorithm inspired by natural evolution.
<br/>
#### The process:

**Genetic Algorithm** starts by initializing a random population of candidate solutions, then repeatedly evaluates their fitness, selects the fittest individuals as parents, applies crossover and mutation to generate new offspring, and replaces the old population with the new one, continuing this process until a termination condition is met, at which point the best solution found is returned.

It's ideal for **complex, large, or poorly-understood** problems where exact methods are inefficient or inapplicable.
<br/>

#### Terminology in GA algo
  * Selection
  * Cross-over
  * Mutattion
- - - -

**A Ant Colony Optimization (ACO)** algorithm is a type of **swarm intelligence algorithm**, which belongs to the broader class of **metaheuristic optimization algorithms**. It is a probabilistic, population-based algorithm inspired by the foraging behavior of real ant colonies.
<br/>
#### The process:

**Ant Colony Optimization** begins by deploying a number of artificial ants that iteratively build solutions by moving through the problem space. During this process, they deposit virtual pheromones on components of good solutions. Over time, paths with stronger pheromone concentrations are more likely to be chosen, guiding future ants toward better solutions. This iterative process continues until a stopping condition is met, at which point the best solution found is returned.

It's ideal for **combinatorial and graph-based problems** such as the **(TSP), routing, scheduling,**  and other optimization tasks where solution quality depends on exploring paths efficiently.
<br/>

### Terminology in ACO algo
  * Pheromone
  * Heuristic information
  * Pheromone evaporation
