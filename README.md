# Autonomous Racing Reinforcement Learning Model  
*A2RL STEM League – ATRC & AWS*

## Overview
This repository contains a **trained Reinforcement Learning (RL) model** developed and optimized during the **A2RL STEM League**, an autonomous racing competition organized by **ATRC** in collaboration with **AWS**. The objective of the competition was to design, train, and evaluate RL agents capable of completing racing laps efficiently, safely, and consistently within a simulated autonomous racing environment.

The provided model represents one of the **final optimized training outcomes**, focusing on **stability, smooth driving behavior, and reliable lap completion**, rather than aggressive but inconsistent speed strategies.

---

## Model File
**File name:**  
`stabilizing-trial3-clone1-model.tar.gz`

**Description:**  
This archive contains the trained policy and associated parameters generated from the reinforcement learning training pipeline. The model was iteratively improved through multiple trials and cloning stages, with this version reflecting a **stabilized training phase** that demonstrated consistent performance during evaluation runs.

---

## Technical Context

### Learning Paradigm
- **Approach:** Reinforcement Learning
- **Type:** Policy-based RL (competition-standard setup)
- **Training Objective:**  
  Maximize lap completion consistency while maintaining optimal racing lines and minimizing off-track events.

### Environment
- Autonomous racing simulation environment used in the A2RL STEM League
- Continuous interaction between agent and environment through:
  - State observations (track position, speed, heading, progress, etc.)
  - Action space (steering angle, throttle control)
  - Reward signals

---

## How It Was Trained

### 1. Reward Function Design
The training process began with the design of a **custom reward function** tailored to autonomous racing constraints. The reward logic emphasized:

- Staying within track boundaries
- Maintaining alignment with the racing line
- Smooth steering to avoid oscillations
- Controlled throttle usage to reduce instability
- Penalization for off-track behavior, excessive steering, and abrupt speed changes

The reward function was iteratively refined to balance **speed, stability, and safety**, ensuring the agent learned consistent driving behavior rather than short-term aggressive gains.

---

### 2. Training Trials and Iteration
Multiple training trials were executed with varying configurations, including:
- Adjustments to reward weightings
- Exploration–exploitation balance tuning
- Observation sensitivity refinements

Each trial was evaluated based on:
- Lap completion rate
- Frequency of off-track events
- Steering smoothness
- Consistency across multiple evaluation runs

Poor-performing configurations were discarded early, while promising models were retained for further refinement.

---

### 3. Model Cloning and Fine-Tuning
High-performing agents were **cloned** and used as starting points for additional training rounds. This approach allowed:
- Faster convergence
- Preservation of stable driving behavior
- Incremental improvements without retraining from scratch

The provided model corresponds to a **cloned and fine-tuned training stage**, where stability and control had already been learned and further optimized.

---

### 4. Stabilization Phase
The final training phase focused on **behavior stabilization**, prioritizing:
- Reduction of steering jitter
- Smoother corner handling
- Improved recovery near track boundaries
- Consistent throttle modulation

At this stage, training emphasized reliability and predictability over marginal speed gains.

---

### 5. Evaluation and Selection
Models were evaluated using repeated simulation runs under identical conditions. Selection criteria included:
- Consistent lap completion
- Low variance in driving behavior
- Minimal off-track penalties
- Smooth control outputs

The selected model demonstrated **repeatable and stable performance**, making it suitable as a reference or baseline model.

---

## Key Features of the Model
- Optimized for stable autonomous driving
- Reduced oscillation and over-steering
- Improved near-boundary recovery
- Balanced speed and control
- Suitable as a baseline for further experimentation or fine-tuning

---

## Usage Notes
This model file is provided for:
- Academic demonstration
- Competition documentation
- Portfolio and research reference

It can be:
- Loaded into compatible autonomous racing or RL evaluation environments
- Used as a starting point for further training
- Analyzed to study reward-function effectiveness and policy behavior

---

## Project Context
This work was completed as part of the **A2RL STEM League**, where participants were required to:
- Apply reinforcement learning concepts in practice
- Design and optimize reward functions
- Train autonomous agents under real constraints
- Evaluate models using performance and stability metrics

The project provided hands-on experience in:
- Reinforcement learning optimization
- Autonomous systems development
- Iterative experimentation and evaluation
- AI model performance analysis

---

## Author
**Manar Omar**  
Fourth-year Information Systems student  
Ajman University  

This project forms part of my broader work in **AI, machine learning, and software engineering**, alongside academic, competition, and industry experience.

---

## License / Disclaimer
This repository is intended for **educational and portfolio purposes**.  
The model reflects competition-based experimentation and may require adaptation for other environments or real-world systems.
