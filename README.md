# LifeLine-Mini-Smart-ECG-Monitoring-with-TinyML-and-Geo-Alerting
LifeLine Mini is a portable, offline smart ECG monitoring system that uses ESP32 and TinyML for real-time arrhythmia detection. It integrates GPS and GSM to automatically send emergency SMS alerts with location details, while providing live ECG visualization and data logging for future analysis.


# ❤️ LifeLine Mini: Smart ECG Monitoring with TinyML and Geo-Alerting

## 📌 Overview

**LifeLine Mini** is a portable, offline ECG monitoring and emergency alert system designed to detect abnormal heart rhythms in real time.

The system uses an **AD8232 ECG sensor** to acquire cardiac signals and an **ESP32 microcontroller** for signal processing. A **TinyML model** deployed on the ESP32 classifies ECG rhythms as normal or abnormal without requiring cloud processing.

When an abnormal rhythm is detected, the system obtains the user's location using a **NEO-7M GPS module** and sends an emergency SMS through the **SIM800L GSM module**. An **OLED display** provides real-time ECG visualization, while a **MicroSD card** stores ECG data for later analysis.

---

## 🎯 Objectives

- Develop a portable ECG monitoring system using ESP32 and AD8232.
- Perform real-time ECG signal acquisition and filtering.
- Implement TinyML for on-device arrhythmia detection.
- Display ECG waveform and system information on an OLED.
- Obtain real-time location using GPS.
- Send automatic emergency SMS alerts through GSM.
- Store ECG readings and events on a MicroSD card.
- Operate independently without Wi-Fi, cloud services, or smartphones.

---

## ✨ Key Features

- ❤️ Real-time ECG monitoring
- 🧠 TinyML-based arrhythmia detection
- 📍 GPS location tracking
- 📱 Automatic GSM emergency SMS
- 📊 Real-time OLED ECG waveform
- 💾 MicroSD data logging
- 🔋 Battery-powered portable design
- 🌐 Offline operation

---

## 🛠️ Hardware Components

| Component | Purpose |
|---|---|
| ESP32 DevKitC | Main processing and control unit |
| AD8232 | ECG signal acquisition |
| SIM800L | GSM-based SMS alerting |
| NEO-7M | GPS location tracking |
| SSD1306 OLED | ECG waveform and status display |
| MicroSD Card Module | ECG and event data logging |
| 18650 Li-ion Battery | Portable power supply |
| ECG Electrodes | Capture cardiac electrical signals |

---

## 💻 Software & Technologies

- Arduino IDE
- C/C++
- ESP32
- TinyML
- Edge Impulse
- EMA Signal Filtering
- TinyGPSPlus
- Adafruit GFX
- Adafruit SSD1306
- SPI / I2C / UART

---

## ⚙️ System Working

The working process of LifeLine Mini is:

**ECG Acquisition → Signal Filtering → TinyML Classification → Normal/Abnormal Detection**

If the ECG is normal, the system continues monitoring.

If an abnormal rhythm is detected:

**Abnormal ECG → GPS Location → GSM SMS Alert → Data Logging**

The OLED continuously displays ECG waveform and system information.

---

## 🔄 System Flow

1. Initialize ESP32 and connected modules.
2. Acquire ECG signals using the AD8232 sensor.
3. Apply EMA filtering to reduce signal noise.
4. Process the ECG data using the TinyML model.
5. Classify the rhythm as Normal or Abnormal.
6. Display ECG waveform and status on the OLED.
7. If an abnormal rhythm is detected:
   - Obtain GPS coordinates.
   - Generate an emergency alert.
   - Send the alert through SIM800L.
   - Store the event on the MicroSD card.
8. Continue real-time monitoring.

---

## 📷 Project Output

### ECG Waveform Output

![ECG Waveform Output](images/ecg-output.jpg)

### ECG Monitoring on OLED

![OLED ECG Output](images/oled-output.jpg)

### GPS Location Output

![GPS Location](images/gps-output.jpg)

### Emergency SMS Alert

![Emergency SMS Alert](images/sms-alert.jpg)

### Final Prototype

![Final Prototype](images/prototype.jpg)

---

## 📊 Results

The developed system successfully demonstrated:

- Real-time ECG signal acquisition and OLED visualization.
- TinyML-based classification of normal and abnormal ECG patterns.
- GPS coordinate acquisition for emergency location tracking.
- Automatic GSM-based emergency SMS alerts.
- ECG and event logging using a MicroSD card.
- Offline operation without requiring Wi-Fi or cloud services.

---

## 🚀 Applications

- Rural healthcare
- Elderly patient monitoring
- Home ECG monitoring
- Ambulances and first-aid units
- Disaster-response environments
- Remote healthcare centres
- Field medical applications

---

## 🔮 Future Enhancements

- Multi-lead ECG monitoring
- Advanced TinyML models for multiple arrhythmia types
- Optional IoT cloud dashboard
- Mobile application integration
- Custom compact PCB design
- Improved battery management
- Buzzer and vibration emergency alerts

---

