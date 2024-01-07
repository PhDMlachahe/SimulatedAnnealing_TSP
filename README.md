<div align="center">
<h1 align="center">Simulated Annealing for the Traveling Salesman Problem (SA-TSP)</h1>

  <p align="center">
    An exploration into metaheuristics for solving the TSP with weighted neighborhood operations and multiple neighborhood operations
  </p>

</div>

## Description

The Simulated Annealing for the Traveling Salesman Problem (SA-TSP) project is an immersive journey into the captivating world of metaheuristics, focusing on the classic optimization challenge of the Traveling Salesman Problem (TSP). This project implements a simulated annealing algorithm that incorporates weighted neighborhood operations and multiple neighborhood operations to find near-optimal solutions efficiently.

Key features from the implementation:
1. 📍 **Initial Solution Generation**: A random initial solution is created by shuffling city coordinates while ensuring the start point is fixed and the route returns to the origin.
2. 📏 **Fitness Evaluation and Distance Calculation**: An efficient fitness function calculates the total route distance using a precomputed distance matrix between all city pairs, guiding the optimization process.
3. 🧬 **Advanced Neighborhood Operations**: Implements a variety of weighted operators, including swap, insert, inverse subroutes, and insert subroutes to generate neighboring solutions. These operations are applied iteratively and adjusted dynamically based on the system's temperature, enabling a nuanced exploration of the solution space.
4. 🌡️ **Cooling Schedule**: Utilizes an exponential decay function to methodically reduce the temperature, systematically decreasing the probability of accepting worse solutions over time.
5. ✔️ **Acceptance Criteria**: Probabilistically accepts new solutions based on their fitness and the system's temperature to balance exploration with the goal of finding an optimal solution.

For an in-depth understanding, refer to my articles detailing the journey and findings:
- 🇫🇷 [Sur la Route de l'Optimum: Recuit Simulé pour le TSP](https://medium.com/wanabilini/sur-la-route-de-loptimum-recuit-simulé-pour-le-tsp-9cb037e74979)

## Repository Structure

- `README.md`: This file with all the information about the project.
- `SimulatedAnnealing_TSP.ipynb`: The main Jupyter notebook with the implementation.
- `results_tsp_2024_01_04_18_26_30`: Folder with the algorithm's output results using various parameters.
- `tableau_recapitulatif.ods`: A summary table of algorithm performance across different benchmarks.

## Results

Our simulated annealing algorithm was tested against well-established benchmarks from TSPLIB. The performance metrics on benchmarks such as `ulysses22.tsp`, `berlin52.tsp`, `st70.tsp`, and `ch130.tsp` demonstrate the effectiveness of our approach.

- The results highlight the importance of selecting the right parameters for simulated annealing and neighborhood strategy.

The following graph illustrates the convergence pattern of the algorithm over iterations for a selected benchmark:

![Graph](results_tsp_2024_01_04_18_26_30/st70_with_parameters_temp_10000_max_1500_gamma_099_weights_40_30_35_5.png)

This graph depicts the algorithm's ability to reduce the total distance (cost function) over time, indicating the efficiency of our simulated annealing implementation in exploring the solution space.


## Contact #

If you have any questions or would like to connect:

- 📬 Email me at [mlachahe.saidsalimo@gmail.com](mailto:mlachahe.saidsalimo@gmail.com)
- 🟦 Connect with me on [LinkedIn](https://www.linkedin.com/in/mlachahesaidsalimo/)
- ⬛ Read my thoughts on [Medium](https://medium.com/@mlachahesaidsalimo)

