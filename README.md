# Bandit-algorithm-in-stock-selection
Use bandit algorithm to train an agent that can do investment like human being

## Problem setting
View the stock recommendation as an interactive recommendation problem because the goal is to maximize the total reward over a long sequence of stock operations.

## The question is
1. How do we track the performance of the stock?
2. How do we define the reward of a recommending stock based on its feedback?
3. Which bandit algorithm should we use to achieve the maximum reward in the long run?

## Strategy
- Epsilon greedy: In each trial, this algorithm first estimates the average payoff of each arm. Then it selects the highest empirical mean with probability (1 - epsilon) and selects a random arm with probability (epsilon).

- Upper Confidence Bounds (UCB): Like epsilon greedy, UCB don't keep track of how much they know about any of the arms available to them. They only pay attention to how much reward they get from the arms. In each trail, the algorithm determines the mean payoff of each arm and a corresponding confidence interval so that |mean payoff - payoff| < corresponding confidence interval holds with high probability. UCB selects the arm which has the maximum upper confidence bound.

- Contextual bandits: The algorithm chooses an action from the arms set based on the given context, then receives a reward. The goal of an algorithm is to maximize its total reward.

## Goal
Train your algo to maximum long-term rewards
