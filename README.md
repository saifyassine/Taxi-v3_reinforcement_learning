# Reinforcement Learning with Q-Learning for Taxi-v3 Environment

## Goal
The objective is to utilize the Q-Learning algorithm to solve the Taxi-v3 environment from OpenAI Gym. The task is to make the taxi agent learn to navigate the grid world, pick up passengers, and drop them off at their destinations.
For detailed information about the Taxi-v3 environment, visit [here](https://gymnasium.farama.org/environments/toy_text/taxi/).

## Algorithm: Q-Learning

### Required Libraries
- `numpy`: For numerical computations
- `pygame`: For rendering the environment
- `gymnasium`: For accessing the Taxi-v3 environment

### Algorithm Implementation
The code utilizes the Q-learning equation to update Q-values for state-action pairs iteratively over a specified number of epochs.

- `alpha` (learning rate) and `gamma` (discount factor) are set.
- `Qmax()` function finds the action with the maximum Q-value for a given state.
- Training the Q-Algorithm:
  - Iterates through epochs, updates Q-values based on actions taken and rewards received.
- Testing the Trained Algorithm:
  - Utilizes the trained Q-value matrix to navigate the environment without retraining.

## Code Overview
- **Training Phase**:
  - Creates the environment and initializes necessary variables.
  - Iterates through epochs, updating Q-values based on the Q-learning algorithm.
  - Displays total reward per epoch and calculates training time.

- **Testing Phase**:
  - Loads the pre-trained Q-value matrix from a saved file.
  - Uses the trained Q-values to test the algorithm without further training.
  - Outputs the total reward achieved during the test.

