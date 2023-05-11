# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1:
Import the necessary packages.

### Step 2:
Read the image.

### Step 3:
Create the structuring element.

### Step 4:
Use Opening operation.

### Step 5:
Use Closing Operation.

### Step 6:
Display all the output images.

 
## Program:

``` Python
# Developed By   : Senthil Kumar S
# Register Number: 212221230091

# Import the necessary packages

import cv2
import matplotlib.pyplot as plt

# Opening The Image

img=cv2.imread("isagi.jpeg")
plt.imshow(img)

# Create the structuring element

kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))

# Use Opening operation

img1=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.imshow(img1)

# Use Closing Operation

img2=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.imshow(img2)

```
## Output:

### Display the input Image
![isa1](https://github.com/Senthil-Kumar-710/demo/assets/93860256/1306b21b-c859-4992-aa49-25868a38bf00)

### Display the result of Opening
![isa2](https://github.com/Senthil-Kumar-710/demo/assets/93860256/757e8b44-ce7d-4850-8fc7-0ecf73ce826d)

### Display the result of Closing
![isa3](https://github.com/Senthil-Kumar-710/demo/assets/93860256/f509be6e-aa50-44e6-bdce-bdeacbeb9aa4)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
