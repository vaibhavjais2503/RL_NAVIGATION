# 🤖 Reinforcement Learning for Autonomous Navigation & Dynamic Obstacle Avoidance (DQN + TD3)

Topological Path Planning represents the environment as a connectivity graph of free-space regions (nodes) and safe transitions (edges). Instead of dense metric maps, it plans a route by searching this graph, making navigation memory-efficient and robust in changing environments.

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

Install dependencies
pip3 install -r requirements.txt

Source ROS2
source /opt/ros/foxy/setup.bash

Launch simulation
ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py

Train DQN
python3 train_dqn.py

Train TD3
python3 train_td3.py

Evaluate
python3 evaluate.py

📈 Results (Summary)

Evaluation metrics:

✅ Success rate (goal reached)
❌ Collision rate
⭐ Average reward
📉 Critic loss / TD error

🚀 Future Work

Larger + more complex environments
Sensor fusion (LiDAR + camera)
Real-world deployment on TurtleBot3

👤 Author

Vaibhav Jaiswal
IIIT Bhagalpur
📩 vaibhavjaiswal2503@gmail.com
GitHub: https://github.com/vaibhavjais2503

