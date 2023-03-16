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
### Developed By: Haridharshini.S
### Register Number: 212221230033
i) #To Read,display the image
```
import cv2
A=cv2.imread("sa.jpg",1)
cv2.imshow("Haridharshini.S",A)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
A=cv2.imread("sa.jpg",1)
cv2.imshow("Haridharshini.S",A)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```
import cv2
color_image = cv2.imread('sa.jpg',1)
print(color_image.shape)

```
iv) #To access rows and columns

```
import random
import cv2
color_image = cv2.imread('sa.jpg',1)
for i in range(150):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('sun2.jpg',color_image)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```
import cv2
color_image = cv2.imread('sa.jpg',1)
part = color_image[300:400,300:400]
color_image[50:150,50:150] = part
cv2.imshow("hari",color_image)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

![exp1a ](https://user-images.githubusercontent.com/94168395/225528868-fe6e3c86-a313-4afc-bdda-f5f239169b83.png)

### ii)Write the image

![exp1a ](https://user-images.githubusercontent.com/94168395/225528868-fe6e3c86-a313-4afc-bdda-f5f239169b83.png)

### iii)Shape of the Image

![exp1b](https://user-images.githubusercontent.com/94168395/225528996-27d55f87-8281-4f12-bb6b-a7a5ad0b3090.png)


### iv)Access rows and columns

![exp1c](https://user-images.githubusercontent.com/94168395/225529049-e135a617-c89e-4883-8d82-8cdc0d97b1c5.png)


### v)Cut and paste portion of image

![exp1d](https://user-images.githubusercontent.com/94168395/225529135-d58af17a-edd9-4bd9-8c65-e816de2bf342.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


