# Finger Bend Detection System – ESP32

An embedded system based on the ESP32 microcontroller that detects finger bending using flex sensors and displays corresponding letters on an OLED screen.

## 📌 Project Overview

This project implements a glove equipped with flex sensors to detect finger bend levels. Based on predefined thresholds, specific hand configurations are recognized and mapped to letters, which are then displayed on an OLED screen.

The project focuses on hardware–software integration, analog signal processing, and low-level embedded programming.

## External resources

- 7x14 bitmap font, file: X11fixed7x14.h
  Author: Markus Kuhn
  Source: http://www.cl.cam.ac.uk/~mgk25/

## ⚙️ Hardware

- ESP32 microcontroller  
- 5x flex sensors (one per finger)  
- OLED display (I2C)  
- Resistors and wiring  
- Power supply  
- Glove used as a base for mounting sensors  

## 🧠 How It Works

1. Flex sensors change resistance depending on finger bend.
2. ESP32 reads analog values using ADC.
3. Values are compared against defined thresholds.
4. Specific finger configurations are mapped to letters.
5. The detected letter is displayed on the OLED screen.

## 🛠️ Software Features

- Analog signal reading using ESP32 ADC  
- Threshold-based classification of finger positions  
- OLED initialization and control via I2C  
- Frame buffer implementation for displaying characters  
- Real-time update of displayed output  

## 🧩 My Contribution

This was a 2-person academic project. My main responsibilities included:

-Creation of a buffer responsible for handling the entire keyboard logic

-Reading data from flex sensors using the ADC

-Implementation of a protection function preventing simultaneous readings from two sensors

-Implementation of an OLED display function that shows which sensor state is currently active (each sensor operates in two states)

Both team members participated in:
- Hardware assembly  
- Soldering and wiring  

## 🧪 What I Learned

- Working with analog sensors and ADC on ESP32  
- Interfacing peripherals using I2C  
- Writing low-level display handling code  
- Hardware–software integration in embedded systems  

## 🚀 Possible Improvements

- Calibration for different hand sizes  
- Support for more letters / gestures  
- Smoother signal processing  
- Wireless output (e.g. Bluetooth)

## 📷 Demo

<img width="1004" height="1323" alt="image" src="https://github.com/user-attachments/assets/26f32f6d-660a-4cc8-a224-c5c124dde4b8" />



- C 
- ESP32  
- ADC  
- I2C  
- Embedded systems
