# Bandit-algorithm-in-stock-selection
Use bandit algorithm to train an agent that can do investment like human being

## Problem setting
View the stock recommendation as an interactive recommendation problem because the goal is to maximize the total reward over a long sequence of stock operations.

## The question is
1. How do we track the performance of the stock?
2. How do we define the reward of a recommending stock based on its feedback?
3. Which bandit algorithm should we use to achieve the maximum reward in the long run?

## Strategy
- Epsilon greedy
- Upper Confidence Bounds (UCB)
- Contextual bandits

## Goal
Train your algo to maximum long-term rewards

## Reference
- 	[Multi-arm Bandits lecture notes](https://github.com/Alice-Huang-Xin/Bandit-algorithm-in-stock-selection/blob/main/Multi-arm%20Bandits.pptx)
- 	[Introduction to Contextual Multi-bandit Algorithm](https://github.com/Alice-Huang-Xin/Bandit-algorithm-in-stock-selection/blob/main/Introduction%20to%20Contextual%20Multi-bandit%20Algorithm.pdf)
- 	[Bandit Algorithms for Website Optimization](https://github.com/Alice-Huang-Xin/Bandit-algorithm-in-stock-selection/blob/main/Bandit%20Algorithms%20for%20Website%20Optimization%20%5BWhite%202013-01-03%5D.pdf)

## Dataset
In this [dataset](https://github.com/Alice-Huang-Xin/Bandit-algorithm-in-stock-selection/blob/main/11%20ETF%20and%20feature%20dataset.xlsx), there are 49 features including 49 US macro-economic indicators such as bond yield, SP500 return, etc. We use past 5d % and last price depending on the data type. All data comes from Bloomberg. And the stock pool consists of 11 sector ETFs. The performance used in calculation of reward is the future 5d return.

## Code
[Disjoint LinUCB algorithm](https://github.com/Alice-Huang-Xin/Bandit-algorithm-in-stock-selection/blob/main/Disjoint%20LinUCB.ipynb)

![myimage](file:///Users/xinhuang/Desktop/1.png)
