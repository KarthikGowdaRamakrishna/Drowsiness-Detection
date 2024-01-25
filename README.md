# RealTime_Drowsiness_Detection_Yolov5
A Yolov5s model is trained from scratch on annotated images to make real-time detections if a person is awake or drowsy.

Steps:

1. Install pytorch and dependencies as per mentioned on their <a href="https://pytorch.org/get-started/locally/">website.</a>
2. Since <a href="https://github.com/ultralytics/yolov5">yolov5</a> is already a pretrained model, we load it into our enviroment and run it on a generic image to check how it makes it's detections. 

![output](https://user-images.githubusercontent.com/97375173/187121160-d42d4da8-51c7-442f-bef7-ca4545fe7925.png)
# using 'opencv' lib to make realtime detection using computers webcam 
![image](https://github.com/KarthikGowdaRamakrishna/Drowsiness-Detection/assets/144963620/f7f2ab5e-ed44-415b-b221-b6e06d5a7b52)
![image](https://github.com/KarthikGowdaRamakrishna/Drowsiness-Detection/assets/144963620/7931deb3-63ef-4402-8bf9-ddfdbd3ff332)


3. We also generate a real-time feed from our webcam using OpenCV and make detections using the loaded model.
4. With the help of a loop and OpenCV we generate 20 images each for both our categories - Drowsy and Awake. 
5. We now use <a href="https://github.com/heartexlabs/labelImg">LabelImg</a>, an open source pythonand QT based graphic annotation tool that helps us draw a box around the subject in each image or 'tag' the image.

![Zidane](https://raw.githubusercontent.com/tzutalin/labelImg/master/demo/demo3.jpg)
![image](https://github.com/KarthikGowdaRamakrishna/Drowsiness-Detection/assets/144963620/431ec725-af0b-46fa-9e78-67cf99bac3e9)
![image](https://github.com/KarthikGowdaRamakrishna/Drowsiness-Detection/assets/144963620/c590da74-79c7-42a0-b26d-632f53af0fe4)


6. Our train dataset is now ready to be input in the model. We then train the model on the basis of the dataset we just created. 
7. Using our trained model and OpenCV webcame feed we can now make real-time detections to see if a person is awake or sleepy.
# Results in Real-Time live feed from web cam
![image](https://github.com/KarthikGowdaRamakrishna/Drowsiness-Detection/assets/144963620/6d654edb-24c3-44c1-8b88-f84f2913b0f0)
# Please do check out the results.csv for better understanding

