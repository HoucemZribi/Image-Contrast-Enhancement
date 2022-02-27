# Image-Contrast-Enhancement
This application permet you to enhance an image contrast.
# Install  
    git clone https://github.com/HoucemZribi/Image-Contrast-Enhancement.git
# Library to install 
    pip install cv2 matplotlib numpy IPython glob2
# Steps 
  1- Convert input image from RGB to CIELAB, progress on L channel​

  2- Calculate the average pixel intensity - M value​

  3- Fuzzification: For each pixel, calculate degree of membership of each class based on pixel intensity and M value. Intensity∈[0,255]​

  4- Inference: Calculate the output fuzzy set from the input pixel intensity based on the proposed rule set​

  5- Defuzzification: For each pixel, calculate centroid value of its output fuzzy set. Centroid∈[−50,305]​

  6- Normalize output pixel intensity from [-50, 305] to [0, 255]​

  7- Merge modified L channel to the original AB channels, convert output image from CIELAB to RGB​
