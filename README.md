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
```
Developed By:MUKESH V
Register Number:212222230086
```
### i)To Read,display the image
```python3
import cv2
image=cv2.imread('RE.jpg', 1)
cv2.imshow('MUKESH V (212222230086)', image)
cv2.waitKey(0)
cv2.destroyAllwindows()
```
### ii)To write the image
```python3
import cv2
image=cv2.imread("RE.jpg",1)
cv2.imwrite("RE.jpg",image)
cv2.imshow("MUKESH V (212222230086)",image)
cv2.waitKey(0)
cv2.destroyAllwindows()
```
### iii)Find the shape of the Image
```python3
import cv2
picture=cv2.imread("RE.jpg",1)
print(picture.shape)
```
### iv)To access rows and columns

```python3
import random
import cv2
image=cv2.imread("RE.jpg",1)
for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("MUKESH V (212222230086)",image)
cv2.waitKey(0)
cv2.destroyAllwindows()
```

### v)To cut and paste portion of image
```python3
import cv2
img = cv2.imread('RE.jpg', 1)
tag = img[90:150, 90:150]
img[20:80:, 20:80] = tag
cv2.imshow('MUKESH V (212222230086)', img)
cv2.waitKey(0)
```

## Output:
### i) Read and display the image
![image](https://github.com/MukeshVelmurugan/READ-AND-WRITE-IMAGE/assets/118707363/b522409f-a8c0-4265-be04-745fa1abf4f4)



### ii)Write the image
![image](https://github.com/MukeshVelmurugan/READ-AND-WRITE-IMAGE/assets/118707363/65a28cc0-039c-4af9-9478-7a4252589449)




### iii)Shape of the Image
![image](https://github.com/MukeshVelmurugan/READ-AND-WRITE-IMAGE/assets/118707363/4d186b01-bb22-4326-b09f-65808bc76de7)



### iv)Access rows and columns
![image](https://github.com/MukeshVelmurugan/READ-AND-WRITE-IMAGE/assets/118707363/86e69f8a-1416-448f-8a73-9665ed4e99df)



### v)Cut and paste portion of image
![image](https://github.com/MukeshVelmurugan/READ-AND-WRITE-IMAGE/assets/118707363/5a72b72f-42b5-4853-93d5-508175c782dd)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
