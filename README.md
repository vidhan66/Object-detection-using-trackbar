# Selective Object Detection in Robotics Project

This project is designed to address common challenges in object detection for robotics by allowing users to manually select the objects they want to track. Traditional object detection techniques using contours and bounding rectangles often detect unwanted objects, leading to inaccuracies. This project solves that problem by using a manual selection method where users specify exactly which objects to detect, resulting in more precise tracking.

## Features

- **Manual Object Selection**: Users can manually select the number of objects they want to track, avoiding detection of irrelevant items.
- **Real-Time Tracking**: Objects are tracked in real time using the MIL tracker from OpenCV, providing a smooth and interactive experience.
- **Customizable Tracking**: Allows dynamic input for the number of objects to be tracked, providing flexibility based on the user's needs.

## How It Works

1. The system initializes a video capture using your computer's default camera.
2. The user is prompted to enter the number of objects they wish to detect.
3. In the first frame, the user manually selects each object by drawing bounding boxes.
4. The program initializes a separate tracker for each object and begins tracking them in subsequent frames.
5. The bounding boxes are updated in real time, and each object is labeled for easy identification.
6. After selecting a object press enter to select another object.

## Dependencies

- Python 3.x
- OpenCV

Install OpenCV using pip:

```bash
pip install opencv-python
