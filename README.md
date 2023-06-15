# Driver-drowsiness-detection-system-based-on-three-approaches-using-Raspberry-pi-and-machine-learning

The proposed system uses three approach for drowsiness detection. The system uses a Raspberry pi night vision camera for facial analysis, a Mi band 4 for heart rate analysis and a velostat pressure sensor for steering grip analysis.


Requirements:
Hardware requirements:
• Raspberry Pi 3 Model B+
• Raspberry Pi Night vision camera
• Mi Band 4
• Velostat pressure sensitive sheet
• woven conductive fabric
• Bluetooth speaker
• Aanalog-to-Digital Converter MCP3008

software requirements:
• VNC viewer
• Raspbian OS


Implementation:
The hardware configuration for the facial analysis method features a raspberry pi night vision camera as an input device providing real-time video stream for the raspberry pi as a computational device using OpenCV viola-jones (Haar Features) and Dlib facial landmark library for face extraction and Region of Interest (ROI) extraction, respectively. The system also uses a Bluetooth speaker to verbally alert the driver when it detects drowsiness.

The Mi Band 4 is connected to the Raspberry Pi utilising Bluetooth Low Energy, allowing for successful interaction, in the hardware configuration for the heart rate analysis method shown in the above figure. The Raspberry Pi is a computational device for heart rate analysis using a specified threshold value, and the system uses the Mi band 4 as an input device to deliver real-time Heart rate fluctuation data. The system also uses a Bluetooth speaker to verbally inform the driver when it detects drowsiness.

The strength of the driver’s steering grip is measured using the velostat pressure sensitive sheet. Since the velostat is an analogue sensor, an analog-to-digital converter is needed. The data from the pressure sensor is converted to digital form here using the MCP3008 ADC. The calculation uses the transformed data as its input to compare the received data to a predetermined threshold in order to identify drowsiness. The output device for the vocal alert to the driver upon sleepiness detection is a Bluetooth speaker.
