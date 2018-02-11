# simple-wifi-controlled-rc-car-kinect
A really simple project using a NodeMCU motor shield to convert a RC car to have WiFi controls

Extending this project so that it can be controlled by a kinect.

# Building the car
- http://www.instructables.com/id/Simple-WiFi-Controlled-RC-Car/

# Installation
### Kinect Libraries
Made use of the v1.7 libraries of Kinect for this project as I was using the XBOX 360 Kinect
 - https://www.microsoft.com/en-us/download/details.aspx?id=36996 - 1.7 SDK - Install First
 - https://www.microsoft.com/en-us/download/details.aspx?id=36998 - 1.7 Developer Toolkit

### Arduino
 - https://www.youtube.com/watch?v=AFUAMVFzpWw - Installing IDE and relevant drivers
 - Build MotorKinect-ESP8266 and copy IP address from serial monitor

### C#
If Kinect references are not picked up in your SLN file, do the following:
- Right-click project > Add > Reference
  - Add Microsoft.Kinect.dll in <PATH-TO-SDK>/v1.7/Assemblies
  - Add Microsoft.Kinect.Toolkit in <PATH-TO-DEV-TOOLKIT-1.7>/Assemblies
  - Add Microsoft.Kinect.Toolkit.Controls in <PATH-TO-DEV-TOOLKIT-1.7>/Assemblies
  - Add Microsoft.Kinect.Toolkit.Interaction in <PATH-TO-DEV-TOOLKIT-1.7>/Assemblies

Update ipFromESP8266 with IP from Serial Console in ESP8266.

# Controls:

### Motion:
- Both hands Raised in red = Forwards
- Both hands lowered in red = Backwards
- One Hand raised in Red and one hand lowered in red = Stopped

### Turning:
- Left hand in lower blue and right hand in upper blue = left
- Right hand in lower blue and left hand in upper blue = right
- Both hands in middle green = Centered

# Credits
- https://github.com/witnessmenow/simple-wifi-controlled-rc-car
- https://msdn.microsoft.com/en-us/library/hh855381
- http://www.instructables.com/id/Kinect-SDK-Hello-World/
