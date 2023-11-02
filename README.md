Face Recognition using OpenCV
=============================

This project is a C++ implementation of face recognition using the OpenCV library. The program captures video from the default camera, detects faces in real-time, and saves the cropped face images.

## Overview

### Libraries and Namespaces
- **OpenCV Libraries**: Used for image processing, computer vision tasks, and GUI functions.
- **Standard Libraries**: For input-output operations.
- **Namespaces**: The code uses the `std` and `cv` namespaces.

### Functions
- **Main Function**: Initializes face detection, captures video frames, and applies face detection.
- **detectAndDisplay**: Processes each frame to detect faces, saves the largest detected face, and displays the results.

## Main Features

1. **Cascade Classifier**: The program uses the Haar cascades classifier (`haarcascade_frontalface_alt.xml`) for face detection.
2. **Face Detection**: In each captured frame, all faces are detected. Among all detected faces, the largest one is identified and cropped.
3. **Image Saving**: The cropped face is saved to the `images` directory with an incremental filename.
4. **Real-time Display**: The original frame with a rectangle around detected faces and the cropped face are displayed in real-time.

## Implementation Details

### Main Function
- Initializes the face cascade classifier.
- Captures video from the default camera.
- Reads the video stream in a loop.
- For each frame, applies the `detectAndDisplay` function to detect faces.
- The program can be stopped by pressing the "Esc" key.

### detectAndDisplay Function
- Converts the frame to grayscale and equalizes its histogram.
- Detects faces in the grayscale frame.
- Identifies the largest detected face based on area.
- Crops and saves the largest face to a file.
- Displays the original frame with rectangles around detected faces and the cropped face.

## Reference
The implementation is inspired by a [Code Review StackExchange post](http://codereview.stackexchange.com/questions/28115/opencv-2-4-5-face-detection-c-code-optimization) on face detection optimization.

## Dependencies
- [OpenCV](https://opencv.org/): Ensure you have OpenCV installed and set up to run C++ applications that use the OpenCV library.

## How to Run
(Note: Execution instructions should be added here based on the project's build and run requirements.)

## License
(Note: License information should be added here if available.)

