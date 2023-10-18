# Conflict-Aware-Safe-Reinforcement-Learning
##Conflict-Aware Safe Reinforcement Learning: A Meta-Cognitive Learning Framework

### [Link to paper](https://ieeexplore.ieee.org/abstract/document/9646175)

#### Authors: [Majid Mazouchi](https://majid-mazouchi.github.io/), Subramanya P. Nageshrao, Hamidreza Modares
### Abstract
In this paper, a data-driven conflict-aware safe reinforcement learning (CAS-RL) algorithm is presented for control of autonomous systems. Existing safe RL results with predefined performance functions and safe sets can only provide safety and performance guarantees for a single environment or circumstance. By contrast, the presented CAS-RL algorithm provides safety and performance guarantees across a variety of circumstances that the system might encounter. This is achieved by utilizing a bilevel learning control architecture: A higher meta-cognitive layer leverages a data-driven receding-horizon attentional controller (RHAC) to adapt relative attention to different system's safety and performance requirements, and, a lower-layer RL controller designs control actuation signals for the system. The presented RHAC makes its meta decisions based on the reaction curve of the lower-layer RL controller using a meta-model or knowledge. More specifically, it leverages a prediction meta-model (PMM) which spans the space of all future meta trajectories using a given finite number of past meta trajectories. RHAC will adapt the system's aspiration towards performance metrics (e.g., performance weights) as well as safety boundaries to resolve conflicts that arise as mission scenarios develop. This will guarantee safety and feasibility (i.e., performance boundness) of the lower-layer RL-based control solution. It is shown that the interplay between the RHAC and the lower-layer RL controller is a bilevel optimization problem for which the leader (RHAC) operates at a lower rate than the follower (RL-based controller) and its solution guarantees feasibility and safety of the control solution. The effectiveness of the proposed framework is verified through a simulation example.

### Overview figure
![Overview](https://github.com/majid-mazouchi/majid-mazouchi.github.io/blob/main/assets/img/ConflAwProj.png)

## Algorithm 2 Conflict-Aware RL Algorithm
![algorithm](https://github.com/majid-mazouchi/majid-mazouchi.github.io/blob/main/assets/img/Algorithm1ConflQLearning.png)
