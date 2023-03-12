## READ AND WRITE AN IMAGE
## Aim:
To write a python program using OpenCV to do the following image manipulations.
```
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.
```
## Software Required:
Anaconda - Python 3.7
## Algorithm:
## Step1:
Choose an image and save it as a filename.jpg
## Step2:
Use imread(filename, flags) to read the file.
## Step3:
Use imshow(window_name, image) to display the image.
## Step4:
Use imwrite(filename, image) to write the image.
## Step5:
End the program and close the output image windows.
## Program:
## Developed By:B.PAVIZHI
## Register Number: 212221230077
## i) To Read,display the image
```
import cv2 as cv
capture=cv.imread('photos/photo.jpg')
cv.imshow('PHOTO',capture)
cv.waitKey(0)
```
## ii) To write the image
```
import cv2 as cv
capture=cv.imread("photos/photo.jpg")
cv.imwrite("photo.jpg",capture)
cv.imshow("212221230077",capture)
cv.waitKey(0)
```
## iii) Find the shape of the Image
```
import random
import cv2 as cv
capture=cv.imread("photos/photo.jpg")
for i in range(100):
    for j in range(capture.shape[1]):
        capture[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv.imshow("212221230077",capture)
cv.waitKey(0)
```
## iv) To access rows and columns

```
import random
import cv2 as cv
capture=cv.imread("photos/photo.jpg")
for i in range(100):
    for j in range(capture.shape[1]):
        capture[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv.imshow("212221230077",capture)
cv.waitKey(0)
```
## v) To cut and paste portion of image
```
import cv2
capture=cv2.imread("photo.jpg",1)
tag=capture[140:240,165:180]
capture[25:125,50:65]=tag
cv2.imshow("212221230077",capture)
cv2.waitKey(0)
```

## Output:

## i) Read and display the image
![](./read.png)

## ii)Write the image
![](./write.png)


## iii)Shape of the Image

![](./shape.png)
## iv)Access rows and columns
![](./rows.png)
## v)Cut and paste portion of image

![](./cut%20and%20pas.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


