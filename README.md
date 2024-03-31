# Reinforcement Learning Algorithms Comparison in Wind Grid Environment

## Introduction
Reinforcement learning (RL) algorithms like SARSA and Q-Learning are widely used in AI problem-solving. This report compares their performance in a wind grid environment, analyzing two action spaces: normal grid (4 actions) and extended grid (8 actions with king's moves).

## Problem Formulation
The problem aims to find an optimal policy in a wind grid environment using SARSA and Q-Learning. The environment is a grid world with discrete states and actions, maximizing agent reward while navigating.

## Problem Statement
- **Objective:** Find optimal policy using SARSA and Q-Learning.
- **Comparison:** Evaluate performance in terms of total reward, convergence episodes, and handling of action spaces (4 vs. 8 actions).

## Pipeline Steps
1. **Initialization:** Set up environment and agents.
2. **Hyper-parameter Tuning:** Define alpha and epsilon ranges, store best parameters.
3. **SARSA Algorithm:** Run SARSA with varied parameters, analyze results.
4. **Q-Learning Algorithm:** Run Q-Learning with optimized parameters.
5. **Results Analysis:** Compare SARSA and Q-Learning, visualize policies, plot convergence.

## Insights
### Normal Grid World (4 Actions)
- **SARSA:** Optimal: Gamma=1, Epsilon=0.15, Alpha=0.5. Convergence: 15 episodes, Total Reward: -9.
- **Q-Learning:** Optimal: Epsilon=0.1, Alpha=0.5. Convergence: 15 episodes, Total Reward: -9.
- **Comparison:** Q-Learning outperforms SARSA in total reward and convergence.

### King’s Moves (8 Actions)
- **SARSA:** Optimal: Gamma=1, Epsilon=0.25, Alpha=0.5. Convergence: 15 episodes, Total Reward: -12.
- **Q-Learning:** Optimal: Gamma=1, Epsilon=0.05, Alpha=0.5. Convergence: 15 episodes, Total Reward: -8.
- **Comparison:** SARSA has fewer steps in King's Moves, while Q-Learning converges faster.

## Conclusion
Q-Learning generally outperforms SARSA in total reward and convergence speed. SARSA may take fewer steps. Q-Learning with 8 actions yields better results than 4 actions. Choosing RL algorithms and action spaces depends on problem characteristics.

