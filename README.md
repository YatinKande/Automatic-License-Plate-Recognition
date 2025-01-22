Automatic License Plate Recognition (ANPR) 🚘
===
The project deals with ANPR, which is the detection and recognition of license plates from vehicle images with the help of advanced image processing techniques. The focus will be on the optimization of the pre-processing steps and OCR accuracy by fine-tuning edge detection and filtering techniques to correctly extract alphanumerical data from license plates.

## Features
- Applied image preprocessing techniques, including bilateral filtering and Gaussian blur, for noise reduction.

- Implemented edge detection methods like Canny edge detection to enhance plate contours.

- Utilized morphological operations for improved plate isolation and text recognition.

- Evaluated OCR performance under different conditions to achieve accurate text extraction.

- Conducted parameter tuning to optimize filter values and edge detection thresholds.

## Preprocessing Techniques Used

- Bilateral Filtering: Applied with different parameter values to balance edge enhancement and noise reduction.

- Gaussian Blur: Used to reduce noise while preserving edges.

- Canny Edge Detection: Applied with varying thresholds to identify strong edges.

- Morphological Operations: Dilation and erosion used to enhance contours and reduce false positives.

## Performance Summary

| Image | Preprocessing Method | OCR Accuracy | Key ObservaItion |
| --- | --- | --- | --- |
|ANPR1|Bilateral Filter (45,100,100), Canny (40,300)|Medium|Misidentifies characters due to pixelation|
|ANPR2|Gaussian Blur (5,5), Canny (50,300)|Good|Perfect OCR accuracy with robust preprocessing|
|ANPR3|Bilateral Filter (45,100,100), Canny (40,300)|Medium|Pixelation affects OCR accuracy|
|ANPR4|Bilateral Filter (35,95,75), Canny (30,100)|Medium|Contour detection complexity increases|
|ANPR5|Bilateral Filter (35,95,75), Canny (30,150)|Good|Accurate OCR, robust performance|
|ANPR6|Bilateral Filter (35,95,75), Canny (30,150)|Good|Reliable isolation and text recognition|
|ANPR7|Bilateral Filter (80,100,80), Canny (30,200)|Poor|Incorrect segmentation, unclear output|

## Install & Dependence
- easyocr
- imutils

## Use
- Navigate to the project directory:
  ```
  cd ANPR/
  ```
- Run the main Python file to start the simulation:
  ```
  python ANPR1.py
  ```
## Code Details

### Tested Platform

- software
  ```
  OS: macOS (MacBook Pro M4 Pro)
  Python: 3.12.7(anaconda)
  ```
- hardware
  ```
  CPU: Apple M4 Pro (12-core)
  GPU: Apple M4 Pro GPU (18-core)
  ```

## Images 
![Watch the video](https://drive.google.com/file/d/1oiag7NzsZJismlO4Z_CMTzZ-nXDf9ZfG/view?usp=share_link)

## References
The code used in this project was inspired by the following YouTube tutorial:
[Automatic License Plate Recognition Tutorial](https://www.youtube.com/watch?v=NApYP_5wlKY)

## License

This project is licensed under the MIT License. See the LICENSE file for details.
