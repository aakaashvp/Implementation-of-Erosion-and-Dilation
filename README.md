## Ex no: 10
## Date: 25/5/2022
# <p align="center">Implementation of Erosion and Dilation

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages.


### Step2:
<br>Create the Text using cv2.putText.

### Step3:
<br>Create the structuring element.

### Step4:
<br>Erode and Dilate the image.

### Step5:
<br>End Program.

 
## Program:
```
DEVELOPED BY : AAKAASH VP
REG NO :2122202300001
```

``` Python
# Import the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt



# Create the Text using cv2.putText
img1 = np.zeros((100,270), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'aakaash',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')


# Create the structuring element
cv2.erode(img1, kernel)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))




# Erode the image

image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')



# Dilate the image

image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')



```
## Output:

### Display the input Image
<br>![image](https://user-images.githubusercontent.com/75235212/169644609-5eed6043-59a8-46fb-a7f0-7b6bb224d68f.png)

<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
<br>![image](https://user-images.githubusercontent.com/75235212/169644695-e021b3da-7d13-46d3-b183-56cc82626a80.png)

<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image
<br>![image](https://user-images.githubusercontent.com/75235212/169644709-1b2f2bda-ae28-4631-8d68-f41e702249a8.png)

<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
