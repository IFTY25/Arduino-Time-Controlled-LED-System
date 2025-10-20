<h1 align="center">🕌 Arduino-Based Time Controlled LED System</h1>
<p align="center">
⏱️ <b>Automated LED and Buzzer Control for Prayer Time Management</b><br>
Built with Arduino Uno, DS3231 RTC, LCD, EEPROM & Push Buttons
</p>

---

## 📘 Overview  
This project introduces an **Arduino-based time-controlled LED and buzzer system** that helps users avoid *Makruh times* — specific periods during which prayers are discouraged in Islamic practice.  
The system automatically tracks time using a **DS3231 RTC**, displays status on an **LCD**, and triggers visual (LED) and audible (buzzer) alerts.  

Developed as part of the **EEE 3210 – Microprocessor, Interfacing, and System Design Lab** at  
**Ahsanullah University of Science and Technology (AUST)**.  

---

## ✨ Key Highlights  
✅ Real-time tracking using DS3231 RTC  
✅ LCD interface for displaying live clock & status  
✅ EEPROM memory to retain data after power-off  
✅ Push buttons for user configuration  
✅ Red/Green LEDs + buzzer for instant feedback  
✅ Manual override via Serial Monitor  

---

<details>
<summary><b>⚙️ Hardware Components</b></summary>

| Component | Quantity | Description |
|------------|-----------|-------------|
| Arduino Uno | 1 | Microcontroller board |
| DS3231 RTC Module | 1 | High-accuracy real-time clock |
| LCD 16x2 (I2C) | 1 | Displays time & LED status |
| Red LED | 1 | Indicates restricted (Makruh) time |
| Green LED | 1 | Indicates prayer-allowed time |
| 220Ω Resistors | 2 | Limits current for LEDs |
| Piezo Buzzer | 1 | Audio alert during restriction |
| Push Buttons | 4 | Set start/end times |
| Breadboard & Jumper Wires | 1 set | For connections |
</details>

---

<details>
<summary><b>🔧 Working Principle</b></summary>

1. **RTC** tracks the real-time clock continuously.  
2. **LCD** displays the current time and prayer status.  
3. **Push buttons** allow users to set restricted (Makruh) hours.  
4. **EEPROM** stores user data even after power loss.  
5. When current time matches Makruh range:  
   - 🔴 Red LED ON  
   - 🔔 Buzzer activated  
   - LCD shows “Restricted Time”  
6. Otherwise:  
   - 🟢 Green LED ON  
   - Buzzer OFF  
   - LCD shows “Prayer Allowed”  
</details>

---

<details>
<summary><b>🧠 Technical Details</b></summary>

- **RTC (DS3231):** Temperature-compensated, high precision, battery-backed clock  
- **EEPROM:** Stores Makruh times persistently  
- **LCD (I2C):** Reduces wiring complexity  
- **Microcontroller Logic:** Compares current vs. restricted times in real time  
</details>

---

## 🧩 Design Trade-offs  

| Aspect | Consideration |
|--------|----------------|
| ⏱️ Accuracy vs. Power | RTC provides precision while conserving power |
| 💸 Cost vs. Performance | Arduino Uno chosen for affordability and reliability |
| 🧍 User Simplicity vs. Complexity | Button interface keeps it beginner-friendly |

---

## 🧪 Implementation & Validation  

- ✅ RTC and LCD synchronization verified  
- ✅ LED & buzzer tested for correct response  
- ✅ Button input and override confirmed functional  
- ✅ EEPROM successfully retained settings post power cycle  

---

<details>
<summary><b>📊 Multidisciplinary Integration</b></summary>

| Field | Application |
|--------|-------------|
| **Electronics** | RTC, EEPROM, LED, buzzer integration |
| **Software** | Time logic, storage, and I/O handling |
| **System Design** | Reliability, low power, usability |
</details>

---

## 🌱 Ethical & Sustainable Design  
- Supports religious practices with inclusivity and neutrality.  
- Designed for ease of use and accessibility.  
- Low power consumption supports sustainability.  

---

## 🧭 Project Development  

**Phases:**  
1. 🔹 Component selection & circuit design  
2. 🔹 Software development & debugging  
3. 🔹 Integration & validation  
4. 🔹 Documentation & presentation  

**Tools Used:**  
- Arduino IDE  
- Proteus Simulation  
- Libraries: `Wire.h`, `RTClib.h`, `EEPROM.h`

---

