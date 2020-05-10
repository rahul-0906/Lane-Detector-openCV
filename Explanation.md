# Lane Detector 

### Project Description:
   This Project is based on the Opencv python module.Identifying the lanes in the roads is common task.This is critical task for automonous vehicle to perform.Here This project based on the simple Lane detection pipeline with computer vision technique.For more info check  [GitHub Link](https://github.com/rahul-0906/Lane-Detector-openCV.git) </span>

## Lane Detection Pipeline:
1. Convert original image to Grayscale.
![](Gray_solidWhiteRight.jpg)
2. Darkened the gray scale image.
3. Convert original image to HLS colour space.
4. Isolate yellow from HLS to get yellow mask (for yellow lane marking).
5. Isolate yellow from HLS to get white mask (for white lane marking).
6. Bit-wise OR yellow and white masks to get common mask.
7. Bit-wise AND mask with Darkened image.
8. Apply slight Gaussian Blur.
9. Apply canny Edge Detector 
10. Define Region of Interest. This helps in weeding out unwanted edges detected by canny edge detector.
11. Retrieve Hough lines.
12. Consolidate and extrapolate the Hough Lines and Draw them on original image
