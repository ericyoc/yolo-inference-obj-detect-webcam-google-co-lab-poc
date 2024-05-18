# Real-Time Object Detection with YOLOv8

This repository contains a Python script that demonstrates real-time object detection using the YOLOv8 pre-trained model. The script utilizes the YOLOv8 model to identify objects in a live video stream captured from the user's webcam. It provides a user-friendly interface with buttons for capturing images, toggling single object detection, and exiting the program.

## Features

- Real-time object detection using the YOLOv8 pre-trained model
- Webcam integration for live video stream
- Bounding box and label visualization for detected objects
- Single object detection mode to focus on the last detected object
- Image capture functionality with customizable filenames based on detected objects
- Exit button to gracefully terminate the program
- Integration with Google Colab for easy setup and execution

## YOLOv8 Pre-trained Model

The script utilizes the YOLOv8 (You Only Look Once version 8) pre-trained model for object detection. YOLOv8 is a state-of-the-art object detection model known for its high accuracy and real-time performance. It is capable of detecting a wide range of objects across various categories, including but not limited to:

- Person
- Car
- Truck
- Bicycle
- Motorcycle
- Bus
- Train
- Airplane
- Boat
- Traffic light
- Fire hydrant
- Stop sign
- Parking meter
- Bench
- Bird
- Cat
- Dog
- Horse
- Sheep
- Cow
- Elephant
- Bear
- Zebra
- Giraffe
- Backpack
- Umbrella
- Handbag
- Tie
- Suitcase
- Frisbee
- Skis
- Snowboard
- Sports ball
- Kite
- Baseball bat
- Baseball glove
- Skateboard
- Surfboard
- Tennis racket
- Bottle
- Wine glass
- Cup
- Fork
- Knife
- Spoon
- Bowl
- Banana
- Apple
- Sandwich
- Orange
- Broccoli
- Carrot
- Hot dog
- Pizza
- Donut
- Cake

For a complete list of objects that YOLOv8 can identify, please refer to the COCO dataset classes. [COCO Dataset Information ](https://docs.ultralytics.com/datasets/detect/coco/)

## Confidence Threshold and Object Identification

To ensure accurate object identification, the script allows you to set a confidence threshold. The confidence threshold determines the minimum confidence score required for an object detection to be considered valid. By default, the confidence threshold is set to 0.5, meaning that only detections with a confidence score of 0.5 or higher will be displayed and considered for further processing.

Adjusting the confidence threshold can help in reducing false positive detections and focusing on the most probable objects in the scene. A higher confidence threshold will result in fewer but more confident detections, while a lower threshold may include more detections but with a higher chance of false positives.

## GPU Acceleration

The script is designed to leverage GPU acceleration when running on a compatible device. By setting the `device` parameter to `'cuda'` in the `model()` function, the script utilizes the GPU for faster inference and improved performance. If a GPU is not available, the script will automatically fallback to using the CPU for object detection.

Please note that GPU acceleration requires the necessary dependencies and drivers to be installed on your system.

## Disclaimer

This repository is intended for educational and research purposes only. The use of the YOLOv8 model and the provided script should comply with the terms and conditions of the original authors and any applicable licenses. The authors of this repository are not responsible for any misuse or unintended consequences resulting from the use of this code.

Please use the code responsibly and respect the intellectual property rights of others.
