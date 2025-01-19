# Eyes Detection with OpenCV
# [Youtube Channel](https://www.youtube.com/channel/UCrT5u-1_J1ogG4l0TKhj21g) | [Linkedin](https://www.linkedin.com/in/noureddin-sameer-45760a236/)
# Drowsiness Detection System

This system utilizes computer vision techniques to monitor the driver's state, specifically focusing on the detection of potential drowsiness or loss of consciousness. By analyzing real-time video feed from a camera, the system aims to identify instances where the driver may be at risk due to inattentiveness or unconsciousness.

This code implements a drowsiness detection system using OpenCV (Open Source Computer Vision Library). It aims to enhance driver safety by detecting eye closures and triggering an alarm in such scenarios.

# Installation

Install OpenCV:
* Using pip: `pip install opencv-python`
* Using conda: `conda install -c conda-forge opencv`

# Dependencies
* OpenCV (cv2)
* winsound (for alarm sound on Windows)
* Code Structure

# Explanation

>Imports: Necessary libraries are imported.

>sound_alarm function: Plays an alarm sound when eyes are closed.

>Cascade Classifiers: Pre-trained classifiers for eye and face detection are loaded.

>Video Capture: Initializes the webcam for capturing video frames.

Main Loop:
Reads a frame from the camera.
Converts the frame to grayscale for improved detection.
Detects eyes and faces using the cascade classifiers.

Checks if eyes are closed (no eyes detected or no face detected):
Prints a message and displays text on the frame indicating drowsiness.
Triggers the alarm sound.

Otherwise, prints a message and displays text indicating the driver is likely awake.
Draws rectangles around detected eyes (for visualization).
Displays the frame with detection results.

Exits the loop on 'q' key press.

Resource Release: Releases the video capture object and closes windows.
Usage

Save the code as a Python file (e.g., drowsiness_detection.py).

Run the script from your terminal: python drowsiness_detection.py
Customization

Alarm Sound: Modify the sound_alarm function to play
