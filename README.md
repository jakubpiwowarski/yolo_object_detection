# Object Detection using YOLO
This script implements object detection using the YOLO (You Only Look Once) model. It utilizes the Ultralytics library, which provides an interface for using the YOLO model. The script supports both webcam input and video playback from a file.

## Features
-Initialization of webcam or video player.
-Initialization of the YOLO model using pre-trained weights.
-Detection and tracking of objects on the current frames.
-Drawing bounding boxes around the detected objects.
=Displaying labels with class names and detection confidence.

## Required Libraries
-ultralytics: Library containing the YOLO implementation and interface for using it.
-cv2: OpenCV library for image and video manipulation.
-cvzone: Library for drawing rectangles and text on images.
-math: Mathematical library for auxiliary calculations.

## Configuration
-Option to choose between a webcam and a video player.
-Selection of the YOLO model using a weight file (in this case, 'yolov8n.pt').
-Definition of a list of class names that the model is capable of detecting (a total of 91 classes).

## Main Loop
1. Read the next frame from the webcam or video player.
2. Call the model() method to perform object detection on the frame.
3. Iterate through the detection results and draw bounding boxes and labels for each detected object.
4. Display the updated frame with the drawn bounding boxes and labels.
5. Wait for user input to exit the program (keypress).

## Useful Information
-The script uses the YOLO model with pre-trained weights 'yolov8n.pt'.
-The list of class names that the model can detect is defined in the classNames variable.
-The cvzone library is used for drawing rectangles and labels on the frames.

### Note: Before running the script, ensure that the required libraries are installed.
