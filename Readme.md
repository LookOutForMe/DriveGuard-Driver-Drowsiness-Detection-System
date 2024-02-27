# Driver Drowsiness Detection using Computer Vision

![Drowsiness Detection](https://github.com/LookOutForMe/DriveGuard-Driver-Drowsiness-Detection-System/blob/main/Screenshots/face_detector.png)

This project focuses on preventing accidents due to driver drowsiness by employing computer vision techniques. We utilize Python along with OpenCV and Dlib libraries for efficient drowsiness detection.

## Overview

Drowsy driving is a major cause of road accidents worldwide. Our project aims to mitigate this risk by developing a drowsiness detection system using computer vision. By analyzing facial landmarks and eye movements in real-time, we can alert drivers when signs of drowsiness are detected.

## Technologies Used

- Python
- OpenCV
- Dlib

## How it Works

1. **Facial Landmark Detection**: We use Dlib to detect facial landmarks, which helps us identify key regions such as eyes and mouth. The pre-trained facial landmark detector inside the dlib library is used to estimate  the location of 68 (x, y)-coordinates that map to facial structures on the face. The 68  landmark output is shown in the figure below.
<img src="https://github.com/LookOutForMe/DriveGuard-Driver-Drowsiness-Detection-System/blob/main/Screenshots/face.png">

2. **Eye State Classification**: By monitoring the ratio of eye closure, we can determine whether the driver's eyes are open, closed, or in a drowsy state. The eye is open if Eye Aspect Ratio is greater than 0.25
<img src="https://github.com/LookOutForMe/DriveGuard-Driver-Drowsiness-Detection-System/blob/main/Screenshots/eye.png">

3. **Alert Mechanism**: When drowsiness is detected, the system triggers an alert to notify the driver, potentially preventing accidents.

## Getting Started

1. Clone this repository:

    ```
    git clone https://github.com/LookOutForMe/DriveGuard-Driver-Drowsiness-Detection-System
    ```

2. Install the required dependencies:

    ```
    pip install -r requirements.txt
    ```

3. Run the main script:

    ```
    python drive_guard.py
    ```

**Note:  Download the shape_predictor_68_face_landmarks.dat file from [this link](https://github.com/davisking/dlib-models/blob/master/shape_predictor_68_face_landmarks.dat.bz2).**

## Contributions

Contributions are welcome! Feel free to submit issues or pull requests to enhance the functionality of the drowsiness detection system.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Thanks to the contributors of OpenCV and Dlib for their invaluable libraries.
