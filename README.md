# Face and Eye Detection Game

This is a simple Python script using OpenCV for face and eye detection. The program captures video frames from the default camera and detects faces and eyes in real-time. It includes a basic game where the user needs to press 's' to start when two eyes are detected on their face.

## How It Works

The script uses OpenCV for computer vision tasks:

1. It loads pre-trained Haar Cascade classifiers for face and eye detection.
2. The program continuously captures video frames from the default camera.
3. For each frame, it converts the frame to grayscale and applies bilateral filtering for noise reduction.
4. It detects faces using the face cascade classifier and draws rectangles around the detected faces.
5. For each detected face, it defines regions of interest (ROI) in both grayscale and color.
6. It attempts to detect eyes within each face region using the eye cascade classifier.
7. If at least two eyes are detected, it prompts the user to press 's' to start the game. If the user presses 's', it prints a message. If fewer than two eyes are detected, it indicates that no eyes are detected or the user loses the game.

## Library Used

- [NumPy](https://numpy.org/): For numerical operations.
- [OpenCV (cv2)](https://opencv.org/): For computer vision tasks, including face and eye detection.

## How to Run

1. **Install Dependencies:**
   - Make sure you have Python installed on your system.
   - Install the required libraries by running:
     ```bash
     pip install numpy opencv-python
     ```

2. **Run the Script:**
   - Clone this repository:
     ```bash
     git clone https://github.com/harika-haru/Blink_detection.git
     cd face-eye-detection-game
     ```
   - Run the script:
     ```bash
     python face_eye_detection_game.py
     ```
   - Press 's' to start the game when prompted.

3. **Exit the Program:**
   - Press 'q' to exit the program at any time.

## Acknowledgments

This project is inspired by [OpenCV's face detection tutorial](https://docs.opencv.org/master/db/d28/tutorial_cascade_classifier.html).

Feel free to contribute, report issues, or suggest improvements!
