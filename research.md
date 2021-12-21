# Research

Research log for MATLAB Robotics Toolbox Exploration

## Path Planning

Path planning vocab:  
* A*&nbsp;&nbsp; &#8594; Finds the optimal path between  two points within a finite time period.
* RRT &#8594; A path planning algorithm that is faster than A*, but the path found is longer.  
   * RRT converges to a collision free path.
   * Algorithm can be developed using Euclidean distance or Manhattan distance calculations. There are pros and cons to each. 

## Pick and Place

Notes:  
* MATLAB Integrates with Gazebo. 

## Differential Drive
Differential drive robot:
* Movement is based on two separate driving wheels placed on either side of the robot chassis. 
* Diagram:
![](diffDrive.jpg)

## MATLAB Toolbox Info -  Accelerating Robotics Algorithms with Code Generation

Inverse kinematics:  
* ik Codegen generates code for inverse kinematics algorithms so you don't have to. 

## Inverse Kinematics

What is it:  
* Inverse kinematics involves calculating variable joint parameters needed to place the end manipulator on a robotic arm in a given position and orientation relative to the start of the chain. 

## Robot Dynamics 

What is it:  
* Robot dynamics is the relationship between the forces acting on a robot and the resulting motion of the robot. 
* Manipulator dynamics information is contained within the rigidBodyTree MATLAB object, which specifies the rigid bodies, attachment parts, and interial parameters for both kinematics and dynamics calculations. 

Dynamics Properties: 
* Specify info for individual bodies of your manipulator using properties of rigidBody objects: 
   * Mass &#8594; kg
   * Center of Mass &#8594; [x y z]
   * Inertia &#8594; [Ixx Iyy Izz Iyz Ixz Ixy]
        * First three elements are moment of interia, second three elements are product of intertia. 
        
rigidBodyTree Object Properties: 
* Gravity &#8594; g [x y z] m/s^2
* Input/output data format ?

