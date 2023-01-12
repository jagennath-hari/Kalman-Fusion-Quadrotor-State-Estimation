# Kalman Fusion: Quadrotor State Estimation
To estimate the state of a quadrotor using different sensor a roboust state estimation technique is required. The gold-standard Kalman Filter was used to fuse data from sensors such as Intertial Measurement Unit(IMU), Vicon(Motion tracking cameras) and Visual Odometry(Optical Flow). The entire project has been divided into $3$ parts(a, b, c). Part (a) implements the Extended Kalman Filter(EKF) to fuse data from IMU and Vicon. Part (b) shows the effectiveness of RANSAC during visual odometry to remove outliers. Finally, part (c) shows the effectiveness of Unscented Kalman Filter(UKF) at the cost of computational speed by fusing the data from optical flow and IMU.

<p align="center">
  <img src ='assets/KLT_tracker_ORB.gif' width="400" height="300" >
  <img src ='assets/KLT_tracker_ORB2.gif' width="400" height="300" >
</p>
<p align="center">
  Kanade–Lucas–Tomasi(KLT) feature tracker using ORB
</p>

## Experiment and Inference
The $3$ submodules contain each of the parts(a, b, c) described above.

Click [HERE](https://github.com/jagennath-hari/Project-1-EKF.git) for Part (a).

Click [HERE](https://github.com/jagennath-hari/Project-2-Visual-Odometry-RANSAC.git) for Part (b).

Click [HERE](https://github.com/jagennath-hari/Project-3-UKF.git) for Part (c).

## Conclusion
The EKF proves to be the most efficient tool for fusing different sensors. The added benefit of high precision and fast computational speed makes it the most optimal sensor fusion technique for mobile robots lacking high-end on board computer. UKF on the other hand improves the accuracy of state estimation using sigma point propogation by sacrificing computational speed. The UKF is a viable state estimation technique for those robots having sufficient computational power, moreover visual odometry and IMU tends to drift over time, the usage of the UKF can improve the accuracy of state estimation when robots are traversing over longer durations.
