# Jack's Car Rental - Policy Iteration 

This project implements the policy iteration algorithm to solve the Jack's Car Rental problem. The goal of the problem is to find an optimal policy that maximizes the profit of two car rental companies - A and B.

The problem is formulated as a Markov Decision Process (MDP), where the state is represented by the number of cars at each company at the end of a day. The action is represented by the number of cars moved from company A to B or vice versa. The reward is based on the number of cars rented out and returned to each company.

## Problem

Jack owns two car rental companies, A and B. Each day, people come to rent cars from each location. Jack has a certain number of cars available at each location, and when a customer arrives, Jack rents a car if one is available. Each location has a limit on the number of cars it can hold, so any additional cars that arrive will be turned away.

At the end of each day, Jack can move cars between the two locations to better meet demand. The cost to move a car is a fixed amount, and Jack can only move a limited number of cars each day.

Jack wants to maximize his profit, which is based on the number of rentals and returns at each location. He needs to decide how many cars to keep at each location and how many to move between the two locations each day.

## Dependencies
- numpy
- matplotlib
- seaborn
- scipy

## Usage

Run the mainLoop function in the code to execute the policy iteration algorithm. The function initializes the value and policy arrays with zeros and iteratively performs policy evaluation and policy improvement until the optimal policy is found. The final values and policies are printed to the console, and a heatmap is displayed showing the optimal value for each state.

## Parameters 

`maxCapacity`: The maximum number of cars that can be stored in each company. 

`maxCompCapacity`: The maximum number of cars that can be moved between the companies.

`discount`: The discount factor for future rewards.

`applicantA`: The mean number of customers at company A.

`applicantB`: The mean number of customers at company B.

`dispensedA`: The mean number of cars rented out at company A.

`dispensedB`: The mean number of cars rented out at company B.

`receiveReward`: The reward for renting out a car.

`loseReward`: The cost of moving a car between the companies.

## Output 

The program outputs the following:

- The optimal values for each state.

- The optimal policy for each state.

- A heatmap showing the optimal value for each state.






