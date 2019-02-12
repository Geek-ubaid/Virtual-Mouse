# Virtual Mouse
A gesture controlled Mouse Module.

## Description
In this project, the mouse cursor movement and click events are controlled using a camera based on colour
detection and segmentation technique. Here real time video has been captured using a Web- Camera. The
user wears coloured tapes to provide information to the system. Individual frames of the video are
separately processed. The processing techniques involve an image subtraction algorithm to detect colours.
Once the colours are detected, the system performs various operations to track the cursor and performs
control actions.

## Methodology
The project works on the concept of colour segmentation. The colour detected are mapped on the live cam
feed and are processed to find the appropriate gesture. The methods and concept used are:
- For Image Processing:
-- Thresholding
-- Segmentation
-- Contouring
--  Morphological Transformations (Dilation/Erosion)
- For Gesture Recognition:
-- Calculated Centroid DIstance
-- Detected the no of contours
-- Calculated maximum area of the contours detected
- For Mouse actions:
-- Maintained the aspect ratio of screen
-- Creating a stack of action for smooth execution of action
-- Mapped the mouse pointer to the movement of contours

## Dependencies
- opencv
- pyautogui
