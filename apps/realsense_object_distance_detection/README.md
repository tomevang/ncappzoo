# Realsense Object Distance Detection
## Introduction
This app does object detection using the Intel Movidius Neural Compute Stick 2/OpenVINO R2 and detects how far the object is using the Intel Realsense Camera (tested with Intel Realsense D415 camera).

## Building the Example

To run the example code do the following :
1. Open a terminal and change directory to the sample base directory
2. Type the following command in the terminal: ```make all```

## Running the Example

After building the example you can run the example code by doing the following :
1. Open a terminal and change directory to the sample base directory
2. Type the following command in the terminal: ```make run``` 

When the application runs normally, another window should pop up and show the feed from the Intel Realsense camera. The program should perform inferences on frames taken from the Intel Realsense Camera.

## Prerequisites
This program requires:
- 1 NCS2/NCS1 device
- OpenVINO 2019 R2 Toolkit
- OpenCV 3.3 with Video for Linux (V4L) support and associated Python bindings*.
- [Intel Realsense SDK 2](https://www.intelrealsense.com/developers#downloads)
- Intel Realsense Camera (tested with [Intel D415 Realsense Camera](https://store.intelrealsense.com/buy-intel-realsense-depth-camera-d415.html))


*It may run with older versions but you may see some glitches such as the GUI Window not closing when you click the X in the title bar, and other key binding issues.

Note: All development and testing has been done on Ubuntu 16.04 on an x86-64 machine.

## Makefile
Provided Makefile has various targets that help with the above mentioned tasks.

### make run or make run_cpp
Runs the sample application.

### make help
Shows available targets.

### make all
Builds and/or gathers all the required files needed to run the application.

### make data
Gathers all of the required data need to run the sample.

### make deps
Builds all of the dependencies needed to run the sample.

### make default_model
Compiles an IR file from a default model to be used when running the sample.

### make install-reqs
Checks required packages that aren't installed as part of the OpenVINO installation. 

### make uninstall-reqs
Uninstalls requirements that were installed by the sample program.
 
### make clean
Removes all the temporary files that are created by the Makefile.
