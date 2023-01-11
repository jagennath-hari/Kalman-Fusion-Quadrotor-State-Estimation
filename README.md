# Kalman Fusion: Quadrotor State Estimation
To estimate the state of a quadrotor using different sensor a roboust state estimation technique is required. The gold-standard Kalman Filter was used to fuse data from sensors such as Intertial Measurement Unit(IMU), Vicon(Motion tracking cameras) and Visual Odometry(Optical Flow). The entire project has been divided into $3$ parts. Part $1$ implements the Extended Kalman Filter to fuse data from IMU and Vicon. Part $2$ shows the effectiveness of RANSAC during visual odometry to remove outliers. Finally, part $3$ shows the effectiveness of Unscented Kalman Filter at the cost of computational speed by fusing the data from optical flow and IMU.

<p align="center">
  <img src ='assets/KLT_tracker_ORB.gif' width="1000" height="500" >
  Kanade–Lucas–Tomasi(KLT) feature tracker using ORB
</p>

## Experiment and Inference
The $3$ submodules contain each of the parts described above.
Click HERE for Part 1.
Click HERE for Part 2.
Click HERE for Part 3.
