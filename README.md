#  Hand Gesture–Based LED Control System

A real-time LED control system driven by hand gestures using **MediaPipe**, **OpenCV**, and **Arduino Uno**. Designed for contactless control, this system interprets hand movements to toggle LEDs and adjust brightness—no buttons or switches required.

##  Project Highlights

-  **Gesture Detection:** Uses **MediaPipe** and **OpenCV** to detect hand and finger landmarks in real time via webcam.
-  **LED Control:** Gestures are mapped to specific LED actions (on/off, brightness) and sent to an **Arduino Uno** via **Serial Communication**.
-  **Brightness Adjustment:** LED brightness varies based on the **vertical position of the hand** (higher hand = brighter).
-  **Real-Time Processing:** Uses lightweight models optimized for 30–60 FPS without needing a GPU.

##  Tools & Technologies

- **MediaPipe** – For hand landmark detection.  
- **OpenCV** – For image/video processing.  
- **PySerial** – For serial communication with Arduino.  
- **Arduino Uno** – Controls LED outputs using received data.

##  System Workflow

1. **Capture** live video using a webcam.
2. **Detect** hand gestures using MediaPipe.
3. **Process** the finger status and hand position.
4. **Send** corresponding signals over serial to Arduino.
5. **Control** LEDs (on/off + brightness) using PWM output.


