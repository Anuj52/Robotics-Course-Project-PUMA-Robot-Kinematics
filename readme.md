# 🤖 Robotics Course Project – PUMA Robot Kinematics (MATLAB)  

## Aim  
To simulate the **kinematics of a PUMA robotic arm** in MATLAB. The objectives are:  
- **Forward Kinematics** → Compute end-effector position and orientation from given joint angles.  
- **Inverse Kinematics** → Calculate joint angles for a specified end-effector position.  
- **Simulation** → Visualize smooth and accurate motion of the robot arm.  

---

## Approach  
1. Defined the **Denavit–Hartenberg (DH) parameters** for the PUMA robot.  
2. Implemented MATLAB scripts for:  
   - `forwardkinematics.m` → Forward kinematics calculation  
   - `pumaForekinem.m` → DH parameter-based forward kinematics  
   - `Inverse.m` → Inverse kinematics solver  
   - `Simulation.m` → Robot motion simulation  
3. Verified correctness by comparing analytical results with simulation outputs.  

---

## Results  
- Forward kinematics produced accurate **end-effector positions and orientation matrices**.  
- Inverse kinematics provided feasible **joint angle solutions** for target positions.  
- Simulation demonstrated **smooth trajectory and controlled motion** of the PUMA robotic arm.  

---

## Usage  
Run the scripts in MATLAB:  

- **Forward Kinematics**  
  ```matlab
  forwardkinematics

## Inverse Kinematics  
- `Inverse.m` → Calculates joint angles for a given end-effector position.  

## Simulation  
- `Simulation.m` → Visualizes smooth motion of the PUMA robotic arm.  

---

## Workflow  

```mermaid
flowchart TD
    A[Input: Joint Angles / Target Position] --> B[Forward Kinematics]
    B --> C[End-Effector Position]
    A --> D[Inverse Kinematics]
    D --> E[Joint Angles]
    C --> F[Simulation]
    E --> F
    F --> G[Robot Motion Visualization]

---

## References  
- J.J. Craig, *Introduction to Robotics: Mechanics and Control*  
- MATLAB Robotics Toolbox Documentation  
