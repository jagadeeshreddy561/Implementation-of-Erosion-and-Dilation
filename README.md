# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.

### Step2:
Create the text image using cv2.putText.

### Step3:
Then create the structuring image for dilation/erosion.

### Step4:
Apply erosion and dilation using cv2.erode and cv2.dilate.

### Step5:
Plot the images using plt.imshow.

 
## Program:
```
Developed by : Jagadeeshreddy561
Registeration Number:212222240059
```

``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
text_image = np.zeros((100,440),dtype = 'uint8')
font = cv2.FONT_HERSHEY_COMPLEX_SMALL
cv2.putText(text_image," JAGADEESH",(5,70),font,2,(255),5,cv2.LINE_AA)
plt.title("Original Image")
plt.imshow(text_image,'magma')
plt.axis('off')

# Create the structuring element
import cv2
import numpy as np
import matplotlib.pyplot as plt
text_image = np.zeros((100,440),dtype = 'uint8')
font = cv2.FONT_HERSHEY_COMPLEX_SMALL
cv2.putText(text_image," JAGADEESH",(5,70),font,2,(255),5,cv2.LINE_AA)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
image_erode = cv2.erode(text_image,kernel)
plt.title("Eroded Image")
plt.imshow(image_erode,'magma')
plt.axis('off')

# Dilate the image
import cv2
import numpy as np
import matplotlib.pyplot as plt
text_image = np.zeros((100,440),dtype = 'uint8')
font = cv2.FONT_HERSHEY_COMPLEX_SMALL
cv2.putText(text_image," JAGADEESH",(5,70),font,2,(255),5,cv2.LINE_AA)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_dilate = cv2.dilate(text_image,kernel)
plt.title("Dilated Image")
plt.imshow(image_dilate,'magma')
plt.axis('off')



```
## Output:

### Display the input Image

![download](https://github.com/jagadeeshreddy561/Implementation-of-Erosion-and-Dilation/assets/120623104/99b5ee79-c30d-4a74-b577-23547fb1922b)


### Display the Eroded Image
![download](https://github.com/jagadeeshreddy561/Implementation-of-Erosion-and-Dilation/assets/120623104/56c14307-a3f1-4419-89db-817cba8cc5a8)



### Display the Dilated Image
![download](https://github.com/jagadeeshreddy561/Implementation-of-Erosion-and-Dilation/assets/120623104/16d09431-fc24-45dd-a07e-f58e3517b4e3)



## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
