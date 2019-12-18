## ros_img_processor
Just a simple template node recievng an image and doing something. Links to OpenCV and ROS wrapped.

## How to run the code
In a terminal window, type:
```sh
$ roslaunch ros_img_processor ros_img_processor.launch
```

## Tip
Check your webcam encodings (yuyv,mjpeg,...) and set them accordingly at file launch/usb_camera.launch

## Circle Detector

Repository forked from :https://github.com/beta-robots/ros_img_processor

The objective of this exercise was to use the previously done Circle Detector code and add it to this project in order to show the unitary vector of a detected circle.
For that, a 3x1 vector has been created where values x and y of the center of the detected circle have been included. Following that, a multiplication between the inverse of the matrixK (which is a 3x3 matrix) and this vector has been made.
The result of this multiplication shows the direction of the vector between the center of the image and the center of the detected circle. 
