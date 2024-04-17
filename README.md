# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2:
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation


 
## Program:
```
DEVELOPED BY: P RAMSAi
REG NO:212221240041
```
### Import the necessary packages
```
import cv2
import numpy as np
```
### Create the Text using cv2.putText
```
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'SAVEETHA', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)

```
### Create the structuring element
```
struct_ele = np.ones((9, 9), np.uint8)

```
### Use Opening operation
```
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)

 ```

###  Use Closing Operation
```
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)



```
## Output:

### Display the input Image
![image](https://github.com/Ramsai1234/OPENING--AND-CLOSING/assets/94269989/7c258d7b-7ba0-4db3-a499-09015146a82c)



### Display the result of Opening
![image](https://github.com/Ramsai1234/OPENING--AND-CLOSING/assets/94269989/dd3402fb-766a-4f59-95c3-eaea1ad19bf3)



### Display the result of Closing
![image](https://github.com/Ramsai1234/OPENING--AND-CLOSING/assets/94269989/cbddb57d-6f30-4b12-83e1-db39a85a10ba)



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
