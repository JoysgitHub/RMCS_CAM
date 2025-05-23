# <img src="static/images/RMCS.png" alt="RMCS Image" width="100" style="display:inline;"> RMCS
Remote AI Mobile CCTV System for Red Teamers



# Setup:
## MOBILE RTSPCAMERA (Raspberrypi 0 w 2):
Hardware:
  -  Raspberry Pi 0 W 2
  -  4G LTE Module (use OTG port ethernet for stable connection)
  -  [Night Vision Camera IR CUT](https://www.amazon.co.uk/Dorhea-Raspberry-Camera-Automatic-Adjustable/dp/B07DNSKMZ1/ref=sr_1_9)
  -  Power Bank

Software:
  - Remote.it (Raspberry pi agent)
  -  RTSP_CAM/*

Download RTSPCAM folder to raspberry pi and change creadentials in .yml 

run RTSPCAM/setup.sh on raspberrypi 0  w 2 to setup rtsp camera

## C2 CAMERA SERVER
Hardware:
  - PC
  - External Storage (USB drive, SSD, HDD)
    
Software:
 - Remote.it (TCP tunnel for secure remote feed access) 
 - FFMPEG 
 - RMCS_CAM/app.py
   
Create a Pushbullet account and add API key to RMCS/APPS/describe.py to enable notifications

download push bullet app and login 

run pip install -r requirements.txt to install libraries
run python3 app.py to start server
