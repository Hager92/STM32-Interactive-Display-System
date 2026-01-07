# Interactive Display System using STM32

## Overview

This project is an **Interactive Display System** developed as a graduation project using **STM32 microcontrollers**. The system consists of two STM32 units—a **Transmitter** and a **Receiver**—communicating via the **UART protocol** to provide synchronized visual output and user interaction.

The system allows users to interact through **push buttons**, displaying corresponding **text, patterns, and images** on an **LED matrix, LCD, and TFT display**, creating an engaging and interactive experience.

---

## System Architecture

* **Transmitter (STM32)**
  Handles user input, LED matrix control, and data transmission.

* **Receiver (STM32)**
  Manages LCD and TFT displays and renders images received via UART.

Communication between both units is achieved using **UART**, while the **TFT display** is interfaced using **SPI**.

---

## Key Features

* Dual STM32 microcontroller architecture
* UART communication between transmitter and receiver
* SPI-based TFT display control
* LED matrix word display
* Interactive push-button control
* Dynamic image and text rendering
* System-wide reset functionality

---

## Hardware Components

* **STM32F401CC Microcontroller**
* **LED Matrix**
* **Push Buttons**
* **LEDs**
* **LCD Display**
* **TFT Display (SPI Interface)**

---

## Software Drivers

### LIB

* BIT_MATH
* STD_Types

### MCAL

* RCC
* GPIO
* NVIC
* SysTick
* USART
* SPI

### HAL

* LCD
* TFT
* LED Matrix

---

## Tools Used

* **FastStone Photo Resizer** – Image resizing for TFT
* **LCD Image Converter** – Image-to-array conversion (R5G6B5)
* **LED Matrix Studio** – Word pattern extraction for LED matrix

---

## Transmitter Functionality

* Detects button presses
* Displays words like **“BLOSSOM”** and **“BUTTERCUP”** on the LED matrix
* Controls LEDs for visual feedback
* Sends UART commands to the receiver
* Includes a **reset mechanism** using a dedicated button

---

## Receiver Functionality

* Receives commands via UART
* Displays corresponding text on the LCD
* Renders images on the TFT display
* Uses SPI for high-speed image transfer
* Supports full system reset and screen clearing

---

## Communication Protocols

* **UART** – Communication between STM32 transmitter and receiver
* **SPI** – TFT display interface

---

## Future Enhancements

* Hardware-based password security system
* Biometric authentication support
* Interactive games with sound integration
* Animated GIF display with hardware acceleration
* Multimedia support with audio output
