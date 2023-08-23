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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
  

```
ii) #To write the image
```
import cv2
color_image=cv2.imread('Moon.jpg',1)
img=cv2.imwrite('xyz1.png',color_image)
cv2.imshow('212222230052 Moon',color_image)
cv2.waitKey(0) 


```
iii) #Find the shape of the Image
```python3
import cv2
image_path = 'Moon.jpg'
image = cv2.imread(image_path)
cv2.imshow('212222230052 Moon',image)
cv2.waitKey(0) 


```
iv) #To access rows and columns

```python3
import cv2
import random
color_img=cv2.imread('Moon.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230052 JAYAKRISHNAN',color_img)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3
import cv2
color_image=cv2.imread('Moon.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222230052 Moon',color_image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

![Screenshot from 2023-08-22 00-00-15](https://github.com/Jayakrishnan22003251/READ-AND-WRITE-IMAGE/assets/120232371/e30a19ac-819b-4718-aafd-69d3a44f6b57)


### ii)Write the image

![Screenshot from 2023-08-22 00-00-15](https://github.com/Jayakrishnan22003251/READ-AND-WRITE-IMAGE/assets/120232371/bc09b4af-2ba4-4d95-bc11-861e6573c75a)


### iii)Shape of the Image

![Screenshot from 2023-08-23 12-46-09](https://github.com/Jayakrishnan22003251/READ-AND-WRITE-IMAGE/assets/120232371/170ce995-7651-4440-9798-e83db82d05dc)


### iv)Access rows and columns
![Screenshot from 2023-08-23 12-43-08](https://github.com/Jayakrishnan22003251/READ-AND-WRITE-IMAGE/assets/120232371/2f5b59f7-3a88-4315-81a8-460d8dcb7997)


### v)Cut and paste portion of image

![Screenshot from 2023-08-22 19-45-39](https://github.com/Jayakrishnan22003251/READ-AND-WRITE-IMAGE/assets/120232371/859cee01-790a-4c0f-a2ca-86435522ea78)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
