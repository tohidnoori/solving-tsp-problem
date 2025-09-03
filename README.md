# Solving Travler salesman problem

This project compares two metaheuristics for solving the **Travelling Salesman Problem (TSP)**:
- **Genetic Algorithm (GA)**
- **Ant Colony Optimization (ACO)**

The algorithms were tested on several problem instances. Each instance was defined by an adjacency matrix (from `in.txt`), where `-1` denotes no direct path.

## Genetic Algorithm (GA)

A **Genetic Algorithm (GA)** is a type of **evolutionary algorithm**, which belongs to the broader class of **metaheuristic optimization algorithms**. It is a stochastic, population-based optimization algorithm inspired by natural evolution.

---

#### The process:

**Genetic Algorithm** starts by initializing a random population of candidate solutions, then repeatedly evaluates their fitness, selects the fittest individuals as parents, applies crossover and mutation to generate new offspring, and replaces the old population with the new one, continuing this process until a termination condition is met, at which point the best solution found is returned.

It's ideal for **complex, large, or poorly-understood** problems where exact methods are inefficient or inapplicable.

---

#### Terminology in GA algo
  * Selection
  * Cross-over
  * Mutattion

---

#### Parameters
- Uses **elitism**, **ordered crossover**, and **swap mutation**.
- Population size: `100`
- Generations: `300`
- Mutation rate: `0.1`

---
## Ant Colony Optimization (ACO)

**A Ant Colony Optimization (ACO)** algorithm is a type of **swarm intelligence algorithm**, which belongs to the broader class of **metaheuristic optimization algorithms**. It is a probabilistic, population-based algorithm inspired by the foraging behavior of real ant colonies.

---
#### The process

**Ant Colony Optimization** begins by deploying a number of artificial ants that iteratively build solutions by moving through the problem space. During this process, they deposit virtual pheromones on components of good solutions. Over time, paths with stronger pheromone concentrations are more likely to be chosen, guiding future ants toward better solutions. This iterative process continues until a stopping condition is met, at which point the best solution found is returned.

It's ideal for **combinatorial and graph-based problems** such as the **(TSP), routing, scheduling,**  and other optimization tasks where solution quality depends on exploring paths efficiently.

---


#### Terminology in ACO algo
  * Pheromone
  * Heuristic information
  * Pheromone evaporation

---

#### Ant Colony Optimization (ACO)
- Parameters:
  - `alpha = 1` (pheromone importance)
  - `beta = 5` (visibility importance)
  - `evaporation = 0.5`
  - `Q = 100` (pheromone reinforcement factor)
- Number of ants: `20`
- Iterations: `100`
---
## TSP Solvers: Genetic Algorithm vs. Ant Colony Optimization

- **Both GA and ACO found optimal solutions** (same tour length in all problems).
- **ACO consistently ran faster** than GA in these test cases.
- **GA** has more exploration power (due to population evolution) but is slower.
- **ACO** leverages pheromone trails and visibility, achieving strong performance quickly.

