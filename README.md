# Real-Time-Object-Detection-With-OpenCV

### Introduction

This project aims to do real-time object detection through a laptop camera or webcam using OpenCV and MobileNetSSD. The idea is to loop over each frame of the video stream, detect objects like person, chair, dog, etc. and bound each detection in a box.
Here, we will go through the steps required for setting up the project and some explanation about the code.

### Project description
To detect the object, we have initialized the list of the 21 class labels MobileNet SSD was trained to. Each prediction composes of a boundary box and 21 scores for each class. Then Assigned random colors(a list of 21 R,G,B values) to each of the classes. When we pass any object from these declared class labels, it detects the object and gives a tag to that object with its corresponding class label. If any undeclared object is passed and is having any similarities with some y object which is present in declared classes then it tags the current undeclared object as ‘y’.
To count the objects, we have created a dictionary which stores all the objects. After the object detected, we updated the objects dictionary with the key as the label and the value as count. If the label is already present in the dictionary, incremented the count. Else, added the label to the dictionary and set the count to 1.
After detecting and counting the objects, displayed FPS Information consists of total Elapsed time and an approximate FPS over the entire video stream.

### Applications
1. Activity Recognition
2. Road condition monitoring  
3. Traffic flow monitoring
4. Crowdedness estimation
5. Product counting in manufacturing industries.

### Conclusion
The goal of Object Counting task is to count the number of object instances in a single image or video sequence. The accuracy of the algorithm depends upon different factors like the camera used, the size of objects, clarity of the image and other illumination conditions.  Object detection is often combined with other computer vision techniques like tracking and counting to develop more robust applications that better solve real-life scenarios.


## Team Members
1. Shaik Zaveriya (Team Leader)
2. Kolluri Chamundeswari
3. Koppala Meghana
4. Lakshmi Narayana Reddy
5. Ragha Likitha
6. Mulla Kousar Banu
7. Boosa Neeraja
