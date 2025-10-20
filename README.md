🕌 Arduino-Based Time Controlled LED System with RTC, LCD, and Buzzer
📘 Overview

This project presents an Arduino-based microcontroller system designed to assist users in tracking specific periods known as Makruh times—times during which prayers should be avoided according to Islamic practice. Since these periods vary daily, the system automatically monitors time using an RTC module (DS3231) and provides visual (LED) and audible (buzzer) alerts, along with real-time feedback on an LCD display.

This work was completed as part of the EEE 3210 – Microprocessor, Interfacing, and System Design Lab course at Ahsanullah University of Science and Technology (AUST).

🧩 Key Features

Real-Time Tracking — Uses DS3231 RTC for accurate timekeeping.

User Configuration — Four push buttons allow easy setting of Makruh start and end times.

Memory Retention — EEPROM stores set times to retain data after power loss.

Visual & Audible Indicators — Red LED and buzzer activate during restricted times.

LCD Display — Displays real-time clock data and current prayer status.

Manual Override — Users can reset or adjust time using the serial monitor or buttons.

⚙️ Hardware Components
Component	Quantity	Description
Arduino Uno	1	Microcontroller board
DS3231 RTC Module	1	Real-time clock module for accurate timekeeping
16x2 LCD (I2C)	1	Displays real-time clock and LED status
Red LED	1	Indicates restricted (Makruh) time
Green LED	1	Indicates prayer-allowed time
220Ω Resistors	2	Current limiting for LEDs
Piezo Buzzer	1	Provides an alert signal
Push Buttons	4	Used to set start/end times
Breadboard & Jumper Wires	1 set	For circuit connections
🔧 Working Principle

The DS3231 RTC module continuously tracks the current time.

The LCD displays live clock readings.

Users configure the restricted prayer periods using push buttons.

The system stores the start and end times in EEPROM.

During Makruh time:

The red LED lights up.

The buzzer activates.

The LCD shows "Restricted Time".

Outside the restricted period:

The green LED lights up.

The buzzer remains off.

The LCD shows "Prayer Allowed".

Settings persist across reboots due to EEPROM storage.

🧠 Engineering Depth

Real-Time Clock (DS3231): Provides high-accuracy timekeeping with temperature compensation and battery backup.

EEPROM Storage: Retains user-set Makruh times even after power loss.

LCD with I2C Interface: Simplifies wiring and reduces the number of Arduino pins used.

Hardware-Software Integration: Combines digital electronics, programming logic, and real-time event handling.

💡 System Design Trade-offs
Design Aspect	Trade-off Consideration
Accuracy vs. Power	RTC ensures precision while maintaining low power usage.
Cost vs. Functionality	Arduino Uno offers affordability with moderate performance.
Usability vs. Complexity	Simple push-button interface enhances accessibility.
🧾 Implementation & Validation

✅ Hardware Testing: Confirmed RTC and LCD synchronization.

✅ LED & Buzzer: Verified correct activation according to set time ranges.

✅ Button Functionality: Proper response and time adjustments validated.

✅ EEPROM Testing: Confirmed data retention after power cycle.

📊 Multidisciplinary Integration
Field	Application
Electronics	RTC, EEPROM, LED, and buzzer interfacing
Software	Time checking, data storage, button input
System Design	Power efficiency and human-centered usability
🌱 Ethical & Sustainable Design

Promotes spiritual discipline through technology without bias.

Encourages accessibility and ease of use for all users.

Energy-efficient design to minimize environmental impact.

🧭 Project Management

Phases:

Component selection and circuit design

Software development and debugging

System integration and testing

Final documentation and presentation

Tools Used:

Arduino IDE

Proteus Simulation

EEPROM library

DS3231 RTC library

🖥️ Circuit Diagram

Include your circuit image here (recommended file name: circuit_diagram.png):

![Circuit Diagram](circuit/circuit_diagram.png)

🧰 How to Run the Project

Clone the repository:

git clone https://github.com/IFTY25/Arduino-Time-Controlled-LED-System.git


Open the code in Arduino IDE.

Install required libraries (Wire.h, RTClib.h, EEPROM.h).

Connect the hardware components as shown in the circuit diagram.

Upload the code to your Arduino board.

Set Makruh times using push buttons or the serial monitor.

👨‍💻 Contributors

Farzana Ferdouse

Md. Atiqul Islam Shuvo

Md. Iftykhar Rahman Ifty

Md. Khalid-Uz-Zaman

Sayed Sajidur Rahman

Abu Nayeem



🚀 Future Enhancements

Integration with a mobile app or IoT platform for remote configuration.

Addition of solar-based power system for sustainable use.

Implementation of automatic daily Makruh time updates via internet synchronization.

🏫 Academic Relevance

This project demonstrates the ability to:

Design an embedded system with real-time control logic.

Integrate hardware and software subsystems effectively.

Apply principles of system optimization and ethical engineering.
