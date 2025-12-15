# 🤖 **AiuBot — Classical ROS Navigation Stack**

> 🧭 *An educational ROS-based mobile robot project built to understand mapping, localization, planning, TF, and costmaps in the classical ROS navigation stack.*

[![ROS](https://img.shields.io/badge/ROS-Melodic-blue.svg)](https://wiki.ros.org/melodic)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Gazebo%20%7C%20RViz-orange.svg)]()
[![Language](https://img.shields.io/badge/Language-C%2B%2B-lightgrey.svg)]()

---

## 🧩 **Key Capabilities**

- ✅ Complete classical ROS navigation stack bringup  
- ✅ Online 2D SLAM using **GMapping**  
- ✅ Probabilistic localization using **AMCL**  
- ✅ Costmap-based global planning  
- ✅ **DWA (Dynamic Window Approach)** local planning  
- ✅ TF tree understanding and debugging  
- ✅ Simulation in **Gazebo + RViz**  
- ✅ Parameter tuning and behavior analysis  

---

## 🧪 **Run the Simulation**

To get started, clone the repository and build the workspace:

```bash
# Clone the repository
git clone https://github.com/ishika3011/aiubot.git
cd aiubot_ws

# Build and source the workspace
catkin_make
source devel/setup.bash

# Launch Gazebo simulation
roslaunch aiubot_gazebo aiubot_house.launch

# Launch navigation stack
roslaunch aiubot_navigation aiubot_navigation.launch
```

This launches:

- Gazebo indoor world  
- Robot model and sensors  
- GMapping for SLAM  
- AMCL for localization  
- Global and local planners (DWA)  

---

## 🧭 **Navigation Pipeline**

- **Mapping:** `gmapping` (laser-based 2D SLAM)  
- **Localization:** `amcl` (particle filter localization)  
- **Global Planning:** Costmap-based global planner  
- **Local Planning:** Dynamic Window Approach (DWA)  
- **Transforms:** `map → odom → base_link → sensor_frames`  

---

## 🎥 **Demo**
> [Gazebo Simulation](https://drive.google.com/file/d/1GPipBcYqLratmANUGE8NlWkhIxI8I28-/view?usp=sharing)
---


## 🧠 **Learning Outcomes**

- Understanding interaction between mapping, localization, and planning  
- Sensitivity of AMCL to motion and sensor model parameters  
- Effect of costmap inflation and resolution on navigation behavior  
- Stability vs responsiveness trade-offs in DWA tuning  
- Importance of TF consistency for reliable localization  

---

## ⚠️ **Assumptions & Limitations**

- 2D planar navigation only  
- Differential-drive robot model  
- Static indoor environments  
- Laser-based sensing only  
- No learning-based planning or control  
- Evaluated only in simulation  

---

## 🚀 **Future Roadmap**
 
- [ ] EKF/UKF-based sensor fusion  
- [ ] Learning-augmented costmaps
- [ ] MPC-based local planning 
- [ ] Deployment on physical robot hardware  

---

## 📄 **License**

MIT License © 2022 Ishika Saijwal  

---

## 👩‍💻 **Author**

**Ishika Saijwal**  
🔗 GitHub: https://github.com/ishika3011  
🔗 LinkedIn: https://linkedin.com/in/ishika-saijwal

