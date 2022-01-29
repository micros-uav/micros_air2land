# micros_air2land Dataset: A deep learning dataset for unmanned aerial vehicle auto landing from air to land


Machine Intelligence and Collective Robotics (MICRO) Lab, Sun Yat-Sen University, GuangZhou, China

---

 ### [Overview](#what-is-air2land) | [Simulation system](#simulation-system) | [Download](#download) | [Contact](#contact)

## What is micros_air2land?

Micros_air2land dataset is a multi-modal dataset for object detection and pose estimation in the context of fixed-wing unmanned aerial vehicle(UAV)’s auto-landing scenarios.

It bridges vision and robotics for ground-based vision guidance systems having the multi-modal data obtained by different sensors and pushes forward the development of computer vision and robotic algorithms targeted at visually assisted UAV landing. The dataset is composed of sequential stereo images and other sensor data (UAV pose, Pan-Tilt Unit angles) simulated in various climate conditions and landing scenarios. Since real-world automated landing data is very limited, our dataset provides the necessary foundation for vision-based tasks such as UAV detection, key point localization, and pose estimation .etc.

Micros_air2landhas several features:

- UAV detection, key point localization, pose estimation in ground vision images

- 115,684 labelled frames

- Rich in light and weather variation, covering early morning, midday and night, as well as sunny, rainy, snowy and foggy weather conditions.

- Frames are also labelled with GPS and gimbal rotation angle.

  <img src=".\imgs\Air2Land-dataset.png" alt="air2land-dataset" style="zoom: 80%;" />

## Simulation system

In our guidance system, two PTUs (pan-tilt units) are symmetrically located on both sides of the run way with each camera fixed on. The computing unit processes the images captured by cameras during UAV landing and estimates the its spatial coordinate and posture. The motion parameters are wirelessly feedback to the on-board autopilot to assist its safe landing. As shown in Figure 2, the [Pixhawk autopilot](https://pixhawk.org/) runs the actual airborne flight control code, which is responsible for the control of the drone during the loading and landing of the mission route, the monitoring and feedback of the drone flight status, the analysis and execution of operating instructions, etc. [QGroundControl](http://qgroundcontrol.com/) is a ground station for UAV flight protection, mainly responsible for flight mission planning, digital map display, data link transmission, and comprehensive data analysis. [ROS](https://www.ros.org/) connects various components to realize the transmission of messages on different topics, and the 3D simulator performs simulation and display of the scene. The built simulation system includes the physical controller and professional dynamics simulation software into the loop, which **retains the kinematic characteristics of the simulation data to the greatest extent**.

<img src=".\imgs\guidanceSystem.png" alt="simulation system" style="zoom:50%;" />

## Download

You are free to use micros_air2landdataset and all empirical data and metadata under the CC-BY licence. You can download the dataset (only partially provided) using [Baidu Drive](https://pan.baidu.com/s/1DP8yxtm3dfXAUWbykk12iQ)  (size: 2.01GB, passward: **6tk1**). When using this dataset in your research, we would appreciate that you cite our paper.


## Contact

The dataset, website, and API is still under development, and being maintained by Xunchen. Please contact me via e-mail if you have any questions: zhengxch7@mail2.sysu.edu.cn

