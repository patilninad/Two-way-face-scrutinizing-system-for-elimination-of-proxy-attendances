# Introduction:-  
Actual project was Face recognition based automatic attendance system. But later we developed a proxy eliminating algorithm and renamed the project. We also submitted our algorithm in Springer Conference for publication in Springer Conference editorials.  
Recording and maintaining an individual's attendance is a time-consuming task
in various educational and corporate institution. Most of them implement roll-call based attendance marking system/passing attendance sheet. In these methods there are chances of marking proxy attendances Maintainance of recorded attendance is another major deed
which may cause manual errors. 
There are many biometric methods available and adopted recently like, Fingerprint/eyeball detection based. Both these methods are time consuming resulting into queues.  
Although there are less chances of marking proxy attendances in both of these methods but they are complex and time-consuming. Hence we have used face detection and recognition system along with novel proxy eliminating algorithm.  
# Algorithm for eliminating proxy attendances:-  
![](https://github.com/patilninad/Two-way-face-scrutinizing-system-for-elimination-of-proxy-attendances/blob/master/Algorithm.PNG)  
_____________________________________________________________________________________________  

![](https://github.com/patilninad/Two-way-face-scrutinizing-system-for-elimination-of-proxy-attendances/blob/master/Algorithm%202.PNG)  
•	The LDR sensor attached to the camera will detect whether the lighting condition is enough. In case the light is insufficient then flashlight will be turned on.  
•	For this case duration of the lecture is assumed to be 50 minutes.  
•	A database consisting of encoded images of enrolled persons is created and stored in the internal memory of raspberry pi.  
•	The camera will start capturing images, the image captured will be encoded and compared with a database of encoded images.  
•	If the two encoded image matches green light will blink indicating the persons face is properly detected.   
•	If the image is not properly captured or if the image is not properly recognized, then red light blinks.  
•	The camera will start capturing and recognizing face images at the beginning of the lecture and will continue until 15 minutes after the expected starting time of the lecture. It records the in time of that person. After 15 minutes the camera will stop capturing images and will turn inwards.  
•	The camera will again start capturing images after the lecture ends(after 50 minutes) and will continue up to 5 minutes, when the person leaves the class the camera captures the image and encodes it, it records the in time and out time of person and marks the attendance of the person in accordance with the time for which he attended the lecture.  
•	After 5 minutes the camera is rotated outwards and is ready to record attendance for next lecture.  
•	After 5 minutes the camera is rotated outwards and is ready to record attendance for next lecture.  
•	At the end of the day, the updated excel file is uploaded to the Dropbox cloud  whose access is provided to respective faculty members.  
•	This system can be programmed according to the lecture timings which varies in different institutions.  
# Prototype of the proposed system:-  
![](https://github.com/patilninad/Two-way-face-scrutinizing-system-for-elimination-of-proxy-attendances/blob/master/Prototype.jpeg)

