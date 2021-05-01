
# Robotics Planning Navigation Algorithms
Assignments solved in the course Robotics: Path Planning and Navigation course by Dr. Madhav Krishna in Spring 2021.

## RRT : Rapidly-exploring Random Tree
- Implement the RRT path planning algorithm for a robot. The robot is to navigate a two dimensional space, avoiding known locations with obstacles, traveling from its initial location to a goal location. Given localization information (robot’s initial position, obstacle location, goal location), your task is to implement a path planning decision maker to drive the robot from its
initial position to the desired location. 
- Specifically, the problem can be formed as follows: Consider a 2D grid instantiated with different kinds of obstacles (for instance, geometrical shapes like Rectangles, Circles, Triangles or a combination of any
of the above 2/3). Assign a start and end point on this grid. 
- Implement the RRT algorithm for two cases, (1) Holonomic Robot and (2) Non-Holonomic Robot.
![holo-output](https://user-images.githubusercontent.com/30972206/116793881-1ae03280-aae7-11eb-91ca-011196ce237b.gif)
![holo-wheel-output](https://user-images.githubusercontent.com/30972206/116793885-1d428c80-aae7-11eb-8d6d-66e390ee29d9.gif)
![non-holo-output](https://user-images.githubusercontent.com/30972206/116793890-20d61380-aae7-11eb-845e-a0d1c58388d1.gif)
![non-holo-wheel-output](https://user-images.githubusercontent.com/30972206/116793893-23d10400-aae7-11eb-9927-6b6ed54cada5.gif)

------------------------------

## Model Predictive Control Planner
- Implement a discrete MPC planner for omni-wheel robot. You must implement the MPC algorithm for a two cases (i) With Obstacles (ii) Without Obstacles. You can use solvers like cvxopt in python or any other equivalent in Matlab.
- Your planner for a robot needs to satisfy various constraints on speed, acceleration, obstacle avoidance to make it feasible. Additionally your plan needs to optimize some aspect in your environment like speed, time or safety. Your plan should be n steps into the future.

![Screenshot from 2021-05-02 01-18-39](https://user-images.githubusercontent.com/30972206/116793434-5b8a7c80-aae4-11eb-9a67-50745bb8f973.png)
![Screenshot from 2021-05-02 01-24-02](https://user-images.githubusercontent.com/30972206/116793580-29c5e580-aae5-11eb-8a5c-71997db307be.png)

---------------------------------
## Velocity Obstacle formulation for collision avoidance
- Use velocity obstacle/ collision cone formulation to perform goal reaching obstacle avoidance. 
- Consider the following situation for the above: A single agent is supposed to reach its goal while avoiding multiple
moving obstacles.
- You can consider using a cost function in order to arrive at the optimal velocity such that the agent reaches the goal while avoiding the obstacles. You can select your preferred method for solving it: (a)Optimization (b) Sampling. Do the above for a Holonomic robot.
![vocc](https://user-images.githubusercontent.com/30972206/116793506-bd4ae680-aae4-11eb-9d03-ef1d74fb8ddc.jpeg)
![output-1](https://user-images.githubusercontent.com/30972206/116793867-0865f900-aae7-11eb-95dc-5612638a7b70.gif)
![output-2](https://user-images.githubusercontent.com/30972206/116793869-0b60e980-aae7-11eb-887b-ef8373b16496.gif)
![output-3](https://user-images.githubusercontent.com/30972206/116793739-2c750a80-aae6-11eb-97a4-3a7fb5c50c4b.gif)
