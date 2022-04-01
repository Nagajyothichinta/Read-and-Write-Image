# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.


## Program:
```python
# Developed By:Ch.Nagajyothi
# Register Number:212221230015
# To Read,display the image

import cv2
color_img=cv2.imread('flowers.jpg',1)
cv2.imshow('212221230015,Ch.Nagajyothi',color_img)
cv2.waitKey(0)


# To write the image

import cv2
color_img=cv2.imread('flowers.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221230015,Ch.Nagajyothi',color_img)
cv2.waitKey(0)


# Find the shape of the Image

import cv2
import random
color_img=cv2.imread('flowers.jpg',1)
print(color_img.shape)


# To access rows and columns

import cv2
import random
color_img=cv2.imread('flowers.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230015,Ch.Nagajyothi',color_img)
cv2.waitKey(0)



# To cut and paste portion of image

import cv2
color_img=cv2.imread('flowers.jpg',-1)
tag=color_img[15:30,15:30]
color_img[15:30,15:30]=tag
cv2.imshow('212221230015,Ch.Nagajyothi',color_img)
cv2.waitKey(0)



```
## Output:

### i) Read and display the image

![output](./img1.png)


### ii)Write the image

![output](./img2.png)

### iii)Shape of the Image

![output](./img3.png)

### iv)Access rows and columns

![output](./img4.png)

### v)Cut and paste portion of image

![output](./img5.png)



## Result:
Thus the images are read, displayed, and written successfully using the python program.


