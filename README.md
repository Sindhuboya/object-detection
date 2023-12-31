This project aims to do real-time object detection through a laptop camera or webcam using OpenCV and MobileNetSSD. The idea is to loop over each frame of the video stream, detect objects like person, chair, dog, etc. and bound each detection in a box. Here, we will go through the steps required for setting up the project and some explanation about the code.
How to run this code?

Step 1: Create a directory in your local machine and cd into it


Step 2: Clone the repository and cd into the folder:


Step 3: Install all the necessary libraries. I used MacOS for this project. These are some of the libraries I had to install:

brew install opencv
pip install opencv-python
pip install opencv-contrib-python
pip install opencv-python-headless
pip install opencv-contrib-python-headless
pip install matplotlib
pip install imutils

Make sure to download and install opencv and and opencv-contrib releases for OpenCV 3.3. This ensures that the deep neural network (dnn) module is installed. You must have OpenCV 3.3 (or newer) to run this code.

Step 4: Make sure you have your video devices connected (e.g. Webcam, FaceTime HD Camera, etc.). You can list them by typing this in your terminal



Step 5: To start your video stream and real-time object detection

python real_time_object_detection.py 

Step 6: If you need any help regarding the arguments you pass, try:

python real_time_object_detection.py --help
