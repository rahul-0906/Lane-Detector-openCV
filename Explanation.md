# Lane Detector 

### Project Description:
   This Project is based on the Opencv python module.Identifying the lanes in the roads is common task.This is critical task for automonous vehicle to perform.Here This project based on the simple Lane detection pipeline with computer vision technique.For more info check  [GitHub Link](https://github.com/rahul-0906/Lane-Detector-openCV.git) </span>

## Lane Detection Pipeline:
### Convert original image to Grayscale.
![Grayscale](/image_output/Gray_solidWhiteRight.jpg)
### Darkened the gray scale image.
### Convert original image to HLS colour space.
### Isolate yellow from HLS to get yellow mask (for yellow lane marking).
### Isolate yellow from HLS to get white mask (for white lane marking).
### Bit-wise OR yellow and white masks to get common mask.
### Bit-wise AND mask with Darkened image.
![Maskimage](/images_output/Color_Mask_solidWhiteCurve.jpg)
### Apply slight Gaussian Blur.
![Gaussianimage](/images_output/Gaussian_solidWhiteRight.jpg)
### Apply canny Edge Detector 
![Cannyimage](/images_output/Canny_solidWhiteRight.jpg)
### Define Region of Interest. This helps in weeding out unwanted edges detected by canny edge detector.
### Retrieve Hough lines.
### Consolidate and extrapolate the Hough Lines and Draw them on original image
![explotingimage](/images_output/Extrapolation_solidWhiteCurve.jpg)
