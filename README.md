# Virtual-Mouse-Using-Finger
  This project demonstrates how to control the mouse cursor using hand gestures, specifically tracking the index finger and thumb using a webcam. The implementation leverages OpenCV for video capture, MediaPipe for hand tracking, and PyAutoGUI for simulating mouse events.

## Features

- **Index Finger Tracking**: The index finger is tracked to move the mouse cursor on the screen.
- **Click Detection**: When the index finger and thumb come close together, a mouse click is simulated.

## Requirements

- Python 3.x
- OpenCV (`opencv-python`)
- MediaPipe
- PyAutoGUI

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/virtual-mouse.git
   cd virtual-mouse

 2. Install the required Python packages:
    ```bash
    pip install opencv-python mediapipe pyautogui

  ## Usage
  Run the script using Python:
  
      python virtual_mouse.py

  ## How It Works
  1. Video Capture: The webcam captures the video, which is processed frame by frame.
  2. Hand Detection: MediaPipe is used to detect hands and extract the landmarks.
  3. Cursor Movement: The coordinates of the index finger are mapped to the screen coordinates, and PyAutoGUI moves the mouse cursor accordingly.
  4. Click Simulation: A mouse click is simulated when the distance between the index finger and thumb is below a certain threshold.

  ## Limitations
  - The system relies on a good lighting condition and a clear background for accurate hand detection.
  - The click detection might be sensitive and may require calibration based on the user's preference.

  ## Future Improvements
  - Implementing more gestures for different mouse actions like right-click, scrolling, etc.
  - Adding support for multiple hands and gestures.

  ## License
  This project is licensed under the MIT License. See the LICENSE file for details.

  ## Acknowledgements
  - MediaPipe by Google for providing a powerful hand tracking solution.
  - OpenCV for computer vision capabilities.
  - PyAutoGUI for simulating mouse and keyboard actions.

    ```bash
      This `README.md` file provides a comprehensive overview of your project, including installation instructions, usage, and a brief explanation of the code. Make sure to replace the repository URL and any other placeholders with actual values specific to your project.
