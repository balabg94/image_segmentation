# image_segmentation

A simple image segmentation using PIL (pillow). 
Here Captchas are segemented. The size of the segmentation is hardcoded in the script.

The Captcha_seg.ipynb is the jupyter notebook file which contains the script.
The python file will be updated soon.

The files named, 0.png, 1.png, 2.png, 3.png, 4.png, are the segmented files in the order. 
The files are the cropped version of the captcha.

As of now the image location is hard coded in the script. The Captcha is converted to monochrome using Otsu thresholding.
Then Dilated and Eroded using Closing mophological transformation in the Opencv. On dilation again, the characters are of appropriate size. 

Since we are using the same kind of Captchas, the character locations in the images are approximately the same. Thus the segmentation rectangles are hardcoded for testing. 

Using PIL (pillow), the segmented portions are cropped out and saved as '.png' files.
