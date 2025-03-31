# Real-Time-Face-Detection 
This MATLAB script demonstrates a real-time face detection and tracking system using a webcam. The script utilizes computer vision tools to detect and track a user's face within a video stream.
 
Prerequisites

MATLAB: You need to have MATLAB installed on your computer. The code was developed and tested on MATLAB.
 
Computer Vision System Toolbox: Ensure that you have the Computer Vision System Toolbox installed, which is necessary for utilizing the built-in functions and objects for face detection and tracking.
 
Webcam: You need a webcam connected to your computer to capture the video stream for face detection and tracking. The code is configured to use the default webcam.
 
Running the Code
Follow these steps to run the code:
 
1.    Open MATLAB: Start MATLAB on your computer.
 
2.    Set Webcam Resolution (Optional): By default, the script sets the webcam resolution to 1280x720. You can modify this resolution by changing the cam.Resolution property to your desired resolution.
 
3.    Run the Script: Open the MATLAB script and run it. You can do this by opening the script file and clicking the "Run" button or typing run in the MATLAB command window.
 
4.    Face Detection and Tracking: 
            Stepwise explanation of how the code works:
      i. Initialization: The script initializes all necessary components, including the webcam,video player, face detector, and point tracker.
      ii. Capture the First Frame: The first video frame from the webcam is captured.
      iii. Main Loop: The script enters a loop where it will continue running until the loop is closed or a specified number of frames are processed (default is 400 frames).
      iv.Frame Processing:
      v.Face Detection: If there are not enough tracked points (less than 10), the code attempts to detect a face in the grayscale frame. If a face is found, it proceeds to detect feature points within the face region.
     vi. Feature Point Tracking: If there are enough feature points, the script uses the point tracker to track these points as they move. A similarity transformation is estimated, and the tracked points are updated.
    vii.Display and Visualization: In each frame, the code visualizes the detected face with a polygon and the tracked feature points on the video frame.
    viii.Loop Termination: The loop continues running until the video player is closed or the specified number of frames have been processed.
 
In summary, the code will start capturing the video from your webcam and initiate face detection and tracking. It will display the video stream with detected faces outlined in real-time.
 
5.    Quit the Application: To exit the application, you can simply close the video player window, or you can stop the code execution within MATLAB.
 
Troubleshooting
a.    If you encounter any errors during script execution, please ensure that you have met the prerequisites mentioned above and that the code is correctly configured.
 
b.    Make sure your webcam is working and properly connected.
 
Important Notes
i.  The code is set to run for a limited number of frames (400 frames by default). You can modify the ‘frame_count’ value to adjust this.
 
ii. The system may perform best in well-lit conditions to ensure accurate face detection.
 
iii.This code serves as a basic demonstration of real-time face detection and tracking. We can modify and extend it to suit our specific requirements or integrate it into larger projects.
 
Please note that this README provides a basic overview of how to run the code. For more detailed information about each part of the code and its functionality, you can refer to the code comments.
 
 
 
 
