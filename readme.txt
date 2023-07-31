Sensors: 9DOF-IMU (Xsens DOT)
Sensor A is fixed on the right foot, and sensor B is fixed on the left foot.

Explanation of some abbreviations:
XF: the agent 1
HR: the agent 2
ccw: counterclockwise
cw: clockwise

Folders description:
1. indoor rectangle: along a rectangle indoor
2. indoor 8shape: along a 8 shape path, the outline of the 8 is the rectangle.
3. outdoor sportspark: along a standard 400m running track.
4. calibration data: for accelerometers.
5. unsync data: Unsynchronised indoor ccw and cw rectangle walking data. (The sensor sync function was forgotten to be turned on, but the data might be useful for some people.)
1-3 are collected in 60Hz sync.

Variables:
data: the raw data.
imu0: the structured data that is transferred to the right-front-up coordinate system, the units are 
%     imu.acc - specific force, in m/s^2
%     imu.gyros - angular velocity, in rad/s
%     imu.mag - magnetic field strength, in nT
%     imu.ts - sampling time, in s, inverse of sampling frequency
%     imu.sT - Sampling Timestamp
pathdirec: 1 is ccw, -1 is cw

The markers on the reference path:
%             marker = [0, 0;0,1.2;0, 2.4;0, 3.6;0, 4.8;0, 6.0;0, 7.2;0, 8.4;0, 9.6;
%                     -1.2, 9.6;
%                     -2.4, 9.6;-2.4, 8.4;-2.4,7.2;-2.4,6.0;-2.4,4.8;-2.4,3.6;-2.4, 2.4;-2.4, 1.2;-2.4, 0;
%                     -1.2, 0;0, 0];
