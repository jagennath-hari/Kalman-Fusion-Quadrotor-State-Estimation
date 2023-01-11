# Kalman Fusion: Quadrotor State Estimation
To estimate the state of a quadrotor using different sensor a roboust state estimation technique is required. The gold-standard Kalman Filter was used to fuse data from sensors such as Intertial Measurement Unit(IMU), Vicon(Motion tracking cameras) and Visual Odometry(Optical Flow). The entire project has been divided into $3$ parts. Part $1$ implements the Extended Kalman Filter(EKF) to fuse data from IMU and Vicon. Part $2$ shows the effectiveness of RANSAC during visual odometry to remove outliers. Finally, part $3$ shows the effectiveness of Unscented Kalman Filter(UKF) at the cost of computational speed by fusing the data from optical flow and IMU.

<p align="center">
  <img src ='assets/KLT_tracker_ORB.gif' width="1000" height="500" >
  Kanade–Lucas–Tomasi(KLT) feature tracker using ORB
</p>

## Experiment and Inference
The $3$ submodules contain each of the parts described above.

Click HERE for Part 1.

Click HERE for Part 2.

Click HERE for Part 3.

## Conclusion
The EKF proves to be the most efficient tool for fusing different sensors. The added benefit of high precision and fast computational speed makes it the most optimal sensor fusion technique for mobile robots lacking high-end on board computer. UKF on the other hand improves the accuracy of state estimation using sigma point propogation by sacrificing computational speed. The UKF is a viable 
