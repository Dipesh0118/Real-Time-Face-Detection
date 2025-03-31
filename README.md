# Real-Time Face Detection

This MATLAB script demonstrates a real-time face detection and tracking system using a webcam. The script utilizes computer vision tools to detect and track a user's face within a video stream.

---

## Prerequisites

Ensure that you have the following installed and set up before running the script:

- **MATLAB**: The code was developed and tested on MATLAB.
- **Computer Vision System Toolbox**: Required for utilizing built-in functions and objects for face detection and tracking.
- **Webcam**: A webcam must be connected to capture the video stream for face detection and tracking. The code is configured to use the default webcam.

---

## Running the Code

Follow these steps to run the script:

1. **Open MATLAB**: Start MATLAB on your computer.
2. **Set Webcam Resolution (Optional)**: The script sets the webcam resolution to `1280x720` by default. You can modify this by changing the `cam.Resolution` property.
3. **Run the Script**: Open the MATLAB script and execute it by clicking the "Run" button or typing `run` in the MATLAB command window.
4. **Face Detection and Tracking**:
   - **Initialization**: The script initializes necessary components, including the webcam, video player, face detector, and point tracker.
   - **Capture the First Frame**: The first video frame from the webcam is captured.
   - **Main Loop**: The script runs in a loop until manually stopped or until 400 frames are processed (default).
   - **Frame Processing**:
     - **Face Detection**: If there are fewer than 10 tracked points, the script attempts to detect a face in the grayscale frame. If detected, it extracts feature points from the face region.
     - **Feature Point Tracking**: If enough feature points exist, the script tracks them as they move, estimates a similarity transformation, and updates the tracked points.
     - **Display and Visualization**: Detected faces are outlined, and feature points are tracked in real-time on the video stream.
   - **Loop Termination**: The loop continues until the video player is closed or the specified number of frames is processed.
5. **Quit the Application**: Close the video player window or stop the script execution in MATLAB.

---

## Troubleshooting

- If errors occur, ensure all prerequisites are met and the code is correctly configured.
- Check that your webcam is properly connected and functioning.

---

## Important Notes

- The script is configured to run for **400 frames** by default. You can modify the `frame_count` value to extend or reduce this limit.
- The system performs best in **well-lit** conditions for accurate face detection.
- This code serves as a **basic demonstration** of real-time face detection and tracking. You can modify and extend it to suit specific requirements or integrate it into larger projects.

---

### Additional Information

For more details on each part of the code and its functionality, refer to the **comments within the script**.

