# Water Quality Monitoring System using STM32 Microcontroller

##  Overview
This project monitors the **quality of water** using various sensors connected to an **STM32 microcontroller**.  
It measures important parameters like **pH**, **turbidity**, and **temperature**, and displays the results on an LCD or sends them wirelessly to another device.

---

##  Features
- Measures key water quality parameters:
  -  **pH Level**
  -  **Turbidity (Water Clarity)**
  -  **Temperature**
- Real-time data monitoring using STM32  
- Optional wireless data transfer (e.g., **NRF24L01** or **ESP8266**)  
- Low power consumption and compact design  

---

##  Components Used
| Component | Description |
|------------|-------------|
| **STM32F103C8T6** | Blue Pill microcontroller board |
| **pH Sensor** | Measures acidity of water |
| **Turbidity Sensor** | Detects water clarity |
| **Temperature Sensor (DS18B20)** | Measures water temperature |
| **LCD Display (16x2)** | Shows sensor data |
| **NRF24L01 / ESP8266** | (Optional) Wireless module for data transfer |
| **Power Supply** | 5V regulated |

---

##  Circuit Description
Each sensor is connected to the STM32:

- pH and Turbidity → Analog input pins  
- Temperature Sensor → Digital pin  
- LCD → I2C or parallel interface  
- Wireless module → SPI or UART interface  

---

##  Software and Tools
- **STM32CubeIDE** or **Keil uVision** for code development  
- **HAL Library** for STM32  
- **C Programming Language**  
- **Serial Monitor / LCD** for displaying readings  

---

##  How It Works
1. The sensors collect real-time water data.  
2. The STM32 processes these signals using ADC (Analog to Digital Converter).  
3. The measured values are displayed on the LCD.  
4. *(Optional)* Data is transmitted to a remote server or device wirelessly.

---
