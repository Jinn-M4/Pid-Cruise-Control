# PID-based Cruise Control System Simulation

## Overview
This project implements a PID-based cruise control system to maintain a target vehicle speed of 60 km/h.  
The controller adjusts throttle input based on the error between the target speed and the current speed, simulating a vehicle’s longitudinal dynamics.

---

## System Description
- Target Speed: 60 km/h  
- Control Method: PID (Proportional–Integral–Derivative)  
- Simulation Environment: Python  

The system continuously calculates the speed error and applies PID control to regulate vehicle acceleration.  
A simplified vehicle model is used, including resistance and external disturbances.

---

## Key Features
- Implementation of PID controller for speed regulation  
- Vehicle dynamics simulation (longitudinal motion)  
- Disturbance handling (simulated road slope after 5 seconds)  
- Throttle saturation (realistic actuator constraint)  
- Anti-windup mechanism for integral term stability  

---

## Results

### Speed Tracking Performance
- The vehicle speed initially rises rapidly and shows a small overshoot  
- The system stabilizes and converges to the target speed (60 km/h)  
- After disturbance is introduced, the controller successfully recovers speed  

---

### Error Convergence
- Initial error starts high due to zero initial speed  
- The error decreases over time and converges to zero  
- Demonstrates effective steady-state error elimination  

---

## Technical Insights
- Increasing **Kp** improves response speed but may cause overshoot  
- **Ki** eliminates steady-state error  
- **Kd** reduces oscillations and improves stability  

The controller parameters were tuned to balance responsiveness and stability.

---

## Conclusion
This project demonstrates the application of PID control in vehicle speed regulation.  
It highlights key control system concepts such as stability, disturbance rejection, and steady-state error minimization.

---

## 🔗 Author
GitHub: https://github.com/Jinn-M4
