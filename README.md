Real-Time Object Detection using OpenCV and SSD MobileNet v3


   This Python script utilizes OpenCV's deep neural network module to perform real-time object detection using the SSD MobileNet v3 model trained on the COCO dataset. The program is capable of detecting various objects in images or videos, drawing bounding boxes around them, and labeling each detected object.

Table of Contents
Setup Instructions
Usage
Example
Additional Notes
Setup Instructions
Prerequisites
Python 3.x
OpenCV (cv2)
Matplotlib
Installation Steps
Clone or download the repository.
Install the required dependencies using pip:

pip install opencv-python matplotlib

Usage
Model Files: Ensure the model files (frozen_inference_graph.pb and ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt) are available.

Labels File: Prepare a labels.txt file containing the class labels corresponding to the COCO dataset.

Configure Variables: Update the following variables in the code:

cnfig_file: Path to the ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt file.
frozen_model: Path to the frozen_inference_graph.pb file.
file_name: Path to the labels.txt file containing class labels.
Ensure the input image/video path matches the filename used in the code (image.jpg and output.mp4).
Run the Script: Execute the Python script.

Example
Detect Objects in an Image:

python object_detection.py
Detect Objects in a Video:

python object_detection.py
(Ensure the video file is named output.mp4 or modify the code accordingly.)

Additional Notes
Adjust Confidence Threshold: Modify the confidence threshold (confThreshold) for object detection as needed.

Camera Usage: If no video file is found, the program switches to the webcam for real-time detection.

Exiting the Program: Press 'q' to exit the real-time video detection.

