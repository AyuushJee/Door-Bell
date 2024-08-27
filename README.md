
# Smart Door Bell

A Smart Door alert system on raspiberry pi using raspiberry pi camera module 5mp.

The face is trained using "haarcascade_frontalface".It gave around 70% accurate result with ideal lighting condition

House door opens automatically if the person registered in database comes in front else guest have the option to press the door bell to let the owner know via call bell or telegram bot.

This smart door system have intrusion detection system and a interative telegram update features.





## Installation

_Capturing Images_

```bash
  cd smart-door/face-detection
  python 01_face_capture_dataset.py
```
👆 This will start capturing 1000 Images

_Model Training_

```bash
  cd smart-door/face-detection
  python 02_face_training.py
```
👆 Model is now trained

_To check the accuracy of current registered face_

```bash
  cd smart-door/face-detection
  python 03_face_recogition.py
```
👆 This program will show the accuracy of the face on which it is trained, you can change the lighting condition to get better results.



## Main Program execution

```bash
  cd smart-door/face-detection
  python main.py
```
👆 Now you can play with the door bell
## Circuit and Flow Diagram
  All required diagrams are in the media folder


## Components
- [Raspberry Pi 4](https://www.indianhobbycenter.com/products/raspberry-pi-5-model-b-with-4-gb-ram?_pos=5&_sid=90d82726b&_ss=r)
- [5MP camera Module](https://www.indianhobbycenter.com/products/raspberry-pi-camera-module?_pos=1&_sid=356a5ed8f&_ss=r)
- [SG90 Mini Servo - 180 Degree Rotation](https://www.indianhobbycenter.com/products/sg90-micro-servo-motor?_pos=1&_sid=5d334fdcf&_ss=r)
- [Digital IR Sensor Module IR Proximity LM393](https://www.indianhobbycenter.com/products/ir-sensor-module?_pos=1&_sid=d9ff90827&_ss=r)
- [16x2 1602 LCD Display (Yellow / Green) with i2c module](https://www.indianhobbycenter.com/products/0829u8outcy-jce-16-x-2-lcd-display?_pos=1&_sid=24913f4a4&_ss=r)


