# Digital Voting System using Arduino

This is a simple Digital Voting System built with Arduino Uno, RFID (MFRC522), a PIR sensor, and push buttons. It simulates a basic election process with real-time vote casting and result display.

## 🎯 Features
- RFID-based voter authentication
- Motion detection using PIR sensor to activate the system
- Push-button based vote casting
- LCD display shows voting options, thank-you message, and winner
- Prevents multiple voting by verifying RFID
- On-demand results display via special button

## 🛠 Components Used
- Arduino Uno
- MFRC522 RFID Module
- PIR Motion Sensor
- 16x2 I2C LCD Display
- 5 Push Buttons (4 for voting, 1 for showing result)
- Jumper Wires, Breadboard
- RFID Tags

## 📂 File Included
- `digital_voting_system.ino` — Main Arduino code



## 🔧 How It Works
1. **Motion Detection**: System stays idle until someone is detected via PIR sensor.
2. **RFID Scan**: Voter scans their RFID tag. Only authorized UIDs can vote.
3. **Vote Casting**: Voter presses a button to vote for PMLN, PTI, TLP, or PPP.
4. **Thank You Message**: LCD shows appreciation after vote is cast.
5. **Result Display**: Pressing a 5th button shows which party is currently winning.

## 📌 Notes
- You need to replace the hardcoded UID `"99 3E 3D 02"` in the code with your actual RFID tag's UID.
- Connect the push buttons to analog pins A0–A3 and digital pin 4 as configured.
- The LCD will turn off after each major action to save power.

## 👤 Author
**TALHA AHMAD**
**Talha Ahmad**  
BSCS Student – Lahore Garrison University  
