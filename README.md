# Head-Pose-Estimation

## Demo:
https://user-images.githubusercontent.com/55801427/220363834-e87030b2-fbfc-4d70-84e3-0427f7be354d.mp4



## Dataset:  
For this project, the dataset used is <a href=http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/Database/AFLW2000-3D.zip>AFLW2000 Dataset</a>, which consists of 2000 face images, with some information about them like the facial landmarks and the pitch, yaw, and roll values for each picture.

## Solution:
1. Used the MediaPipe library to extract the face landmarks x,y.
2. Performed preprocessing step to make the model independent of the face position or scale using nomralize data based on position noise.
3. Trained a regression model using the position of the most important facial landmarks to estimate the values of the pitch, yaw, and roll.
4. Used rotation, translation, and projection of the axes on the image to visualize the direction the person is looking at.
5. Used the values of pitch, yaw, and roll to define the direction.  


## Libraries used:
1. MediaPipe
2. Numpy
3. OpenCV
4. Matplotlib
5. Pandas
6. Scikit-Learn
