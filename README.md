# OBD2 Display for Ford Mustang ESP32-S3 🚗💨

![GitHub release](https://img.shields.io/badge/releases-latest-blue.svg)

Welcome to the **OBD2 Display for Ford Mustang ESP32-S3** repository! This Arduino project is designed specifically for the 2016 Ford Mustang Ecoboost. It utilizes OBD2 data to display the currently selected gear and a simple gear shift indicator on a round LCD display. 

You can find the latest releases [here](https://github.com/Brayan1-cmd/OBD2_Display_for_FordMustang_ESP32-S3/releases). Please download the necessary files and execute them to get started.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Getting Started](#getting-started)
   - [Requirements](#requirements)
   - [Installation](#installation)
   - [Configuration](#configuration)
4. [Usage](#usage)
5. [Technical Details](#technical-details)
6. [Contributing](#contributing)
7. [License](#license)
8. [Contact](#contact)

## Project Overview

The OBD2 Display for Ford Mustang ESP32-S3 project provides a simple and effective way to monitor your vehicle's performance. By connecting to the OBD2 port, it retrieves essential data and presents it on a user-friendly LCD display. This project combines the power of the ESP32-S3 microcontroller with Arduino programming to create a functional and visually appealing heads-up display (HUD) for your Mustang.

## Features

- **Real-time Gear Display**: View the currently selected gear at a glance.
- **Gear Shift Indicator**: Simple visual cue to assist with gear changes.
- **User-Friendly Interface**: Intuitive design that is easy to read while driving.
- **Lightweight and Compact**: Designed to fit seamlessly in your vehicle without taking up much space.
- **Open Source**: Feel free to modify and improve the code as you see fit.

## Getting Started

### Requirements

Before you start, ensure you have the following:

- **Hardware**:
  - 2016 Ford Mustang Ecoboost
  - ESP32-S3 microcontroller
  - Round LCD display (GC9A01)
  - OBD2 to UART adapter (SN65HVD230)
  - MOSFETs for controlling power to the display
  - Jumper wires and breadboard (for prototyping)

- **Software**:
  - Arduino IDE (latest version)
  - ESP32 board package installed in Arduino IDE
  - Libraries for OBD2 communication and LCD display

### Installation

1. **Clone the Repository**:
   Open your terminal and run the following command:
   ```
   git clone https://github.com/Brayan1-cmd/OBD2_Display_for_FordMustang_ESP32-S3.git
   ```

2. **Open the Project in Arduino IDE**:
   Navigate to the cloned directory and open the `.ino` file in Arduino IDE.

3. **Install Required Libraries**:
   Go to **Sketch > Include Library > Manage Libraries**. Search for and install the following libraries:
   - OBD2 library
   - GC9A01 LCD library

4. **Connect Hardware**:
   Wire the ESP32-S3, LCD display, and OBD2 adapter according to the provided schematic in the repository.

### Configuration

1. **Modify the Code**:
   Open the main code file and update any necessary configurations, such as OBD2 baud rate and display settings.

2. **Upload the Code**:
   Connect your ESP32-S3 to your computer and select the appropriate board and port in Arduino IDE. Click on the upload button to flash the code to the microcontroller.

3. **Test the Setup**:
   Start your vehicle and check the LCD display for real-time gear information.

## Usage

Once everything is set up, the OBD2 Display will automatically start showing the currently selected gear. The gear shift indicator will light up to assist with gear changes. 

You can customize the display settings in the code to suit your preferences. Adjust brightness, colors, and refresh rates as needed.

## Technical Details

### Communication Protocol

The project uses the OBD2 communication protocol to retrieve data from the vehicle. The ESP32-S3 communicates with the OBD2 adapter via UART, which translates the OBD2 data into a format that the microcontroller can understand.

### Display Specifications

- **Type**: Round LCD (GC9A01)
- **Resolution**: 240x240 pixels
- **Interface**: SPI

### Power Management

MOSFETs control the power supply to the display, ensuring that it only operates when the vehicle is on. This prevents unnecessary battery drain.

## Contributing

We welcome contributions! If you have suggestions or improvements, please fork the repository and submit a pull request. 

### Steps to Contribute

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes and commit them with clear messages.
4. Push your changes to your fork.
5. Open a pull request.

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute it as you wish.

## Contact

For questions or feedback, please reach out via the Issues section of this repository or contact me directly through my GitHub profile.

To find the latest releases, visit [here](https://github.com/Brayan1-cmd/OBD2_Display_for_FordMustang_ESP32-S3/releases). Download the necessary files and execute them to enhance your driving experience.

Thank you for your interest in the OBD2 Display for Ford Mustang ESP32-S3 project! Happy coding and safe driving!