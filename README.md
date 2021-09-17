# Facial Detection API
## CKM VIGIL PVT. LTD.

:star2: **Target**

- The target of this project is to make an API would help us to improve the precision of the given model that would allow us to improve its efficency to detect distinct facial features including different characteristics like distances between 2 points, angles, positioning of different part of face.
    
    
    
---
:star2: **Started With**

- We started with a pre trained face mesh model knowed as Mediapipe which would give us 468 key points in the image,then with use of various python libraries like OpenCv,Numpy,pandas etc;we would then make certain improvements to this 
for better decection of facial features and rule out any flaws, for eg: detection of distance between two points in the iris which current model does not detect ideally.



---
:star2: **Overview and documentation**

 we have deployed the project on the streamlit (link given below) site whose homepage will look:
 
 
  ![site](https://github.com/ckmvigil/face-api-readme/blob/main/site.png)
  
##By using the *face api* we can obtain the characterstics of the face shown in the uploaded photo and video.

  
  ![exampleimg](https://github.com/ckmvigil/face-api-readme/blob/main/aaa.jpg)
  
###The uploaded image is copied into two variables for processing:- clone and keypoints
- `clone = image.copy() 
keypoints = image.copy()`
  
-`keypoints_mapping = {"right_ear": 234, 
    "left_ear": 454, 
    "right_eye": [33, 7, 163, 144, 145, 153, 154, 155, 133, 173, 157, 158, 159, 160, 161, 246], 
    "left_eye": [362, 382, 381, 380, 374, 373, 390, 249, 263, 466, 388, 387, 386, 385, 384, 398], 
    "jaw_line": [234,93,132,58,172,136,150,149,176,148,152,377,400,378,379,365,397,288,361,323, 454],
    "upper_head": [10, 8],
    "middle_head": [8, 1],
    "bottom_head": [164, 152],
    "right_ear_to_nose": [234, 5],
    "nose_to_left_ear": [5, 454],
    "right_eyebrow": 107,
    "left_eyebrow": 336, 
    "right_corner_of_mouth": 61, 
    "left_corner_of_mouth": 291,
    "upper_lip_to_lower_lip":[0,17],
    "right_eye_cord":[159,145],
    "left_eye_cord":[386,374],
    "head":[10,1],
    "vertical_line":[10,152],
    "right_ear_to_nose": [234, 5],
    "left_ear_to_nose": [5, 454],
    "mouth":[0,267,269,270,409,291,375,321,405,314,17,84,181,91,146,61,185,40,39,37],
    "jawContourLine2":[132,164,361],
    "jawContourLine3":[172,17,397],
    "vertical_line_more": [10,151,9,8,168,6,197,195,5,4,1,19,94,2,164,0,11,12,13,14,15,16,17,18,200,199,175,152]
    }`
    
- keypoint image :

  ![keypoints](https://github.com/ckmvigil/face-api-readme/blob/main/keypoints.jpeg)
  
- characteristics image:
  
  ![characteristics](https://github.com/ckmvigil/face-api-readme/blob/main/characterics.jpeg)
  
###Some functions are written to draw the shapes such as cirle for the keypoints, polygon lines and arrows for the distances measured and angle and angle slope line  for displaying the angles in the image
- distances image:
  
  ![distances](https://github.com/ckmvigil/face-api-readme/blob/main/distances.png)
  
- angles image:

  ![angles](https://github.com/ckmvigil/face-api-readme/blob/main/angles.png)
 






---
:star2: **Modules and Pakages**
    
- *Modules Used*
  1. streamlit
  1. pillow
  1. deepface
  1. pandas
  1. scikit-image
  1. opencv-python
  1. mediapipe
  
 - *Pakages Used*
    1. freeglut3-dev
    1. libgtk2.0-dev      
    

---
:star2: **Repository content**
- *Streamlit_app.py* - It contain the main code of the project which is in python language.

- *pakages.txt* - It contains the name of the pakages used in this project.

- *Requirement.txt* - It contains the names of the modules used in the code .

- *Setup.sh* - It is the scripting language command file to chain commands together in a file.




---
:star2: **Live working**
- The whole project is deployed at _Streamlit_ that turns data script to shareable web apps for python.

- To see the live working you can click [here](https://share.streamlit.io/ckmvigil/face-api/main)
---

