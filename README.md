# Car Number Plate Detection

A Python and OpenCV project that detects possible vehicle number-plate regions from a live webcam feed using a Haar Cascade classifier.

## Demo

The application highlights detected number-plate regions with green bounding boxes.

![Car Number Plate Detection Demo](screenshot\detection_result.png)

## Features

- Live webcam-based detection
- Grayscale image processing
- Green bounding boxes around candidate plates
- Haar Cascade model for plate detection

## Project Structure

```text
car-number-plate-detection/
├── model/
│   └── haarcascade_russion_plate_number.xml
├── screenshots/
│   └── detection_result.png
├── number_plate.py
├── requirements.txt
└── README.md
```

## Installation and Usage

**Requirements:** Python 3.9+, OpenCV, and a working webcam.

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Run the application:

```bash
python number_plate.py
```

**Controls:** Use `Ctrl + C` in the terminal to interrupt execution.

## Limitations

- Detects possible plate regions but does not recognize registration numbers as text (OCR).
- May produce false detections depending on lighting, angle, distance, and background.
- Performance on Indian number plates may vary with the Haar Cascade model.

## Future Improvements

- Add OCR to extract registration numbers.
- Improve detection accuracy and reduce false positives.
- Evaluate performance on a collection of vehicle images.