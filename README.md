# 8-Bit Parallel Communication Interface Simulator

An interactive web-based simulator designed to demonstrate the working of an **8-bit parallel communication interface** through a simple and visual interface.

## 📌 Project Overview

This project simulates the transfer of an 8-bit data byte between a **Transmitter (TX)** and a **Receiver (RX)**.

Users can:
- Enter an ASCII character and load it onto the 8-bit data bus.
- Manually toggle individual data bits D7–D0.
- Transmit the data byte using a simulated handshake sequence.
- Observe the receiver LEDs corresponding to the transmitted bits.
- View the binary, hexadecimal, decimal, and ASCII representation of the received data.
- Monitor the communication activity through a terminal log.
- Visualize the STROBE, BUSY, ACK and DATA signals using a digital waveform.

## ⚙️ Communication Sequence

The simulator demonstrates the following handshake process:

1. **STROBE** – Indicates that valid data is available.
2. **BUSY** – Indicates that the receiver is processing the data.
3. **Data Latching** – The receiver captures the 8-bit data.
4. **STROBE OFF** – Data-valid signal returns to idle.
5. **BUSY OFF** – Receiver becomes available.
6. **ACK** – Receiver sends an acknowledgement pulse.
7. **IDLE** – Communication cycle is completed.

## 🖥️ Main Features

### Transmitter Unit
- 8-bit data bus
- Manual bit toggling
- ASCII character input
- Load Character function
- Transmit Data Byte function

### Receiver Unit
- 8 LED indicators for D7–D0
- Binary display
- Hexadecimal display
- Decimal display
- ASCII character display
- Communication activity log

### Digital Oscilloscope
Displays the simulated timing relationship between:

- DATA
- STROBE
- BUSY
- ACK

## 🧠 Concepts Demonstrated

- Parallel data transmission
- 8-bit data representation
- ASCII encoding
- Binary-to-decimal conversion
- Binary-to-hexadecimal conversion
- Handshaking
- Data-valid signalling
- Receiver acknowledgement
- Digital timing diagrams

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript
- HTML Canvas API

No external libraries or frameworks are required.

## ▶️ How to Run

1. Download or clone this repository.
2. Open `index.html` in any modern web browser.
3. Enter a character or manually toggle the data bits.
4. Click **Transmit Data Byte**.
5. Observe the receiver LEDs, readout values, activity log, and waveform.

## 📂 Project Structure

```text
8-Bit-Parallel-Communication-Interface-Simulator/
│
├── index.html
└── README.md
