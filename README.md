# COLOR_CONVERSIONS_OF-IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.

i) Read, display, and write an image.

ii) Access the rows and columns in an image.

iii) Cut and paste a small portion of the image.

iv)To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg ,
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
### Step6:
Convert BGR and RGB to HSV and GRAY
### Step7:
Convert HSV to RGB and BGR
### Step8:
Convert RGB and BGR to YCrCb
### Step9:
Split and Merge RGB Image
### Step10:
Split and merge HSV Image

##### Program:
### Developed By:pragaharshitha N.C
### Register Number: 212222110033


## Output:

### i) Read and display the image
```
import cv2
import matplotlib.pyplot as plt

img=cv2.imread("pvr.jpg",1)
cv2.imshow("display window",img)
cv2.waitKey(0)
cv2.destroyAllWindows()
print(img.shape)
```
OUTPUT:
![Screenshot (17)](https://github.com/pragachellapillai/COLOR_CONVERSIONS_OF-IMAGE/assets/148254952/fcfd98d7-c548-4d7b-8eea-29e5be2dcbbe)


### ii)Write the image
```
img1=cv2.imread("pvr.jpg",0)
cv2.imshow("display window",img1)
cv2.waitKey(0)
cv2.destroyAllWindows()
cv2.imwrite('greyscale.jpeg',img1)
```

OUTPUT:
![Screenshot (18)](https://github.com/pragachellapillai/COLOR_CONVERSIONS_OF-IMAGE/assets/148254952/a308cc14-16b0-426b-9ae2-11223f6bf4c9)


### iii)Shape of the Image
```
import cv2
img1=cv2.imread("pvr.jpg",1)
print(img1.shape)
```
OUTPUT:
![Screenshot (19)](https://github.com/pragachellapillai/COLOR_CONVERSIONS_OF-IMAGE/assets/148254952/8850a738-5da7-4a67-928c-73af03fab41d)


### iv)Access rows and columns
```
import random
import cv2
image=cv2.imread('pvr.jpg',1)
image=cv2.resize(image,(400,400))
for i in range (150,200):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255), random.randint(0,255), random.randint(0,255)] 
cv2.imshow('part image',image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
OUTPUT:



### v)Cut and paste portion of image
<br>
<br>

### vi) BGR and RGB to HSV and GRAY
<br>
<br>

### vii) HSV to RGB and BGR
<br>
<br>

### viii) RGB and BGR to YCrCb
<br>
<br>

### ix) Split and merge RGB Image
<br>
<br>

### x) Split and merge HSV Image
<br>
<br>




## Result:
Thus the images are read, displayed, and written ,and color conversion was performed between RGB, HSV and YCbCr color models successfully using the python program.







