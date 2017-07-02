#**Extended kalman filter project for vehicle lidar & radar sensor fusion**

This is a project for Udacity Self-Driving Car Nanodegree program. In this project, I utilize a kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. All codes are written with C++ and tested on the Udacity simulator 

## Requirement 

- C++
- Udacity simulator : [here](https://github.com/udacity/self-driving-car-sim/releases)
- uWebSocketIO : [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac
- For window users : [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. 

## Other Important Dependencies

* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Run the Project 

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF

## About the Project 

I constructed the C++ software mostly based on the lecture. The performance of extended kalman filter is evaluated by 
the RMSE(Root mean squared error) of position x,y and velocity vx,vy. 
I got 0.0975, 0.0854, 0.4185, 0.4790 for each, which is quite accurate number to gound truth.
This is my result image:  
![Test image](https://github.com/KHKANG36/Extended-Kalman-Filter-Project/Sim2.jpg)

## Discussion/Issues 

I also tested this while using only one sensor, either radar or lidar. As I expected, lidar only shows almost comparable performance to both sensor fusion scenario. Otherwise, radar only case shows relatively poor performance. 
