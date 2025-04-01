# Reinforcement Learning: Q-Learning and Dyna-Q

## Project Overview  
This project focuses on developing and applying **Q-Learning**, a model-free reinforcement learning (RL) algorithm, and **Dyna-Q**, a model-based extension. The learning agent was tested in a simulated navigation environment where it learned optimal paths under uncertainty and obstacles. This foundational RL work prepares for future applications in algorithmic trading and real-world decision-making.

**Languages/Tools Used:** Python, NumPy  
**Key Concepts:** Reinforcement Learning, Q-Learning, Dyna-Q, Policy Learning, Navigation, Exploration vs. Exploitation

---

## Project Objectives
- Implement a Q-Learner agent with support for:
  - Discrete state and action spaces
  - Learning via Q-table updates using the Bellman Equation
  - Epsilon-greedy action selection with decaying randomness
- Extend the learner using **Dyna-Q**, a hybrid approach that improves convergence speed by "hallucinating" additional experience from an internal model
- Test both Q-Learning and Dyna-Q in a **navigation problem** modeled as a grid world with:
  - Obstacles, quicksand, and random movement
  - Goal-seeking behavior and penalty/reward conditions
- Measure agent performance using median reward per episode and convergence speed

---

## Technical Highlights
- Implemented `QLearner` with:
  - Adjustable learning rate (alpha), discount factor (gamma), and exploration settings (rar, radr)
  - Q-table initialized to zeros and updated with every action taken
  - Support for action selection with decaying randomness (rar * radr)
- Added **Dyna-Q** capability:
  - Internal model stores past experiences
  - Generates simulated experiences to update the Q-table in addition to real experiences
  - Speeds up convergence significantly (shown via navigation tests)
- Code designed to be **domain-agnostic**: the same QLearner can later be applied to financial trading

---

## Value & Learning Outcomes
- Gained deep understanding of reinforcement learning fundamentals  
- Learned the difference between **model-free** and **model-based** learning  
- Designed an agent capable of **adapting policy through experience**  
- Implemented **efficient exploration-exploitation balancing**  
- Developed reusable, testable, and extensible RL architecture

---

## Repository Access  
Due to academic policy, the full implementation—including agent code, environment wrappers, and experiment scripts—is stored in a private GitHub repository. **Access available upon request.**

