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
### Developed By:Archana priya.J
### Register Number:212221230007 
i) #To Read,display the image
```
import cv2
colorim = cv2.imread('sce.jpg',1)
cv2.imshow('Scenery',colorim)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
colorim = cv2.imread('sce.jpg',1)
cv2.imwrite('written.jpg',colorim)
cv2.imshow('Scenery',colorim)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import cv2
colorim = cv2.imread('sce.jpg',1)
print(colorim.shape)
cv2.waitKey(0)
```
iv) #To access rows and columns

```

import cv2
colorim = cv2.imread('sce.jpg',1)
import random
for i in range (100):
    for j in range(colorim.shape[1]):
        colorim[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('partofimage',colorim)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
v) #To cut and paste portion of image
```python3

import cv2
colorim = cv2.imread('sce.jpg',1)
tag = colorim[300:400,300:400]
colorim[50:150,50:150] = tag
cv2.imshow('portioned',colorim)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

<br>
![Screenshot (345)](https://user-images.githubusercontent.com/93427594/225084276-4ead96a9-2379-4714-ab30-a5b4c04125d1.png)

<br>

### ii)Write the image


![Screenshot (346)](https://user-images.githubusercontent.com/93427594/225085161-0f88d929-3427-48b0-89bc-b5522c206513.png)
![Screenshot (345)](https://user-images.githubusercontent.com/93427594/225084276-4ead96a9-2379-4714-ab30-a5b4c04125d1.png)




### iii)Shape of the Image

<br>
![sceshape](https://user-images.githubusercontent.com/93427594/225085293-13e7bcdc-0b57-428a-bf10-ddc79b946caf.png)

<br>

### iv)Access rows and columns
<br>
![Screenshot (350)](https://user-images.githubusercontent.com/93427594/225084710-6eaa41e5-bf98-468f-be3a-760557454f06.png)

<br>

### v)Cut and paste portion of image
<br>
![Github)](https://user-images.githubusercontent.com/93427594/225084436-15adbc83-b945-4cad-8136-581375888b3c.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


