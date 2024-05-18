# Real-Time Object Detection with Webcam and Integration with Google Co-lab

This repository contains a Python script that demonstrates real-time object detection using the YOLOv8 pre-trained model. The script utilizes the YOLOv8 model to identify objects in a live video stream captured from the user's webcam. It provides a user-friendly interface with buttons for capturing images, toggling single object detection, and exiting the program.

## Motivating Articles and Related Work
Lin, T. Y., Maire, M., Belongie, S., Hays, J., Perona, P., Ramanan, D., ... & Zitnick, C. L. (2014). Microsoft coco: Common objects in context. In Computer Vision–ECCV 2014: 13th European Conference, Zurich, Switzerland, September 6-12, 2014, Proceedings, Part V 13 (pp. 740-755). Springer International Publishing. https://link.springer.com/chapter/10.1007/978-3-319-10602-1_48

Zhou, Y. (2024). A yolo-nl object detector for real-time detection. Expert Systems with Applications, 238, 122256. https://www.sciencedirect.com/science/article/abs/pii/S0957417423027586

Vijayakumar, A., & Vairavasundaram, S. (2024). YOLO-based Object Detection Models: A Review and its Applications. Multimedia Tools and Applications, 1-40. https://link.springer.com/article/10.1007/s11042-024-18872-y

## Toolbox

YOLO Docs https://docs.ultralytics.com/

YOLO GitHub https://github.com/ultralytics/ultralytics

## Features

- Real-time object detection using the YOLOv8 pre-trained model
- Webcam integration for live video stream
- Bounding box and label visualization for detected objects
- Single object detection mode to focus on the last detected object
- Image capture functionality with customizable filenames based on detected objects
- Exit button to gracefully terminate the program
- Integration with Google Colab for easy setup and execution

## Results
### Person and Scissors Detected
![](https://github.com/ericyoc/yolo-inference-obj-detect-webcam-google-co-lab-poc/blob/main/person__0.95_scissors__0.95.jpg)

### Person and Bottle Detected
![](https://github.com/ericyoc/yolo-inference-obj-detect-webcam-google-co-lab-poc/blob/main/person__0.96_bottle__0.89.jpg)

### Person and Cup Detected
![](https://github.com/ericyoc/yolo-inference-obj-detect-webcam-google-co-lab-poc/blob/main/person__0.97_cup__0.94.jpg)

### Only Bottle Detected
![](https://github.com/ericyoc/yolo-inference-obj-detect-webcam-google-co-lab-poc/blob/main/bottle_0.86.jpg)

## YOLOv8 Pre-trained Model

The script utilizes the YOLOv8 (You Only Look Once version 8) pre-trained model for object detection. YOLOv8 is a state-of-the-art object detection model known for its high accuracy and real-time performance. It is capable of detecting a wide range of objects across various categories. For a complete list of objects that YOLOv8 can identify, please refer to the COCO dataset classes. [COCO Dataset Information ](https://docs.ultralytics.com/datasets/detect/coco/#dataset-yaml)

## Confidence Threshold and Object Identification

To ensure accurate object identification, the script allows you to set a confidence threshold. The confidence threshold determines the minimum confidence score required for an object detection to be considered valid. By default, the confidence threshold is set to 0.5, meaning that only detections with a confidence score of 0.5 or higher will be displayed and considered for further processing.

Adjusting the confidence threshold can help in reducing false positive detections and focusing on the most probable objects in the scene. A higher confidence threshold will result in fewer but more confident detections, while a lower threshold may include more detections but with a higher chance of false positives.

## GPU Acceleration

The script is designed to leverage GPU acceleration when running on a compatible device. By setting the `device` parameter to `'cuda'` in the `model()` function, the script utilizes the GPU for faster inference and improved performance. If a GPU is not available, the script will automatically fallback to using the CPU for object detection.

Please note that GPU acceleration requires the necessary dependencies and drivers to be installed on your system.

## Disclaimer

This repository is intended for educational and research purposes only. The use of the YOLOv8 model and the provided script should comply with the terms and conditions of the original authors and any applicable licenses. The authors of this repository are not responsible for any misuse or unintended consequences resulting from the use of this code.

Please use the code responsibly and respect the intellectual property rights of others.
