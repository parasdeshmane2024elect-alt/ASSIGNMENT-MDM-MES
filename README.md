# Arduino and ESP32 Embedded Systems Practicals

## 📌 Overview

This repository contains a collection of embedded systems experiments and practical implementations using **Arduino and ESP32 development platforms**. It covers fundamental to intermediate concepts in microcontroller programming, digital and analog interfacing, timers, interrupts, communication protocols, PWM generation, and sensor data acquisition.

The experiments are designed to develop practical knowledge of embedded C/C++ programming, hardware interfacing, real-time operations, and peripheral communication.

## 🎯 Objectives

- Configure the development environment for Arduino and ESP32 platforms.
- Understand digital input/output operations and LED control.
- Implement software delays and non-blocking timing techniques.
- Interface pushbuttons and implement switch debouncing.
- Display information using LCD and graphical OLED modules.
- Explore hardware timers, interrupts, and periodic tasks.
- Generate PWM signals for actuator control.
- Measure the period and frequency of external signals.
- Implement UART and SPI communication.
- Read analog sensor data using ADC and apply digital filtering.

## 🧪 Experiments

| No. | Experiment Title | Key Concepts |
|---|---|---|
| 1 | Development Environment Setup | Arduino IDE, board configuration, libraries, program uploading |
| 2 | LED Control Using Timing Methods | Digital output, software delay, non-blocking timing |
| 3 | Pushbutton-Controlled LED with Debouncing | Digital input, switch bouncing, debounce logic |
| 4 | Interfacing a 16×2 LCD | LCD initialization, text display, data and control signals |
| 5 | Timer1-Based Periodic LED Task | Hardware timers, periodic execution, pushbutton input, I²C LCD |
| 6 | PWM Signal Generation | Duty cycle, PWM, DC motor and buzzer control |
| 7 | Period and Frequency Measurement | Signal timing, pulse measurement, frequency calculation |
| 8 | UART Communication with Interrupt-Based Reception | Serial communication, transmit/receive, interrupts |
| 9 | SPI-Based Graphical OLED Interface | SPI communication, bitmap images, graphical display |
| 10 | ADC-Based Sensor Data Acquisition | Analog-to-digital conversion, sensor readings, digital filtering |

## 🛠️ Hardware and Software Requirements

### Hardware
- Arduino-compatible development board
- ESP32 development board
- LED and current-limiting resistors
- Pushbutton switches
- 16×2 LCD module
- I²C LCD module
- SPI-based graphical OLED display
- DC motor or buzzer for PWM experiments
- Analog sensors or potentiometer
- Breadboard and jumper wires
- USB cable and suitable power supply

*Note: The hardware required depends on the experiment. Not every component is needed for every practical.*

### Software
- [Arduino IDE](https://www.arduino.cc/en/software)
- [Arduino Language Reference](https://docs.arduino.cc/language-reference/)
- [ESP32 Arduino Core](https://docs.espressif.com/projects/arduino-esp32/en/latest/)
- Required libraries for the selected display and peripheral modules

## 📂 Repository Structure

```text
Arduino-ESP32-Embedded-Systems/
│
├── README.md
│
├── Experiment-01-Development-Setup/
├── Experiment-02-LED-Timing/
├── Experiment-03-Pushbutton-Debouncing/
├── Experiment-04-LCD-Interface/
├── Experiment-05-Timer1-Periodic-Task/
├── Experiment-06-PWM-Control/
├── Experiment-07-Period-Frequency-Measurement/
├── Experiment-08-UART-Interrupt-Communication/
├── Experiment-09-SPI-Graphical-OLED/
└── Experiment-10-ADC-Sensor-Filtering/
```

Each experiment folder can contain the source code, circuit diagram, pin connections, working principle, and observed results.

## 🚀 Getting Started

1. Install the Arduino IDE.
2. Configure the required board package for Arduino or ESP32.
3. Connect the development board to your computer using USB.
4. Select the correct board and communication port.
5. Install any required libraries.
6. Open the relevant experiment's `.ino` source file.
7. Verify the code and upload it to the development board.
8. Connect the required components according to the circuit diagram.
9. Observe the output using the connected hardware, Serial Monitor, or display module.

## ⚠️ Important Compatibility Notes

- **Arduino and ESP32 are different platforms:** pin assignments, timer implementations, ADC characteristics, and PWM APIs may differ.
- **Timer1:** The Timer1-based experiment must use a timer implementation supported by the selected board. AVR-specific Timer1 registers and libraries are not directly portable to ESP32.
- **PWM:** Configure PWM using the APIs supported by the selected board and core version.
- **UART:** Select the appropriate hardware serial interface and baud rate.
- **I²C and SPI:** Verify the display's communication interface, pin mapping, and library compatibility.
- **ADC:** Sensor voltage must remain within the selected board's permitted input range. ESP32 GPIOs are not 5 V tolerant.
- **Motor control:** Use a suitable motor driver and an appropriate external motor supply rather than powering a DC motor directly from a GPIO pin.

## 📚 Learning Outcomes

After completing these experiments, learners should be able to:

- Write and upload embedded programs to Arduino and ESP32 boards.
- Interface digital and analog peripherals.
- Design responsive programs using non-blocking timing.
- Understand timers, interrupts, and periodic task execution.
- Generate PWM signals and control compatible actuators.
- Implement UART and SPI communication.
- Acquire, process, and display sensor data.
- Troubleshoot basic hardware, software, and communication issues.

## 👨‍💻 Contributions

Contributions and suggestions are welcome. You can improve the repository by adding circuit diagrams, code comments, simulation results, hardware observations, or platform-specific implementations.

When contributing, ensure that the code is readable, tested on the stated platform, and accompanied by the necessary wiring details.

## 📄 License

This repository may be used for educational and learning purposes. Add a `LICENSE` file to specify the terms under which others may use, modify, and distribute the code.

---

**Keywords:** Arduino, ESP32, Embedded Systems, Microcontrollers, GPIO, LCD, OLED, PWM, UART, SPI, ADC, Timers, Interrupts, Sensor Interfacing.
