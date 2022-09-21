# Jetson_Nano_YOLO_Object_Detection

Object-Detection-in-Jetson-Nano
NVIDIA Jetson Nano
jetson

![189518011-1d189aaf-bfdf-4d54-b41b-495afd89cf15](https://user-images.githubusercontent.com/97033991/191567441-69846278-694b-42de-acdb-b9034f5a7a68.jpg)

The NVIDIA Jetson Nano Developer Kit is an AI computer for makers, learners, and developers that brings the power of modern artificial intelligence to a low-power, easy-to-use platform. Get started quickly with out-of-the-box support for many popular peripherals, add-ons, and ready-to-use projects.

We are grateful to NVIDIA and SRM Institute of Science and Technology for giving us the opportunity to work on this project. 

Setting up NVIDIA Jetson Nano


For setting up the kit for the first time we reffered to the tutorial made by the NVIDIA Developer - Video Link

Other than the kit we have connected some other required objects-

IMX-219-77 Camera Module
Ethernet connection
External Monitor/Display
32GB MicroSD Card
HDMI Cable
Power Adapter with Supply image
Setting up YOLO-Object Detection
We will be installing Darknet using the Jetson's terminal from AlexeyAB/darknet.
git clone https://github.com/AlexeyAB/darknet.git
cd darknet
Enable GPU and OpenCV support by editing the Makefile and also compile the makefile-
sudo nano Makefile
Set the following values to enable GPU and OpenCV support-

GPU=1

CUDNN=1

OPENCV=1 
https://user-images.githubusercontent.com/97033991/191580097-c48ba9e1-6527-47c8-adc4-4117b317aeb2.mp4

make
To run object detection with Darknet, we need a model config and model weights(in the cfg directory).
wget https://pjreddie.com/media/files/yolov3.weights
wget https://pjreddie.com/media/files/yolov3-tiny.weights
We are done with installation part and we need to run the camera module to see the predictions in real time-
detectnet-camera.py
Results from our kit -
