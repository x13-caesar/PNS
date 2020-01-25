# Parking Spots Hunter

This is a tool helping you automatically find avaiable parking spots and send you message alert. It's based on Python3, using object detection algorithm Maks R-CNN and some popular cloud services. 

![logo](https://pbs.twimg.com/media/ELdI0KPW4AI-K9M?format=png&name=medium)

## Requirements
Python 3.4, TensorFlow >=1.3+, Keras >=2.0.8, and other modules in requirements.txt

## Getting Started
1. **start.sh** is a linux command line script helping you set up all requirements for this project. You **MUST** run it before starting to use this project.
2. **parking_spots_hunter.py** is the main code for Parking Spots Hunter. Run it to start use our tool. It will automatically show the pictures with bounding boxes of cars and parking spots and send alert to you notifying newly empty space. 
3. To **costomize** this project to fit your own purpose and devices, you need to change following **configs**:
- **Twilio** config: API configs of Twilio
- **ROOT_DIR**: the root directory of this project
- **VIDEO_SOURCE**: Video file or camera to process - set this to 0 to use your webcam instead of a video file
- **INTERVAL**: How many frames we skip by one catching. Default to be 100.
4. **mask\_rcnn\_coco.h5** is pre-trained Mask R-CNN weights file. It's trained on COCO database. You can replace it by your own weights but please remember to adjust *parking_spots_hunter.py* related part.

## Contact Info
If any more questions, please contact following address:  
- Qiangwen Xu: qxu47@fordham.edu  
- Mengyao Sun: msun54@fordham.edu  
- Bailing Fu: bfu6@fordham.edu   
**Credit to our Professor, [Dr.Yijun Zhao](https://www.fordham.edu/info/25112/cis_faculty_and_administration/10363/yijun_zhao)**


