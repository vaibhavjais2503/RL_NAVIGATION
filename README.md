# 🤖 Reinforcement Learning for Autonomous Navigation & Dynamic Obstacle Avoidance (DQN + TD3)

Autonomous navigation project using **Deep Q-Network (DQN)** and **Twin Delayed DDPG (TD3)** to train a **TurtleBot3** for goal-reaching and **dynamic obstacle avoidance** in a **ROS2 Foxy + Gazebo 11** simulation.

![Simulation Demo](media/simulation.gif)

---

## ✨ Highlights
- 🚗 Autonomous navigation in TurtleBot3 simulation
- 🧱 Avoids **static + dynamic obstacles**
- 🧠 Implements **DQN** (discrete) and **TD3** (continuous control)
- ⚙️ Training stability improvements (scheduler, tuning, etc.)
- 📊 Performance evaluation with reward/loss/success trends

---

## 🧩 Project Overview
This project trains a TurtleBot3 agent to learn navigation behavior using reinforcement learning. The agent learns to:
- reach a goal efficiently
- avoid collisions with moving obstacles
- improve success rate over episodes via trial-and-error learning

---

## 🧠 Algorithms Used

### Deep Q-Network (DQN)
- Off-policy, value-based RL
- Learns Q(s,a) using a neural network
- Uses ε-greedy exploration and target network updates

### Twin Delayed DDPG (TD3)
- Actor-Critic RL for continuous actions
- Twin critics reduce overestimation bias
- Delayed policy updates improve stability

---

## 🛠️ Installation

### Prerequisites
- Ubuntu 20.04
- ROS2 Foxy
- Gazebo 11
- Python 3.8+
- PyTorch

### Clone
```bash
git clone https://github.com/vaibhavjais2503/RL_NAVIGATION.git
cd RL_NAVIGATION
