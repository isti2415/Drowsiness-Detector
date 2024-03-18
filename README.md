# Drowsiness Detector

![Drowsiness Detector](https://img.shields.io/badge/Drowsiness-Detector-blue)

## Overview

The Drowsiness Detector is a computer vision project aimed at detecting drowsiness and yawning in individuals using webcam feeds. This project utilizes TensorFlow, OpenCV, and Keras libraries for implementing the detection algorithms. Haar cascades are employed to identify the movements of eyes and mouth, determining whether the person is getting drowsy or yawning.

## Features

- Detects drowsiness and yawning in real-time using webcam feed.
- Utilizes TensorFlow, OpenCV, and Keras for implementing the detection algorithms.
- Alarm is set off if a person is drowsy for more than 10 frames consecutively.

## Dataset

The dataset used for training and testing contains 725 labeled images per category and is categorized into the following classes:
- "Open"
- "Close"
- "Yawn"
- "No_yawn"

These images represent various states of eyes and mouth movements, crucial for training the detection model.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/isti2415/drowsiness-detection.git
   ```

2. Open the .ipynb files in your local jupyter notebook compiler.

## Training the Model

1. Open the `model.ipynb` file in Jupyter Notebook or any compatible environment.

2. Follow the instructions in the notebook to train the detection model using the provided dataset.

## Running the Software

1. Open the `drowsiness.ipynb` file in Jupyter Notebook or any compatible environment.

2. Run the cells in the notebook to execute the Drowsiness Detector software.

## How it Works

The Drowsiness Detector employs a multi-step process to detect drowsiness and yawning:

1. **Face Detection**: Utilizes Haar cascades to detect faces in the webcam feed.

2. **Eye and Mouth Detection**: Once a face is detected, the regions of interest (eyes and mouth) are identified within the face region.

3. **Feature Extraction**: Extracts relevant features from the eye and mouth regions to determine their states (open, closed, yawning, not yawning).

4. **Drowsiness Detection**: Analyzes the temporal sequence of eye and mouth states to determine if the person is getting drowsy or yawning.

5. **Alarm Triggering**: If the person is identified as drowsy for more than 10 consecutive frames, an alarm is triggered to alert the individual.

## Contributing

Contributions are welcome! Please feel free to open a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- The Drowsiness Detector project is inspired by the work done in the field of computer vision for driver monitoring systems.
- Special thanks to the developers and contributors of TensorFlow, OpenCV, and Keras for their invaluable libraries and documentation.
