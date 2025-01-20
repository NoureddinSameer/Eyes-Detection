# Eyes Detection with OpenCV
# [Youtube Channel](https://www.youtube.com/channel/UCrT5u-1_J1ogG4l0TKhj21g) | [Linkedin](https://www.linkedin.com/in/noureddin-sameer-45760a236/)

## Drowsiness Detection program

This program utilizes computer vision techniques to monitor the driver's state, specifically focusing on detecting potential drowsiness or loss of consciousness. By analyzing a real-time video feed from a camera, the program identifies instances where the driver may be at risk due to inattentiveness or unconsciousness.

The code uses **OpenCV** (Open Source Computer Vision Library) to detect eyes, and `winsound` to generate an alarm to wake the driver in case of potential drowsiness.

</br></br>

### Features
* **Real-Time Monitoring:** Detects eye and face states using a webcam.
* **Audio Alarm:** Alerts the driver with a sound alarm when drowsiness is detected.
* **User-Friendly Output:** Displays visual feedback (messages and bounding boxes) on the video feed.

</br></br>

### Prerequisites
* **Python Version:** `Python 3.9.13` (recommended).

</br></br>

### Dependencies
**Ensure the following libraries are installed:**
- **OpenCV (`cv2`):** For video processing and face/eye detection.

  - **Install via pip:** ```pip install opencv-python```

</br></br>

### How to Use?

**Option 1: Run the Program Directly**
1. Save the code as `Detection.py` file

</br>

**Option 2: Clone from Repository**
1. **Clone the repository:**
   - `git clone https://github.com/NoureddinSameer/Eyes-Detection-with-OpenCV.git`
2. **Navigate to the cloned directory:** `cd <repository-folder>` 

</br></br>

**Run the program**
* **Use the command prompt to execute the program:**`python Detection.py`**


</br></br>

**Program Functionality**

* **The program will detect drowsiness in real-time:**
   - **If eyes are open and detected:**
     - Displays **Eyes open** and **The Driver is Awake**.
       
   - **If eyes are closed or not detected:**
     - Displays **Eyes closed** and **The Driver is Sleeping** and **activates an alarm**.

</br></br>


**Exit the Program**
* **Press the `q` key to stop the program.**



</br></br>

### How It Works?
1. **Eye and Face Detection:**
   - Uses pre-trained Haar cascade models for detecting faces and eyes.
     
2. **Grayscale Conversion:**
   - Converts video frames to grayscale for better detection accuracy.

3. **Drowsiness Detection:**
   - If no eyes or faces are detected, the program assumes the driver is drowsy and triggers an alarm.

4. **Visual Feedback:**
   - Displays messages and bounding boxes for easy monitoring.

</br></br>

### Customization
1. **Alarm Sound:**
   - Modify the `sound_alarm` function to use a custom alarm or a different sound frequency/duration.

2. **Detection Parameters:**
   - Fine-tune the parameters in the `detectMultiScale` method for better accuracy based on your environment.

