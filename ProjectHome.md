
---



---

IMPORTANT

This code project is now maintained at:

http://www.x-io.co.uk/open-source-imu-and-ahrs-algorithms/


---



---


The project provides the source code for the algorithms developed and discussed in the report, "An efficient orientation filter for inertial and inertial/magnetic sensor arrays".

The available downloads (tab above) include: The internal report (pdf) with source code in appendix; the Visual Studio 2008 projects used to create the IMU and MARG demo videos; an image (pdf) detailing the physical sensor axis alignments of the Sparkfun 6DOF IMU Razor and HMC5843 breakout board; and the x-io Board firmware (hex and readme in zip) required by the MARG demo to interface to the HMC5843.

Report abstract:

"This report presents a novel orientation filter applicable to IMUs consisting of tri-axis gyroscopes and accelerometers, and MARG sensor arrays that also include tri-axis magnetometers. The MARG implementation incorporates magnetic distortion and gyroscope bias drift compensation. The filter uses a quaternion representation, allowing accelerometer and magnetometer data to be used in an analytically derived and optimised gradient-descent algorithm to compute the direction of the gyroscope measurement error as a quaternion derivative. The benefits of the filter include: (1) computationally inexpensive; requiring 109 (IMU) or 277 (MARG) scalar arithmetic operations each filter update, (2) effective at low sampling rates; e.g. 10 Hz, and (3) contains 1 (IMU) or 2 (MARG) adjustable parameters defined by observable system characteristics. Performance was evaluated empirically using a commercially available orientation sensor and reference measurements of orientation obtained using an optical measurement system. A simple calibration method is presented for the use of the optical measurement equipment in this application. Performance was also benchmarked against the propriety Kalman-based algorithm of orientation sensor. Results indicate the filter achieves levels of accuracy exceeding that of the Kalman-based algorithm; <0.6 degrees static RMS error, <0.8 degrees dynamic RMS error. The implications of the low computational load and ability to operate at low sampling rates open new opportunities for the use of IMU and MARG sensor arrays in real-time applications of limited power or processing resources or applications that demand extremely high sampling rates."

Demonstration videos:

http://www.youtube.com/watch?v=Egl75nv9E7s (IMU algorithm)

http://www.youtube.com/watch?v=fOSTOnQzZCI (MARG algorithm)

http://www.youtube.com/watch?v=7GVXqNLLH7Q (Example application: camera control/stabilisation)