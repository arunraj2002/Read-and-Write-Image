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
### Developed By: R ARUNRAJ
### Register Number: 212220230004
i) #To Read,display the image
```
  import cv2
  import random
  color=cv2.imread("dip.jpg")
  cv2.imshow("img",color)
  cv2.waitKey(0)
```
ii) #To write the image
```
   cv2.imwrite("tower.jpg",color)
```
iii) #Find the shape of the Image
```
   print(color.shape)
```
iv) #To access rows and columns
```
   for i in range(70,90):
    for j in range(110,170):
        color[i][j]=[0,0,0]
   cv2.imshow("tower.jpg",color)
   cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
   tow=cv2.imread("dip.jpg")
   tow[150:250,150:250]=tow[300:400,300:400]
   cv2.imshow("tower.jpg",tow)
   cv2.waitKey(0)
```

## Output:

### i) Read and display the image
<img src="https://user-images.githubusercontent.com/75235747/161131460-44aaf9dc-2874-4fee-9687-eb32c8688a2b.png" width="600">
|<br>

### ii)Write the image
<img src="https://user-images.githubusercontent.com/75235747/161131636-242026bc-96d5-4a41-953e-7816665b7319.png" width="600">
<br>

### iii)Shape of the Image
<img src="https://user-images.githubusercontent.com/75235747/161131726-84c81fcd-6873-495e-9ed4-c050cbec658f.png" width="600">
<br>

### iv)Access rows and columns
<img src="https://user-images.githubusercontent.com/75235747/161131826-8c243a9e-e779-4c1b-9320-ccafc7b4cf0c.png" width="600">
<br>

### v)Cut and paste portion of image
<img src="https://user-images.githubusercontent.com/75235747/161131925-91d1c3c7-2ea6-447e-a938-2d6f3be23be8.png" width="600">
<img src="https://user-images.githubusercontent.com/75235747/161131950-26281bde-5f06-4bdf-9df2-2f2355d5c18d.png" width="600">
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


