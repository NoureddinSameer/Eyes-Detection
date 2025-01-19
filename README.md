# Eyes Detection with OpenCV
# [Youtube Channel](https://www.youtube.com/channel/UCrT5u-1_J1ogG4l0TKhj21g) | [Linkedin](https://www.linkedin.com/in/noureddin-sameer-45760a236/)


This program utilizes computer vision techniques to monitor the driver's state, specifically focusing on detecting potential drowsiness or loss of consciousness. By analyzing a real-time video feed from a camera, the program identifies instances where the driver may be at risk due to inattentiveness or unconsciousness.

The code uses **OpenCV** (Open Source Computer Vision Library) to detect eyes, and `winsound` to generate an alarm to wake the driver in case of potential drowsiness.


### Features
* **Real-Time Monitoring:** Detects eye and face states using a webcam.
* **Audio Alarm:** Alerts the driver with a sound alarm when drowsiness is detected.
* **User-Friendly Output:** Displays visual feedback (messages and bounding boxes) on the video feed.


### Prerequisites
* **Python Version:** `Python 3.9.13` (recommended).



### Dependencies
**Ensure the following libraries are installed:**
- **OpenCV (`cv2`):** For video processing and face/eye detection.

  - **Install via pip:** ```pip install opencv-python```



### How to Use?
1. Save the code as `Detection.py` file

2. Run the program using `cmd`: `python Detection.py`

3. The program will detect drowsiness in real-time:
   - Displays **Eyes open** and **The Driver is Awake** if eyes are detected.
   - Displays **Eyes closed** and **The Driver is Sleeping** with an alarm if no eyes are detected.

4. Press the `q` key to exit the program.



### How It Works?
1. **Eye and Face Detection:**
   - Uses pre-trained Haar cascade models for detecting faces and eyes.
     
2. **Grayscale Conversion:**
   - Converts video frames to grayscale for better detection accuracy.

3. **Drowsiness Detection:**
   - If no eyes or faces are detected, the program assumes the driver is drowsy and triggers an alarm.

4. **Visual Feedback:**
   - Displays messages and bounding boxes for easy monitoring.



### Customization
1. **Alarm Sound:**
   - Modify the `sound_alarm` function to use a custom alarm or a different sound frequency/duration.

2. **Detection Parameters:**
   - Fine-tune the parameters in the `detectMultiScale` method for better accuracy based on your environment.

