# Real-Time Traffic Sign Detection

## Description

This repository contains code for real-time detection and recognition of traffic signs using computer vision techniques. The system is capable of identifying both red and blue traffic signs in real-time video streams.

## Features

- Detection and recognition of red and blue traffic signs
- Real-time processing of video streams
- Integration with SVM classifiers for sign recognition
- Uses MSER (Maximally Stable Extremal Regions) for object detection
- Incorporates Histogram Equalization and Color Segmentation for improved accuracy

## Requirements

- Python 3.x
- OpenCV
- NumPy
- scikit-image
- scikit-learn

## How It Works

- **Training**: The system requires pre-trained SVM classifiers for both red and blue traffic signs. These classifiers are trained using HOG (Histogram of Oriented Gradients) features extracted from a dataset of labeled traffic sign images.

- **Detection**: MSER is utilized to detect potential traffic sign candidates in the input video frames. The detected regions are then filtered based on color segmentation and aspect ratio criteria to isolate potential traffic signs.

- **Recognition**: The isolated traffic sign regions are resized to a standard size and fed into the SVM classifiers for recognition. The classifiers predict the type of traffic sign (e.g., speed limit, stop sign) along with confidence scores.

- **Visualization**: Detected traffic signs are highlighted in the video frames, and the recognized sign labels are overlayed for visualization purposes.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.
