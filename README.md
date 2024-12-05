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

``print("Path to dataset files:", path)`

This will download the dataset to your machine, and the path where it's saved will be printed.
