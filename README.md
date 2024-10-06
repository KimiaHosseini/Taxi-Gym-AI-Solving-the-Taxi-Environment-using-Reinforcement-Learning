# Taxi-Gym-AI-Solving-the-Taxi-Environment-using-Reinforcement-Learning

## Introduction

The Taxi-v3 environment is a simple grid-based environment where a taxi must pick up a passenger from a random location and drop them off at a designated destination. The taxi must navigate through a 5x5 grid and can take six actions: moving up, down, left, right, picking up the passenger, and dropping off the passenger.

The project implements and compares various reinforcement learning algorithms to solve this problem, focusing on performance metrics such as total rewards and convergence rates.
Algorithms Implemented

The following RL algorithms are implemented and compared:

#### Value Iteration:
A dynamic programming method used to calculate the optimal policy by iteratively improving the value function.

#### Policy Iteration:
Alternates between policy evaluation and policy improvement to converge on the optimal policy.

#### Q-Learning:
A model-free RL algorithm that updates the Q-values for each state-action pair based on experiences.

#### Direct Evaluation (Monte Carlo):
Evaluates policies by averaging returns from multiple runs of the same policy.

## Results

The performance of each algorithm is measured based on the total rewards achieved and the number of iterations required to converge. Detailed results are presented in the notebook, including:

#### Convergence Rates: How quickly each algorithm converges to an optimal solution.
#### Total Rewards: The cumulative reward obtained by the agent during training.

## Comparison of Algorithms

#### Value Iteration:

Fast convergence for smaller state spaces.
Requires knowledge of the environment's dynamics (transition probabilities).

#### Policy Iteration:

Alternates between policy evaluation and improvement.
Slower convergence but guarantees optimal policies under certain conditions.

#### Q-Learning:

Model-free, does not require knowledge of the environment.
Balances exploration and exploitation but may require tuning of the learning rate and epsilon for optimal performance.

#### Direct Evaluation:

Uses experiences from Monte Carlo simulations.
Suitable for problems where the environment's model is unavailable, but slower in performance compared to the above methods.
