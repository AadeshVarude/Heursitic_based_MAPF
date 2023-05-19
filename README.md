# Heursitic_based_MAPF
The objective of this project is to propose a motion planning methodology that can generate trajectories for multiple non-holonomic mobile robots, which are safe, dynamically feasible, and nearly optimal. The state-of-the-art literature divide the path search of the agents based on priority, which is further used for planning the path using Enhanced Conflict Based Search (ECBS). However, prioritized optimization may lead to infeasible subproblems for lower-priority robots due to lack of consideration by higher-priority robots. Hence, we propose a heiristic based motion planning approach that generates safe, dynamically feasible and near-optimal trajectories for multiple non-holonomic mobile robots. Our current implementation is divided into two parts, enhanced conflict-based search (ECBS) is leveraged as the multi-robot discrete path planner. These paths are subject to constraints to ensure obstacle avoidance and further these paths are parsed through a Los (Line of sight) control checking algorithm to generate a nonholonomic feasible path. Our current implementation involves A* based prioritized MAPF algorithm with feasible motion primitives, which adhere to the non-holonomic constraints of differential drive robot. We also propose heuristic based A* MAPF algorithm with feasible motion primitives, which imply the non holonomic constraints. We test our implementation on the DiffusionBot in ARGoS. Additionally, we have developed a custom visualizer using OpenCV to evaluate our algorithm's performance.
# Results
**Results of the improved algorithm with hueristic approach for multiple non holonomic robots.**
![MAPF](https://github.com/AadeshVarude/Heursitic_based_MAPF/assets/50541542/12ee40b2-f029-4066-b9bf-0801426ed486)

**Results of the MAPF algorithm with prioritized based approach**


**Results in Visualizer (Without Non holonomic constraints)**
  
**Results in Visualizer (With Non holonomic constraints)**
