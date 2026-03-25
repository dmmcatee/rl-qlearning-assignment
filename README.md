# Reinforcement Learning with Q-Learning (FrozenLake-v1)

## Overview
This assignment explores reinforcement learning using the Gymnasium library. The goal was to train an agent to navigate the FrozenLake-v1 environment using Q-Learning, a model-free reinforcement learning algorithm. The agent learns optimal actions through trial and error by interacting with the environment and updating a Q-table.

---

## Part A: Environment Exploration
The FrozenLake-v1 environment was initialized and explored. The agent interacted with the environment by taking random actions and observing the resulting states, rewards, and termination conditions. This demonstrated how an agent receives feedback from an environment and transitions between states.

---

## Part B: Q-Learning Implementation
A Q-table was initialized with zeros, representing all possible state-action pairs. The agent was trained over multiple episodes using the Q-Learning algorithm.

Key components:
- **Learning rate (alpha):** Controls how much new information overrides old information.
- **Discount factor (gamma):** Determines the importance of future rewards.
- **Exploration rate (epsilon):** Balances exploration vs. exploitation.

The agent used an epsilon-greedy strategy to choose actions and updated the Q-table using the Bellman equation. Over time, epsilon decayed to reduce exploration and favor learned behavior.

---

## Part C: Evaluation and Visualization
The trained agent was evaluated using a greedy policy (always selecting the best-known action). Performance was measured using:
- Average reward
- Success rate (reaching the goal)

Learning progress was visualized using:
- Total reward per episode
- Moving average of rewards

Results showed that the agent improved over time, though performance was somewhat inconsistent due to the stochastic (slippery) nature of the environment.

---

## Part D: Reflection
One key challenge was the randomness and sparse rewards in FrozenLake, which slowed learning. Hyperparameters had a significant impact:
- Higher alpha increased learning speed but reduced stability
- Higher gamma improved long-term decision-making
- Epsilon decay helped balance exploration and exploitation

Reinforcement learning has practical applications in areas such as sports analytics (decision optimization), autonomous systems, robotics, and recommendation systems.

---

## Conclusion
This assignment demonstrated how Q-Learning enables an agent to learn optimal behavior through interaction with an environment. Despite challenges like randomness and sparse rewards, the agent was able to improve performance over time, highlighting the effectiveness of reinforcement learning techniques.
