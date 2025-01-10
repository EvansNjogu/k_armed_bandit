# k-Armed Bandit Problem

The k-armed bandit problem is a classic reinforcement learning task where an agent repeatedly chooses from `k` different options (actions) to maximize the total reward received over a period of time. Each action corresponds to a stationary probability distribution of rewards, and the agent must balance **exploration** (trying new actions to learn more about them) and **exploitation** (choosing the known best action).

## Problem Description

You are faced repeatedly with a choice among `k` actions. Each action provides a numerical reward drawn from a stationary probability distribution. The goal is to maximize the total expected reward over a sequence of steps.

This problem illustrates the trade-off between:
- **Exploration**: Trying less-optimal actions to gather information.
- **Exploitation**: Choosing the current best-known action to maximize reward.

## Algorithms Implemented

### 1. ε-Greedy Action Selection
The ε-greedy algorithm balances exploration and exploitation:
- With probability **1 - ε**, the agent selects the action with the highest estimated value.
- With probability **ε**, the agent selects a random action.

### 2. Gradient Bandit Algorithm
This algorithm learns preferences for actions rather than directly estimating their value. The probability of selecting each action is determined using a **softmax function**.

## References

- Sutton, R. S., & Barto, A. G. (2018). *Reinforcement Learning: An Introduction*. (Chapter 2)
- [k-Armed Bandit Problem on Wikipedia](https://en.wikipedia.org/wiki/Multi-armed_bandit)

