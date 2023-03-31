# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
import opencv

### Step2:
Read the original Image.

### Step3:
Store the required conversion of the image in a variable.

### Step4:
Show the image stored in the given variable.

### Step5:
Destroy all the windows and end the program.

## Program:
```python
# Developed By:K.Jhansi

# Register Number:212221230045

#i) Convert RGB to HSV, GRAY,YCrCb,BGR

#RGB to HSV

import cv2

rselephant_color_image= cv2.imread('rselephant.jpg')

cv2.imshow ('Original image', rselephant_color_image)

hsv_image = cv2.cvtColor (rselephant_color_image, cv2.COLOR_RGB2HSV)

cv2.imshow('RGB2HSV', hsv_image)

cv2.waitKey(0)

cv2.destroyAllWindows()

#RGB to Gray

 import cv2
 
 rselephant_color_image= cv2.imread('rselephant.jpg')
 
 cv2.imshow ('Original image', rselephant_color_image)
 
 gray_image=cv2.cvtColor(rselephant_color_image, cv2.COLOR_RGB2GRAY)
 
 cv2.imshow('RGB2GRAY', gray_image)
 
 cv2.waitKey(0)
 
 cv2.destroyAllWindows()
 
 #RGB to YCrCb
 
 import cv2
 
rselephant_color_image = cv2.imread('rselephant.jpg')

cv2.imshow('Original Image',rselephant_color_image)

YCrCb_image = cv2.cvtColor(rselephant_color_image, cv2.COLOR_RGB2YCrCb)

cv2.imshow('RGB2YCrCb',YCrCb_image)  

cv2.waitKey(0)

cv2.destroyAllWindows()

#RGB to BGR

import cv2

rselephant_color_image= cv2.imread('rselephant.jpg')

cv2.imshow ('Original image', rselephant_color_image)

bgr_image = cv2.cvtColor (rselephant_color_image, cv2.COLOR_RGB2BGR)

cv2.imshow('RGB2BGR', bgr_image)

cv2.waitKey(0)

cv2.destroyAllWindows() 

#ii)Convert HSV to RGB and BGR

#HSV to RGB

import cv2

rselephant_hsv_image=cv2.imread('dip_hsv.png')

cv2.imshow('HSV_image',rselephant_hsv_image)

RGB_image=cv2.cvtColor(rselephant_hsv_image,cv2.COLOR_HSV2RGB)

cv2.imshow('HSV2RGB',RGB_image)

cv2.waitKey(0)

cv2.destroyAllWindows()

#HSV to BGR

import cv2

rselephant_hsv_image=cv2.imread('dip_hsv.png')

cv2.imshow('HSV_image',rselephant_hsv_image)

BGR_image = cv2.cvtColor(rselephant_hsv_image, cv2.COLOR_HSV2BGR)

cv2.imshow('HSV to BGR',BGR_image)

cv2.waitKey(0)

cv2.destroyAllWindows()

#iii)Convert BGR to YCrCb, HSV, GRAY:


#BGR to HSV

import cv2

rselephant_bgr_image= cv2.imread('Downloads/bgr_image.png')

cv2.imshow ('bgr_image', rselephant_bgr_image)

hsv_image = cv2.cvtColor (rselephant_bgr_image, cv2.COLOR_BGR2HSV)

cv2.imshow('BGR2HSV', hsv_image)

cv2.waitKey(0)

cv2.destroyAllWindows()

#BGR to gray

import cv2

rselephant_bgr_image= cv2.imread('Downloads/bgr_image.png')

cv2.imshow ('bgr_image', rselephant_bgr_image)

gray_image= cv2.cvtColor (rselephant_bgr_image, cv2.COLOR_BGR2GRAY)

cv2.imshow('BGR2GRAY', gray_image)

cv2.waitKey(0)

cv2.destroyAllWindows()

#BGR to YCrCb

import cv2

rselephant_bgr_image = cv2.imread('Downloads/bgr_image.png')

cv2.imshow('bgr_image', rselephant_bgr_image)

YCrCb_image = cv2.cvtColor(rselephant_bgr_image, cv2.COLOR_BGR2YCrCb)

cv2.imshow('BGR2YCrCb',YCrCb_image)  

cv2.waitKey(0)

cv2.destroyAllWindows()

# iv)Split and Merge RGB Image

import cv2

img = cv2.imread("dip_bgr.png")

img1= cv2.resize(img, (270,190))

cv2

B,G,R = cv2.split(img1)

cv2.imshow("RED MODEL", R)

cv2.imshow("GREEN MODEL", G)

cv2.imshow("BLUE MODEL ", B)

merger = cv2.merge([B,G,R])

cv2.imshow("MERGED IMAGE", merger )

cv2.waitKey(0)

cv2.destroyAllWindows()

# v) Split and merge HSV Image

import cv2

img = cv2.imread("dip_hsv.png")

img1= cv2.resize(img, (270,190))

HSV = cv2.cvtColor(img1 , cv2.COLOR_BGR2HSV)

cv2.imshow("Initial_HSV ", HSV)

H,S,V = cv2.split(HSV)

cv2.imshow("RED MODEL", H)

cv2.imshow("GREEN MODEL",S)

cv2.imshow("BLUE MODEL ", V)

merger = cv2.merge([H,S,V])

cv2.imshow("MERGED IMAGE", merger )

cv2.waitKey(0)

cv2.destroyAllWindows()

```
## Output:
### i) BGR and RGB to HSV and GRAY

#RGB to HSV:

![output](https://github.com/jhansi21005096/Color-Conversion/blob/main/dipout-1.png)

#RGB to GRAY:

![output](https://github.com/jhansi21005096/Color-Conversion/blob/main/dipout-2.png)

#RGB to YCrCb:

![output](https://github.com/jhansi21005096/Color-Conversion/blob/main/dipout-3.png)

#RGB to BGR:


### ii) HSV to RGB and BGR
#HSV to RGB:

#HSV to BGR:

### iii) RGB and BGR to YCrCb
#BGR TO HSV:

#BGR TO GRAY:

#BGR TO YCrCb:

### iv) Split and merge RGB Image


### v) Split and merge HSV Image



## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
