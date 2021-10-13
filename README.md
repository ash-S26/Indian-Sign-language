# Indian-Sign-language
_________________________
The project is based on idea of detection of indian sign language. This is a computer vision based project which detects what the hand is showing using certain algorithm as described below.

# Dependencies/pakage
________________________
  1) opencv - pip install opencv-python

# Algorithm
____________
   1) Seperate out the skin color from the input frame (captured through attached camera) using HSV or other color format with upper and lower bound for skin color as per range.
   2) Removal of noise from image via dialation and errosion, and applying filters to smooothen the image.
   3) Finding the contour of the mask(seperated skin color mask) and drawing convex-hull.
   4) Using the various properties for seperation various Hand_Gestures(In this project we will use Indian-sign-language as Hand_Gesture- 1,2,3..) like-
      - Finding the extreme most points of contours and computing angle between bottommost and other extreme points and using the values in if loop.
      - Finding the corner points of hull.
      - Finding number of lines in contour of specific gesture.
      - Area of contour for different gestures.
      
# How to run the code
_______________________
    1) git clone 
    2) python 
    
# Results
___________
![](https://github.com/ash-S26/Indian-Sign-language/blob/main/results/HAND_GESTURE_DETECTION.gif)
