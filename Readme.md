# Smart Lock with RFID and Fingerprint Authentication

![Arduino](https://img.shields.io/badge/Platform-Arduino-blue)
![RFID](https://img.shields.io/badge/Technology-RFID-green)
![Biometric](https://img.shields.io/badge/Technology-Fingerprint-orange)
![IITRPR](https://img.shields.io/badge/Project-IIT%20Ropar-yellow)

---

## Overview

This project implements a **Smart Lock System** that integrates **RFID** and **Fingerprint** authentication using an **Arduino** board.  
Users can unlock the system using either an authorized RFID card or a registered fingerprint.  
It provides enhanced **security**, **ease of access**, and **dual-mode authentication** for homes, labs, or offices.

**Course:** GE107 — Tinkering Lab  
**Institution:** Indian Institute of Technology Ropar  

**Team Members:**
- Rahul Yadav — 2022MEB1334  
- Rajeev Kumar — 2022MEB1335  
- Sumer Mohan Singh Bassi — 2022MEB1351  
- Tejasva Jindal — 2022MEB1359  
- Vineet Kumar — 2022MEB1366  

---

## Working Principle

1. The system waits for an RFID card or fingerprint input.  
2. The Arduino verifies the input against a list of **pre-registered authorized users**.  
3. If authenticated:
   - The **servo motor or solenoid lock** unlocks the door.  
   - A **buzzer or LCD** gives feedback to the user.  
4. Unauthorized attempts trigger a warning or denial message.  

This combination of **RFID** and **biometric** technology ensures flexibility and strong access control.

---

## Components Used

| Component | Description |
|------------|-------------|
| Arduino Uno / Mega / Nano | Main controller board |
| RFID Module (MFRC522) | Reads RFID tags/cards |
| Fingerprint Sensor (R305 / GT-511C3) | Captures and verifies fingerprints |
| Servo / Solenoid Lock | Controls the locking mechanism |
| Relay Module | Power interface for lock |
| LCD Display (optional) | Displays user messages |
| Buzzer, LEDs | Feedback indicators |
| Power Supply | 5V DC regulated supply |
---

## 💻 Arduino Code

The main program is located at:

/code/smart_lock.ino

### Required Libraries
Install these from the Arduino IDE Library Manager:
- `MFRC522` (for RFID module)
- `Adafruit Fingerprint Sensor Library` (for R305 module)
- `Servo.h` (for controlling servo motor)

### Uploading Instructions
1. Open `smart_lock.ino` in Arduino IDE.  
2. Connect your Arduino via USB.  
3. Select the correct COM port and board type.  
4. Click **Upload**.  
5. Present a registered RFID tag or fingerprint to test authentication.

---

## Demonstration Videos

- 🎥 [RFID Unlock Demo](videos/RFID_demo.mp4)  
- 🎥 [Fingerprint Unlock Demo](videos/Fingerprint_demo.mp4)

---

## Future Improvements

- Add **dual-factor authentication** (RFID + Fingerprint together)  
- Include **data logging** for access history  
- Integrate with **IoT / Wi-Fi modules** (ESP8266 or ESP32)  
- Implement **mobile notifications** for access events  

---

## License

This project is open-sourced under the **MIT License**.  
Feel free to use or modify with appropriate citation.

---



