# Computer Vision - Traditional method
Application 1 - Converting handwrittern or hand drawn text into E-text.
Libraries - cv2, numpy, matplotlib
Language - Python
Topics - Thresholding, BGR (RGB) channel and alpha channel
Pipeline - 
  Read the image.
  Pre-processing :-
    crop the image as per requirement.
    Convert the image into gray scale - as to form the threshold mask of the image, the image must be in the gray scale (blacka and white channel).
  Pass the pre-processed image into the thresholding function by setting the threshold value (as per the image) and set the threshold type as THRESH_BINARY_INV (the valid parts will be masked into white color / 255).
  As a result it returns into setted threshold value and the threshold mask
  Post-processing :-
    Split the origional cropped image's channel into B, G, R.
    Form a new variable that contains the values of image's B,G,R and threshold mask (as an alpha channel) 
  Merge the new variable as a new image that has upscaled from 3 channels into 4 channels - B G R Alpha.
  Save the image - the image that trasforms the handwrittern text into digital or scanned text.
