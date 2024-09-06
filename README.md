# COLOR_CONVERSIONS_OF-IMAGE
## AIM
Write a Python program using OpenCV that performs the following tasks:

i) Read and Display an Image.

ii) 	Draw Shapes and Add Text.

iii) Image Color Conversion.

iv) Access and Manipulate Image Pixels.

v) Image Resizing

vi) Image Cropping

vii) Image Flipping

viii)	Write and Save the Modified Image


## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Load an image from your local directory and display it.
### Step2:
o	Draw a line from the top-left to the bottom-right of the image.
o	Draw a circle at the center of the image.
o	Draw a rectangle around a specific region of interest in the image.
o	Add the text "OpenCV Drawing" at the top-left corner of the image.

### Step3:
o	Convert the image from RGB to HSV and display it.
o	Convert the image from RGB to GRAY and display it.
o	Convert the image from RGB to YCrCb and display it.
o	Convert the HSV image back to RGB and display it.

### Step4:
o	Access and print the value of the pixel at coordinates (100, 100).
o	Modify the color of the pixel at (200, 200) to white.

### Step5:
o	Resize the original image to half its size and display it.
### Step6:
o	Crop a region of interest (ROI) from the image (e.g., a 100x100 pixel area starting at (50, 50)) and display it.
### Step7:
o	Flip the original image horizontally and display it.
o	Flip the original image vertically and display it.

### Step8:
o	Save the final modified image to your local directory.


##### Program:
### Developed By: Sriram G
### Register Number: 212222230149


## Output:

### i)Read and Display an Image

```
import cv2
# Read the image
image = cv2.imread('Lokesh.JPG')
# Display the image in a window
cv2.imshow('Image Window', image)
# Wait indefinitely for a key press
cv2.waitKey(0)
# Destroy all windows created by OpenCV
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/f21cc1d1-82f1-48c5-a35b-e4adbe02580d)
<br>
<br>

### ii)Draw Shapes and Add Text

```
import cv2

img = cv2.imread("Lokesh.JPG")
start=(0,0)
stop=(500,329)
color=(100,255,100)
thickness=10
res_img=cv2.circle(img,(330,225),150,(255,0,0),10)
res_img=cv2.rectangle(img,start,stop,color,thickness)
text = "OpenCV Drawing"
org = (10, 30)  # top-left corner of the text string
font = cv2.FONT_HERSHEY_SIMPLEX
font_scale = 1
text_color = (255, 255, 255)  # White color
thickness = 2
res_img = cv2.line(img,(100,200),(900,100),(200,100,205),10)
res_img= cv2.putText(res_img, text, org, font, font_scale, text_color, thickness, cv2.LINE_AA)

# Display the HSV image
cv2.imshow('Image Window', res_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/39ee7efc-fdd6-49a3-8284-716f847e4ec1)

<br>
<br>

### iii)Image Color Conversion

```
# Read the image
image = cv2.imread("Lokesh.JPG")

# Convert to HSV color space
img_hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)

# Display the HSV image
cv2.imshow('Image Window (HSV)', img_hsv)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
![image](https://github.com/user-attachments/assets/c6b5d1d6-a215-489f-b52a-71d66129309f)
<br>
<br>

### iv)Access and Manipulate Image Pixels
<br>
<br>

### v)Image Resizing
<br>
<br>

### vi)Image Cropping
<br>
<br>

### vii)Image Flipping
<br>
<br>

### viii)Write and Save the Modified Image
<br>
<br>






## Result:
Thus the images are read, displayed, and written ,and color conversion was performed  successfully using the python program.







