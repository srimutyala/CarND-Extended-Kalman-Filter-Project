# Extended Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

In this project we utilize a kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. Passing the project requires obtaining RMSE values that are lower that the tolerance outlined in the project rubric. 

## Project Instructions and Rubric

Code Compile

The main program can be built and run by doing the following from the project top directory.

    mkdir build
    cd build
    cmake ..
    make
    ./ExtendedKF

Accuracy

The algorithm is run against dataset 1 and the px, py, vx, vy coordinates have an RMSE < [.11, .11, .52, .52]. The same algorithm when run against dataset2 is close to the RMSE thresholds but slightly over.

[image1]: ./DS1.jpg "DS1"
[image2]: ./DS2.jpg "DS2"

![alt text][image1]
![alt text][image2]


Algorithm

The algorithm is built based on the mathematical concepts from the Udacity SDC lectures notes and videos. The measurements and weights are appropriately initialized. The algorithm also handles initially input whether it's LIDAR or RADAR.

Efficiency

The algorithm uses siple strcutures without the need for complex classes for data/property handling. Most calculations are straight forward and has been programmed to minimize code redundancy. 

