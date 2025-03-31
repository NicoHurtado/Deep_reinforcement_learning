# DQN Agent for CartPole-v1 (Keras-RL2 + Gym)

This project demonstrates how to train and evaluate a Deep Q-Network (DQN) agent using `keras-rl2` on the classic CartPole environment from OpenAI Gym.

---

## Objective

Balance a pole on a cart using reinforcement learning. The agent observes four continuous state variables and chooses between two discrete actions.

---

## Algorithms & Tools

- **DQN (Deep Q-Network)**: Value-based RL using experience replay and target networks.
- **Keras-RL2**: Lightweight RL wrapper around Keras models.
- **OpenAI Gym**: Provides the environment (`CartPole-v1`).
- **Keras (TensorFlow backend)**: Neural network implementation.

---

## Installation

### 1. Set up virtual environment (recommended)

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 2. Install required packages

```bash
pip install tensorflow==2.11.0 keras-rl2==1.0.5 gym==0.25.2 pyglet
```

> Use Python 3.10 or lower. `keras-rl2` is not compatible with TensorFlow ≥ 2.12 or Python ≥ 3.11.

---

## Training the Agent

Run `inteligent_agent.py` to train a DQN agent on CartPole-v1:

```bash
python inteligent.py
```

- Trains for `100,000` steps
- Uses `BoltzmannQPolicy` for action selection
- Prints the average score after testing

---

## Watching a Random Agent

If you want to visualize a baseline (non-learning) agent making random moves:

```bash
python random_agent.py
```

- Opens a GUI window showing the CartPole simulation
- Scores are printed for each episode

