# Weapon_Detection_YOLOv8
In this repo we will perfrom weapon detection on videos with the help of YOLOv8 by training in onto Weapon Detection Dataset downloaded from kaggle 

# Downloading Dataset
To download the dataset from Kaggle using your terminal, You can use kagglehub to download datasets, follow these steps:
Install the Kaggle API if you haven't already:

`pip install kaggle`

`pip install kagglehub`

To use kagglehub from your terminal, follow these steps:

Open your terminal.
Run Python in the terminal:

`
python `

In the Python interactive shell, run the following:

`import kagglehub`

Download the dataset

`path = kagglehub.dataset_download("snehilsanyal/weapon-detection-test")`

Print the path where the dataset is saved

`print("Path to dataset files:", path)`

This will download the dataset to your machine, and the path where it's saved will be printed.

Dataset is : https://universe.roboflow.com/joao-assalim-xmovq/weapon-2/dataset/2

# How to use
Repository Cloning:

git clone https://github.com/Faryalaurooj/Weapon_Detection_YOLOv8.gt

Create a new environment (replace yolo_weapon_detection with your preferred environment name):

`conda create --name gun_detection_robo `

Activate the new environment:

`conda activate yolo_weapon_detection`

Installation of dependencies:

pip install -r requirements.txt


# Testing
Place best.pt file of pre-trained model in the main folder where you have opened your terminal and then run this command to run prediction on one image:

`yolo detect predict model=best.pt source=test_image.jpg --img-size 640 --save-txt --save-conf --device cuda`

To perform inference on all the images in a folder using YOLOv8 and your trained model (best.pt), you can use the source argument with the folder path. YOLOv8 will automatically process all the images in that folder.

`yolo detect predict model=best.pt source=path_to_test_folder`

in my case i wrote it like this 

` yolo detect predict model=best.pt source=/home/faryal/Downloads/Weapons-and-Knives-Detector-with-YOLOv8/test/images/`

To perform object detection on a video using YOLOv8 with your trained model (best.pt), you can use the yolo detect predict command in a similar way as for images, but instead of specifying an image file or folder, you specify the path to the video file.
Command for testing on a video:

`yolo detect predict model=best.pt source=path_to_video.mp4`


