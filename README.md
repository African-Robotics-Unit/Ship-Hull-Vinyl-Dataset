We provide the data in the form of ROS bags, a well-known format that is commonly used in the SLAM and robotics fields. The data is supplied in three formats: raw, pre-processed and enhanced. The raw data has not been edited. The pre-processed data has been synchronized and images have been stereo rectified and undistorted. The enhanced data has been pre-processed and the images have additionally been enhanced with a CLAHE filter and dehazing, discussed more in chapter \ref{vo pipeline}, for improved underwater feature detection. With the ROS bags we also include the stereo camera and stereo-inertial calibration output files in yaml format. 

In the Meta Data folder, we detail the data collection method in a PDF for contextual understanding of the dataset and provide the data sheets of the sensors used. The original calibration data for camera and stereo-inertial calibrations are also included in ROS bag format so that users can perform their own calibrations if desired.  

The below figure shows the file structure of the dataset resource. 

African Robotics Unit - Ship Hull Vinyl/
├── README
├── Meta Data/
│   ├── Methods.pdf
│   ├── Sensor Suite/
│   │   ├── ArduCam_IMX477_Data_Sheet.pdf
│   │   ├── Xsens_MTi630_Data_Sheet.pdf
│   │   └── EZO_Pressure_Sensor_Data_Sheet.pdf
│   └── Calibration/
│       └── Michael Noyce - IMU Allan Variance
└── synchronize/
    ├── config/
    ├── launch/
    ├── src/
    ├── CMakeLists.txt
    ├── package.xml
    └── README.md