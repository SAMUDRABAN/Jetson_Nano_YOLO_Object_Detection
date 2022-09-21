# Jetson_Nano_YOLO_Object_Detection

# NVIDIA jetson Nano 
NVIDIA Jetson Nano
jetson

![189518011-1d189aaf-bfdf-4d54-b41b-495afd89cf15](https://user-images.githubusercontent.com/97033991/191567441-69846278-694b-42de-acdb-b9034f5a7a68.jpg)

The NVIDIA Jetson Nano Developer Kit is an AI computer for makers, learners, and developers that brings the power of modern artificial intelligence to a low-power, easy-to-use platform. Get started quickly with out-of-the-box support for many popular peripherals, add-ons, and ready-to-use projects.

We are grateful to NVIDIA and SRM Institute of Science and Technology for giving us the opportunity to work on this project. 

# Setting up NVIDIA Jetson Nano 

![WhatsApp Image 2022-09-22 at 00 57 51](https://user-images.githubusercontent.com/97033991/191594355-489780a5-f877-45c7-8778-d4e7b77b5a23.jpeg)




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



make
To run object detection with Darknet, we need a model config and model weights(in the cfg directory).
wget https://pjreddie.com/media/files/yolov3.weights
wget https://pjreddie.com/media/files/yolov3-tiny.weights
We are done with installation part and we need to run the camera module to see the predictions in real time-
detectnet-camera.py

# Results from our kit -


https://user-images.githubusercontent.com/97033991/191591158-5ebe1e5b-bdae-49e1-b5e3-a1b67550447c.mp4



# AUTHORS 

# SAMUDRA BANERJEE (ML AND WEB DEVELOPER)

![WhatsApp Image 2022-09-13 at 17 25 05](https://user-images.githubusercontent.com/97033991/191584794-cc53d331-a268-475c-b5f9-0ec5eca6c440.jpeg)


# GOVIND KALAWATE(ML AND WEB DEVELOPER)

![WhatsApp Image 2022-09-21 at 10 39 41](https://user-images.githubusercontent.com/97033991/191584737-76733a01-33e1-4771-9839-29a2897dafaa.jpeg) 

# OM  WAGHMARE(ML AND FLUTTER DEVELOPER)

![image](https://user-images.githubusercontent.com/97033991/191585110-a4e157d0-e3f5-483e-9a74-af4546c71e9b.png)

