# Bayesian Optimization Examples

This repository contains a collection of Jupyter notebooks demonstrating various Bayesian optimization techniques for learning purposes. Bayesian optimization is a powerful approach for optimizing black-box functions, particularly when function evaluations are expensive or time-consuming.

## Overview

Bayesian optimization is a sequential design strategy for global optimization of black-box functions that doesn't require derivatives. It's particularly useful for:
- Hyperparameter tuning in machine learning
- Experimental design
- Optimizing complex simulations
- Any optimization problem where evaluations are expensive

## Notebooks

This repository includes three example implementations:

### 1. Standard Bayesian Optimization (`bayes-opt.ipynb`)
- Implementation using Expected Improvement (EI) acquisition function
- Gaussian Process surrogate model with Matérn kernel
- Step-by-step visualization of the optimization process
- Demonstrates the balance between exploration and exploitation

### 2. q-Expected Improvement (`q-EI.ipynb`)
- Parallel Bayesian optimization using qLogNoisyExpectedImprovement
- Implementation with BoTorch library
- Batch sampling for efficient optimization
- Optimization of a randomly generated 2D function

### 3. Thompson Sampling (`thompson-sampling.ipynb`)
- Parallelized Bayesian optimization via Thompson sampling
- Exploration-exploitation trade-off through posterior sampling
- Visualization of convergence to global optimum
- Demonstrates how uncertainty decreases over iterations

## Key Concepts

The notebooks demonstrate several key concepts in Bayesian optimization:

1. **Surrogate Models**: Using Gaussian Processes to model the unknown objective function
2. **Acquisition Functions**: Strategies to determine the next evaluation points
3. **Exploration vs. Exploitation**: Balancing between exploring uncertain regions and exploiting promising areas
4. **Batch Optimization**: Methods to propose multiple evaluation points simultaneously
5. **Convergence**: How the algorithm converges to the global optimum over iterations

## Requirements

To run these notebooks, you'll need:

```
numpy
scipy
matplotlib
scikit-learn
torch
botorch
gpytorch
seaborn
jupyter
```

You can install the required packages using:

```bash
pip install numpy scipy matplotlib scikit-learn torch botorch gpytorch seaborn jupyter
```

## Usage

Clone this repository and run the Jupyter notebooks:

```bash
git clone <repository-url>
cd bayes-opt
jupyter notebook
```

Each notebook is self-contained and includes explanations alongside the code.

## Learning Resources

If you're new to Bayesian optimization, here are some recommended resources:

1. [A Tutorial on Bayesian Optimization](https://arxiv.org/abs/1807.02811) by Peter I. Frazier
2. [Practical Bayesian Optimization of Machine Learning Algorithms](https://proceedings.neurips.cc/paper/2012/file/05311655a15b75fab86956663e1819cd-Paper.pdf) by Jasper Snoek, Hugo Larochelle, and Ryan P. Adams
3. [Taking the Human Out of the Loop: A Review of Bayesian Optimization](https://ieeexplore.ieee.org/document/7352306) by Shahriari et al.

## License

This project is intended for educational purposes. Feel free to use and modify the code for your own learning.
