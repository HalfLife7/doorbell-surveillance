# Doorbell Surveillance with Facial Recognition

# **Tasks for Each Members**

# Setup

- **Setting up development environment and tools (Thanh Tran)**
  - Raspbian installation and configuration
  - PyCharm for IDE
  - Git with Github
- **Facial Recognition – Installing the dependencies and getting it to work (David Nguyen)**
  - Install dlib
  - Cv2
  - imutils
- **Hardware Configuration**
  - Picamera with picamera dependency (David Nguyen)
  - PIR motion sensor with gpiozero dependency (Thanh Tran)
  - Breadboard LED

# Coding

Main.py

- **Facial Recognition –** [https://www.pyimagesearch.com/2018/06/25/raspberry-pi-face-recognition/](https://www.pyimagesearch.com/2018/06/25/raspberry-pi-face-recognition/)
- **Send Email –** Thanh Tran
  - When unknown person with link to view camera remotely
- **Send Text Message –** Thanh Tran
  - When unknown person with link to view camera remotely
- **Live-stream of Camera to Website –** David Nguyen
- **Toggle LED –** Thanh Tran
  - Lights up red if unknown, green if camera is on and yellow if face is recognized
- **Motion Detection –** Thanh Tran and David Nguyen
  - Sensor is too sensitive

encode\_faces.py

- --Takes 5 pictures over 20 seconds
- --Updates the database with new set of photos / person

Index.php - Site to view camera feed and send text-to-speech to speaker

- Text-to-to speech through input text not working – David
  - Uses espeak module
  - sudo is required to run python scripts through webpage
  - sudo does not work with espeak on our raspberry pi
- Send command to run encode\_faces.py - David
  - Requires parameter to set firstname\_lastname