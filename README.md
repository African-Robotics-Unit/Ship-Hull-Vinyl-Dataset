An inside sweet water tank at the Institute for Maritime Technology (IMT) in Cape Town was used to take a controlled underwater dataset using a prototype sensor rig - 24 October 2023. The target scene is a life-sized photomosaic of the side of a commercial ship hull that IMT had previously taken when the ship was last in dry dock. The photomosaic is printed onto a large vinyl tarpaulin and hung along the side of the tank, seen below.

<img src=https://github.com/adriennewinter/Ship-Hull-Vinyl-Dataset/assets/41785960/88b79a48-5fd5-487f-be79-a25328e091f1 height="300" align=right>

Because the tank platform is 1m from the surface of the water, two 3m PVC pipes were used to manoeuvre the rig through the water, seen below. The rig is moved horizontally along the side of the platform facing the vinyl surface. Marks were placed on the PVC pipes as a visual aid to keep the rig at a relatively constant depth when moving horizontally. Once at the end of the vinyl, the rig is lowered directly downward to the next marked depth and moved horizontally back along the platform, creating a square ‘C’ shape. The data collection starts at 0.5m depth and returns at 1m depth.

We provide the data in the form of ROS bags on an accompanying [ZivaHub](https://zivahub.uct.ac.za/articles/dataset/Ship_Hull_Vinyl_Dataset/25828264) page. The data is supplied in two formats: raw and pre-processed. The raw data has not been edited. The pre-processed data has been synchronized and images have been stereo rectified and undistorted. With the ROS bags we also include the stereo camera and stereo-inertial calibration output files in yaml format. 

In the Meta Data folder, we detail the data collection method in a PDF for contextual understanding of the dataset and provide the data sheets of the sensors used. The original calibration data for camera and stereo-inertial calibrations are also included in ROS bag format on the sister ZivaHub so that users can perform their own calibrations if desired.

The below figure shows the file structure of this GitHub resource. 

```
African Robotics Unit - Ship Hull Vinyl/
├── README
├── LISENCE
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
```
