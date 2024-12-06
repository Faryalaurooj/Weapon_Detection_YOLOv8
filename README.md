# Weapon and Knives Detection System

This repository contains the source code and resources related to the academic weapon detection project, developed as part of research in the area of ​​computer security.

## Overview

The main objective of this project is to design and implement an advanced system for the autonomous detection of firearms and knives. Using the YOLOv8 (You Only Look Once) framework and transfer learning techniques, we seek to improve security effectiveness through continuous, real-time surveillance.

## Key Features

- **YOLOv8 Framework:** One implementation uses YOLOv8, known for its efficiency in real-time object detection.
  
- **Transfer Learning:** Transfer learning techniques are employed to adapt the model to a specific context and improve accuracy in weapon detection.

- **Integration with IP Cameras:** The system is designed for easy integration with IP cameras, allowing for real-time surveillance and immediate notifications.


## Dataset

https://universe.roboflow.com/joao-assalim-xmovq/weapon-2/dataset/2

## How to use

1. **Repository Cloning:**

```
git clone https://github.com/Faryalaurooj/Weapon_Detection_YOLOv8.git
```

2. **Installation of dependencies:**

```
pip install -r requirements.txt
```

# Testing

To perform inference on all the images in a folder using YOLOv8 and your trained model (best.pt), you can use the source argument with the folder path. YOLOv8 will automatically process all the images in that folder.
```
yolo detect predict model=best.pt source=path_to_test_folder
```
```
yolo detect predict model=best.pt source=/home/faryal/Downloads/Weapons-and-Knives-Detector-with-YOLOv8/test/images/

```
Command for testing on a video:
```
yolo detect predict model=best.pt source=path_to_video.mp4
```
For example if you have downloaded the video gun2.mp4 then run this command

```
yolo detect predict model=best.pt source=./test_videos/gun2.mp4
```


