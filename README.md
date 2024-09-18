**Objective:** Detect and highlight lane lines in images or video streams from a camera. This involves preprocessing, edge detection, region of interest (ROI) masking, and line detection using Hough Transform.
Tools & Libraries: OpenCV for computer vision tasks, NumPy for numerical operations, and Matplotlib for visualizations.
**Steps and Techniques**

**Image Preprocessing:**

Grayscale Conversion: Convert the input image to grayscale to simplify the subsequent processing steps.
Gaussian Blur: Apply Gaussian blur to reduce noise and improve edge detection.

**Edge Detection:**

Canny Edge Detection: Use the Canny edge detection algorithm to identify edges in the image. This is crucial for detecting lane lines.
Region of Interest (ROI) Masking:

Define ROI: Create a mask to focus on the region where lanes are expected (e.g., lower half of the image). This reduces computational complexity and improves detection accuracy.
Line Detection:

Hough Line Transform: Apply the Hough Line Transform to detect lines in the edge-detected image. This algorithm finds lines by mapping points in the image space to a parameter space.
Lane Marking:

Overlay Lane Lines: Draw the detected lane lines on the original image to visualize the results.
Real-time Processing:

Video Stream: Extend the approach to process video streams for real-time lane detection. This involves reading frames from a video, applying the lane detection pipeline, and displaying the results.

**Results**

Visualize detected lanes overlaid on the original images or video frames.
Assess performance based on detection accuracy and robustness under varying conditions (e.g., different lighting, weather).

**Usage**

Setup: Ensure OpenCV and other dependencies are installed.
Run the Script: Execute the provided script to detect lanes in a static image or video file.
Real-time Application: Modify the script for real-time lane detection using a webcam.
This project provides a comprehensive approach to lane detection, useful for enhancing vehicle safety and autonomy.