## 🖥️ Circuit Diagram  
<h1 align="center">🕌 Arduino-Based Time Controlled LED System</h1>
<p align="center">
⏱️ <b>Automated LED and Buzzer Control for Prayer Time Management</b><br>
Built with Arduino Uno, DS3231 RTC, LCD, EEPROM & Push Buttons
</p>

---

## 📘 Overview  
This project introduces an **Arduino-based time-controlled LED and buzzer system** that helps users avoid *Makruh times* — specific periods during which prayers are discouraged in Islamic practice.  
The system automatically tracks time using a **DS3231 RTC**, displays status on an **LCD**, and triggers visual (LED) and audible (buzzer) alerts.  

Developed as part of the **EEE 3210 – Microprocessor, Interfacing, and System Design Lab** at  
**Ahsanullah University of Science and Technology (AUST)**.  

---

## ✨ Key Highlights  
✅ Real-time tracking using DS3231 RTC  
✅ LCD interface for displaying live clock & status  
✅ EEPROM memory to retain data after power-off  
✅ Push buttons for user configuration  
✅ Red/Green LEDs + buzzer for instant feedback  
✅ Manual override via Serial Monitor  

---

<details>
<summary><b>⚙️ Hardware Components</b></summary>

| Component | Quantity | Description |
|------------|-----------|-------------|
| Arduino Uno | 1 | Microcontroller board |
| DS3231 RTC Module | 1 | High-accuracy real-time clock |
| LCD 16x2 (I2C) | 1 | Displays time & LED status |
| Red LED | 1 | Indicates restricted (Makruh) time |
| Green LED | 1 | Indicates prayer-allowed time |
| 220Ω Resistors | 2 | Limits current for LEDs |
| Piezo Buzzer | 1 | Audio alert during restriction |
| Push Buttons | 4 | Set start/end times |
| Breadboard & Jumper Wires | 1 set | For connections |
</details>

---

<details>
<summary><b>🔧 Working Principle</b></summary>

1. **RTC** tracks the real-time clock continuously.  
2. **LCD** displays the current time and prayer status.  
3. **Push buttons** allow users to set restricted (Makruh) hours.  
4. **EEPROM** stores user data even after power loss.  
5. When current time matches Makruh range:  
   - 🔴 Red LED ON  
   - 🔔 Buzzer activated  
   - LCD shows “Restricted Time”  
6. Otherwise:  
   - 🟢 Green LED ON  
   - Buzzer OFF  
   - LCD shows “Prayer Allowed”  
</details>

---

<details>
<summary><b>🧠 Technical Details</b></summary>

- **RTC (DS3231):** Temperature-compensated, high precision, battery-backed clock  
- **EEPROM:** Stores Makruh times persistently  
- **LCD (I2C):** Reduces wiring complexity  
- **Microcontroller Logic:** Compares current vs. restricted times in real time  
</details>

---

## 🧩 Design Trade-offs  

| Aspect | Consideration |
|--------|----------------|
| ⏱️ Accuracy vs. Power | RTC provides precision while conserving power |
| 💸 Cost vs. Performance | Arduino Uno chosen for affordability and reliability |
| 🧍 User Simplicity vs. Complexity | Button interface keeps it beginner-friendly |

---

## 🧪 Implementation & Validation  

- ✅ RTC and LCD synchronization verified  
- ✅ LED & buzzer tested for correct response  
- ✅ Button input and override confirmed functional  
- ✅ EEPROM successfully retained settings post power cycle  

---

<details>
<summary><b>📊 Multidisciplinary Integration</b></summary>

| Field | Application |
|--------|-------------|
| **Electronics** | RTC, EEPROM, LED, buzzer integration |
| **Software** | Time logic, storage, and I/O handling |
| **System Design** | Reliability, low power, usability |
</details>

---

## 🌱 Ethical & Sustainable Design  
- Supports religious practices with inclusivity and neutrality.  
- Designed for ease of use and accessibility.  
- Low power consumption supports sustainability.  

---

## 🧭 Project Development  

**Phases:**  
1. 🔹 Component selection & circuit design  
2. 🔹 Software development & debugging  
3. 🔹 Integration & validation  
4. 🔹 Documentation & presentation  

**Tools Used:**  
- Arduino IDE  
- Proteus Simulation  
- Libraries: `Wire.h`, `RTClib.h`, `EEPROM.h`

---

## 🖥️ Circuit Diagram  
<p align="center">
  <img src="circuit/circuit_diagram.jpg" alt="Circuit Diagram" width="600">
</p>


---

## 🧰 How to Run  

1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/Arduino-Time-Controlled-LED-System.git


