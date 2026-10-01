# Accident Alert System

A smart accident detection and emergency alert system built using Arduino Uno. The system detects sudden impact using a MEMS accelerometer, reads the vehicle location using GPS, and sends alerts through GSM to emergency contacts or rescue services.

## Overview

Road accidents often lead to delays in emergency response due to limited real-time location and communication. This project addresses that issue by automatically identifying crashes and notifying emergency services with the exact accident location.

The prototype uses:
- Arduino Uno as the main controller
- MEMS accelerometer to detect impact
- GPS module to fetch latitude and longitude
- GSM module to send SMS/call alerts
- Buzzer and LCD display for local indication

## Features

- Detects sudden vehicle impact using vibration/accelerometer data
- Fetches live GPS coordinates after accident detection
- Sends emergency SMS with location link
- Makes a voice call to a predefined emergency number
- Displays crash status on an LCD screen
- Allows manual reset using a button

## System Workflow

1. The MEMS sensor continuously monitors motion and vibration.
2. When an abnormal impact is detected, the Arduino identifies it as a possible accident.
3. GPS module fetches the current coordinates.
4. GSM module sends the accident alert and location to the emergency number.
5. The buzzer activates and the system displays the alert on the LCD.

## Hardware Components

- Arduino Uno
- MEMS Accelerometer Sensor
- GPS Module (NEO-6M)
- GSM Module (SIM800L)
- 16x2 LCD with I2C
- Buzzer
- Emergency button
- Power supply and connecting wires

## Repository Contents

- [Arduino Source Code](accident%20alert%20system/accidentcode.txt)
- [Project Report / Documentation](accident%20alert%20system/Accident%20Alert%20System.pdf)
- [System Screenshot 1](accident%20alert%20system/Screenshot%202025-06-27%20100527.png)
- [System Screenshot 2](accident%20alert%20system/Screenshot%202025-06-27%20100543.png)
- [Demo Video 1](accident%20alert%20system/VID-20250627-WA0004.mp4)
- [Demo Video 2](accident%20alert%20system/VID-20250627-WA0006.mp4)
- [Demo Video 3](accident%20alert%20system/VID-20250627-WA0007.mp4)
- [Demo Video 4](accident%20alert%20system/VID-20250627-WA0009.mp4)

## Project Images

![System Overview](accident%20alert%20system/Screenshot%202025-06-27%20100527.png)

![Alert System Interface](accident%20alert%20system/Screenshot%202025-06-27%20100543.png)

## Working Principle

The accelerometer continuously measures changes in the axis values. If the change crosses a predefined threshold, the system considers the event as a collision. The Arduino then triggers the GPS module, obtains the coordinates, and uses the GSM module to notify emergency responders. This helps reduce response time and increases the chance of saving lives.

## How to Use

1. Connect the Arduino Uno with the accelerometer, GPS module, GSM module, buzzer, and LCD as shown in the project documentation.
2. Upload the code from [accidentcode.txt](accident%20alert%20system/accidentcode.txt) to the Arduino board.
3. Power the system.
4. Monitor the LCD and ensure the GPS/GSM modules are connected properly.
5. Simulate or trigger an impact to observe the emergency notification.

## Notes

- The emergency phone number is defined inside the code and can be changed as needed.
- Before using the GSM module, verify the correct SIM and network connectivity.
- The GPS module may take a short time to acquire coordinates depending on signal quality.

## Future Improvements

- Add a mobile app or web dashboard for real-time monitoring
- Integrate cloud storage and emergency logs
- Improve threshold logic to reduce false accident detection
- Add more sensors for better accident confirmation
- Support multiple emergency contacts

## Conclusion

This project demonstrates an affordable and practical accident alert system that can help reduce emergency response time during road accidents. It is suitable for academic, prototype, and IoT-based safety applications.

---

For more details, please view the [project report](accident%20alert%20system/Accident%20Alert%20System.pdf).