# Design-of-Hostage-Locating-Hexapod-for-SAR-operations

Hostage Locating Hexapod
Introduction
Welcome to the Hostage Locating Hexapod project! This project was done by Final Year ECE students (Tenzin Kuenkhyab, Tenzin Gyeltshen, Sonam Tenzin and Choki Gyeltshen). This repository contains all the necessary files and instructions to build and operate a hexapod robot designed for search and rescue (SAR) operations. The hexapod is capable of navigating challenging terrains, streaming live video feeds, and detecting human presence in real-time.

Features
1. Six-Legged Design: Enhanced stability and mobility over rugged terrains.
2. Remote Control: Wireless control for navigating and operating the hexapod.
3. Live Video Streaming: Real-time video feed from a night vision camera.
4. Human Detection: Integrated AI for detecting human presence using YOLO v8.
5. Modular Components: Easily replaceable and upgradable parts.

Components
1. Hardware
    1. Chassis: Lightweight, durable frame.
    2. Legs: 3D-printed legs with servo motor attachments.
    3. Servo Motors: MG996R servo motors for leg articulation. (18 nos)
    
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/22699bd6-7320-4703-8766-f971fb3a2580)


    4. Controller: Raspberry Pi 4B for processing and control.
    
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/f176f9d7-7982-49eb-b82b-b3b8f1535ef7)


    5. Camera: Night vision camera for video feed.  
    
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/e9e474fc-f395-4998-9879-c5bc317f7dc0)


    6. Battery: Li-ion battery for power supply.  
    
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/dba48818-97e2-427f-9691-c965579ec55f)


    7. PCA 9685 16 channel Servo Driver: To control all the servo motors.  
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/d3f52a83-e4be-41a0-82b9-9979b75b0a2d)
   

    8. XL4005 Buck Converter: to control incoming voltages for the servo motors  
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/7eaa5b1a-8533-48b6-8ed1-ff1e42b1feff)


    9. Mini 360 Step Down Converter: to control incoming voltages for the raspberry pi
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/427e3301-c1e6-48b6-a5a6-1c8a010a8fcb)


    10. Overall Connection  
    ![image](https://github.com/Tenkuen/Design-of-Hostage-Locating-Hexapod-for-SAR-operations/assets/147422662/2af4271b-73f2-4453-a5ea-d142ba2c54c0)

     
2. Software
    1. Webots: Simulation software for testing hexapod movements.
    2. YOLO v8: AI tool for real-time object detection.
    3. Python Scripts: Control scripts for movement, video streaming, and human detection.
   
Installation
  Raspberry Pi
  Requirements
  Raspberry Pi is running Raspberry Pi OS.

   Enable I2C through raspi-config
    
    sudo raspi-config
    
  Install required packages
    
    sudo apt-get install python3-numpy python3-pip
    
  Install required Python modules
    
    pip3 install adafruit-circuitpython-servokit

Ngrok Installation

Install ngrok via Snap with the following command:
    
    snap install ngrok
   
Run the following command to add your authtoken to the default ngrok.yml configuration file.
    
    ngrok config add-authtoken *************************************************

Bluedot installation

Install Bluedot from Terminal:
    
    sudo pip3 install bluedot
    
To upgrade to the latest version:
    
    sudo pip3 install bluedot --upgrade


Assembly of Hexapod
  3D print all the files from the 3D design file. To assemble, visit https://wiki.lynxmotion.com/info/wiki/lynxmotion/view/servo-erector-set-robots-kits/ses-v1-robots/ses-v1-3-4-dof-hexapods/phoenix-3-dof-assembly/


Hexapod Testings
 
[![Watch the video](https://img.youtube.com/vi/miCRDi7d_nc/maxresdefault.jpg)](https://youtu.be/miCRDi7d_nc)

### [Watch this video for more information](https://youtu.be/miCRDi7d_nc)
 
 
