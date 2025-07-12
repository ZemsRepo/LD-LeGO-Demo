# LiDAR, IMU and GNSS sensor fusion for odometry and mapping in highway and urban scenarios

## SLAM Demo
<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe src="https://www.youtube.com/embed/WzqqQRNQ9w8" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;" 
          allowfullscreen>
  </iframe>
</div>

## Abstract
This thesis addresses the problem of odometry and mapping in real-world highway and urban scenarios through a multi-sensor fusion framework that combines Light Detection and Ranging (LiDAR), Inertial Measurement Unit (IMU), and Global Navigation Satellite System (GNSS). Under the paradigm of Simultaneous Localization and Mapping (SLAM), we propose a LiDAR-centric system capable of tackling key challenges including dynamic objects, sensor drift, sparse geometric structures, and lack of loop closure.

To improve robustness and accuracy, the system incorporates three core components: (1) a motion removal module based on a sparse 3D convolutional neural network (CNN), which filters out independently moving objects to stabilize scan registration; (2) an online, ground-based dynamic LiDAR calibration strategy that compensates for sensor misalignments during runtime; and (3) a decoupled sensor fusion design, leveraging IMU data in the frontend for high-frequency pose initialization and GNSS measurements in the backend to constrain long-term drift.

The entire framework is designed for real-time execution on standard and embedded platforms without reliance on high-end graphical processing units (GPUs), ensuring practical deployability in industrial contexts. Evaluations conducted on three production-grade datasets—spanning both highway and urban environments, demonstrate significant gains in localization accuracy and robustness.

By bridging the gap between academic research and industrial application, this work delivers a scalable and hardware-efficient SLAM solution for autonomous driving in complex real-world settings.