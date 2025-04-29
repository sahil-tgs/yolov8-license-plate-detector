[requirements.txt](https://github.com/user-attachments/files/15526179/requirements.txt)
# Car License Plate Detection using YOLOv8


This repository contains code for detecting car license plates using the state-of-the-art object detection algorithm, YOLOv8, and a dataset from Kaggle.

```You can access this streamlit  link:
https://yolov8-1.onrender.com
```
## Dataset

The dataset used for training and evaluation is from Kaggle and can be found [here](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection). This dataset contains images of cars with their license plates annotated using bounding boxes.

## Setup

1. Clone this repository:

```bash
git clone https://github.com/vedantparmar12/car-plate-detection.git
```
cd car-plate-detection
Install the required dependencies:
```
bashCopy codepip install -r requirements.txt
```
Download the Kaggle dataset and place it in the data directory.

Training
To train the YOLOv8 model on the car license plate dataset, run the following command:``` python train.py --data data/car_plates.yaml --weights yolov8n.pt --cfg yolov8n.yaml --batch 16 --epochs 100 ```

Sure, here's a README file for your GitHub repository on car license plate detection using YOLOv8 and the Kaggle dataset:
markdownCopy code# Car License Plate Detection using YOLOv8

This repository contains code for detecting car license plates using the state-of-the-art object detection algorithm, YOLOv8, and a dataset from Kaggle.

## Dataset

The dataset used for training and evaluation is from Kaggle and can be found [here](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection). This dataset contains images of cars with their license plates annotated using bounding boxes.

## Setup

1. Clone this repository:

```bash
git clone https://github.com/vedantparmar12/car-plate-detection.git
```
cd car-plate-detection

Install the required dependencies:

bashCopy code
``` pip install -r requirements.txt
```


val_batch1_labels
``` https://wandb.ai/omega_one/YOLOv8/reports/val_batch1_labels-24-08-09-15-56-34---Vmlldzo4OTgwMTA3```

metric graph can be visualized here
``` https://wandb.ai/omega_one/YOLOv8/reports/results-24-08-09-16-04-30---Vmlldzo4OTgwMTc0  ```

f1 graph
``` https://wandb.ai/omega_one/YOLOv8/reports/undefined-24-08-09-16-06-19---Vmlldzo4OTgwMTg0 ```



Download the Kaggle dataset and place it in the data directory.

Training
To train the YOLOv8 model on the car license plate dataset, run the following command:
bashCopy codepython train.py --data data/car_plates.yaml --weights yolov8n.pt --cfg yolov8n.yaml --batch 16 --epochs 100
This will start training the yolov8n model on the dataset using a batch size of 16 for 100 epochs. You can adjust the hyperparameters as needed.
Evaluation
To evaluate the trained model on the test set, run the following command:
``` python val.py --data data/car_plates.yaml --weights runs/train/exp/weights/best.pt --task test
```
This will evaluate the best model weights from the training run on the test set and display metrics like precision, recall, and mean Average Precision (mAP).
Inference
To run inference on a single image or a directory of images, use the following command:
```
python detect.py --source path/to/image/or/directory --weights runs/train/exp/weights/best.pt
```
This will run the object detection model on the provided image(s) and display the results with license plate bounding boxes.
WandB Dashboard
During training and evaluation, you can monitor the progress and metrics using the WandB dashboard. Simply create a free WandB account, and the dashboard will be automatically updated with the latest results.
Contributing
If you would like to contribute to this project, please open an issue or submit a pull request with your proposed changes.
License
This project is licensed under the MIT License.

This README file provides an overview of the project, instructions for setting up the environment, training the model, evaluating the model, running inference, and monitoring the progress using the WandB dashboard. It also includes information about contributing to the project and the license.

Feel free to modify the content according to your specific requirements and add any additional sections or details as needed.
