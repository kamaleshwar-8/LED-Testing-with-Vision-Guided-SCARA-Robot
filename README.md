# Overview

This project was an advanced version of the earlier LED testing system, now enhanced with vision guidance using a monochromatic camera mounted on the J2 joint of the Epson T6-
B602S SCARA robot. The aim was to automate the identification, testing, and sorting of randomly placed LEDs using machine vision and robotic manipulation.

# Project Outline :

- Camera-Based Detection: A monochrome vision system was used to detect LEDs that were randomly positioned and oriented on a flat surface. The number of LEDs was not fixed, simulating a realistic unsorted input scenario.
  
- Robot and Vision Calibration: The camera was mounted on J2 of the T6 SCARA, and full camera-to-robot calibration was performed using Epson RC+ Vision Guide to enable precise coordinate transformation from the camera view to robot motion space.
  
- Automated LED Testing Routine:
  - After vision detection, the robot picked one LED and placed it on a testing circuit.
  - The LED was held for 0.5 seconds, then lifted by 50 mm along Z, rotated 180° along Z-axis (to reverse polarity), and tested again after re-placement.]
  - This ensured bidirectional testing and eliminated the need for pre-sorted orientation.
    
- Sorted Placement: Once tested, the LED was not returned to the original location. Instead, it was placed in a neatly arranged line-by-line layout in a separate area, using programmed offsets to build rows dynamically.

  # Result

  Video link : https://youtu.be/Ox8jvq1gBys


<img width="715" height="883" alt="image" src="https://github.com/user-attachments/assets/0f9154ae-749f-4eaf-a6c2-d82fd28bc9f9" />

<img width="709" height="875" alt="image" src="https://github.com/user-attachments/assets/48802757-368e-46ef-bb6f-bb093721b014" />

<img width="715" height="909" alt="image" src="https://github.com/user-attachments/assets/9d612db5-4dc4-45d9-8d18-81a513ab0fcd" />
