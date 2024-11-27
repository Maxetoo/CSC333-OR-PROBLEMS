# Maximizing and Minimizing Linear Programming Problems

This repository contains Python code for solving linear programming problems involving maximizing profits and minimizing costs for a manufacturing process. The problems involve various constraints such as labor, material, machine time, and product profits/costs.

## Table of Contents

- [Overview](#overview)
- [Methodology](#methodology)
- [Instructions](#instructions)
- [Visualizing the Solution](#visualizing-the-solution)




## Overview

This project solves the following optimization problems using linear programming. In each case, the problems are modeled as linear programming problems, where an objective function is maximized or minimized subject to several constraints.



## Methodology

The methodology for solving these linear programming problems involves the following steps:

1. **Define the Objective Function**  
   The first step is to define the objective function, which represents the goal of the optimization (e.g., maximizing profit or minimizing cost). This is usually a linear function of the product quantities.

2. **Set Constraints**  
   The next step is to define the constraints. These constraints limit the possible solutions and are typically related to available resources like labor, material, or machine time. These are expressed as linear inequalities.

3. **Linear Programming Solver**  
   We use the `linprog` function from the `scipy.optimize` library to solve the linear programming problems. The `linprog` function minimizes a linear objective function subject to constraints. For maximization problems, the objective function is negated to convert the problem into a minimization problem.

4. **Interpret the Results**  
   Once the problem is solved, the output provides the optimal quantities of products to produce, along with the maximum or minimum value of the objective function.

5. **Visualize the Solution**  
   We use `matplotlib` to plot the feasible region and highlight the optimal point that satisfies the constraints.

---

## Instructions

### Install the Required Libraries

Before running the code, you need to install the required libraries. You can do this using `pip`:

```bash
pip install numpy matplotlib scipy pandas
```

### Visualizing the solution


Each problem includes a graphical representation of the feasible region. The feasible region is the area where all constraints are satisfied, and the optimal solution lies within this region. The graph includes:

Feasible Region: Shaded area where all constraints are satisfied.
Optimal Point: Marked on the graph to show the optimal values of products A and B (or X and Y).
The matplotlib library is used to create graphs that visualize the feasible region and highlight the optimal solution. Each constraint is plotted as a line, and the feasible region is the area where all these lines intersect.



