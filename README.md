# **ParkFinder: Parking Space Monitoring System**

**ParkFinder** is a real-time parking space monitoring system that uses **OpenCV** to analyze a video feed from a car park, detecting free and occupied parking spaces. The system processes video frames, applies image processing techniques, and provides real-time parking availability updates.

## **How it Works**
1. The system loads a video feed (e.g., `carPark.mp4`) and predefined parking space positions (stored in `CarParkPos` using Pickle).
2. It processes each video frame by converting it to grayscale, applying Gaussian Blur, adaptive thresholding, median blur, and dilation to detect parking spaces.
3. The system counts non-zero pixels in each parking space to determine if it’s free or occupied.
4. The output video displays rectangles around each parking space, indicating its status.

## **Libraries Used**
- **Python 3.x**
- **OpenCV (cv2)**: For image processing and video feed handling.
- **NumPy**: For numerical operations.
- **Pickle**: For serializing and loading parking space position data.
- **CVZone**: For enhanced computer vision functionality.

## **References**
- [OpenCV](https://opencv.org/)
- [NumPy](https://numpy.org/)
- [Pickle](https://docs.python.org/3/library/pickle.html)
- [CVZone](https://github.com/cvzone/cvzone)
