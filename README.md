# Home Automation with PICSimLab

This project demonstrates a home automation system utilizing **PICSimLab** to control temperature, humidity, and lighting with a focus on IoT integration through the **Blynk IoT** platform. The system uses various sensors to monitor environmental conditions and actuators to respond to user commands or environmental changes.

## Features

- **Temperature Control:** Automatically adjusts or alerts based on set temperature thresholds.
- **Humidity Control:** Monitors and maintains ideal humidity levels.
- **Lighting Control:** Allows on/off toggling for lights.
- **Blynk IoT Integration:** Provides remote control and monitoring capabilities from a smartphone or web dashboard.

## Components

- **Microcontroller:** PIC microcontroller (simulated in PICSimLab)
- **Sensors:** Temperature and humidity sensors for environmental monitoring
- **Actuators:** Light control (relay simulation)
- **Blynk IoT:** For remote monitoring and control of the home environment

## Prerequisites

1. **PICSimLab**: A simulation environment to emulate PIC microcontroller circuits.
2. **Blynk IoT App**: To connect and control the device remotely.
3. **Blynk Library**: Install the Blynk library in PICSimLab for IoT integration.

## Getting Started

### 1. Setup PICSimLab

- Download and install [PICSimLab]([https://sourceforge.net/projects/picsim/]).
- Load the project simulation file or set up a new project with the necessary components (temperature and humidity sensors, relay for lights, etc.).
  
### 2. Connect to Blynk IoT

- Download the **Blynk IoT App** on your mobile device.
- Create a new project in the app and add the necessary widgets (temperature, humidity, and button controls).
- Get the **auth token** from the Blynk app and add it to the code.

### 3. Code

- Upload the provided code to simulate the microcontroller behavior.
- Configure the Blynk library with your `auth token`, Wi-Fi credentials, and pin mappings for the simulated sensors and actuators.

### 4. Run the Simulation

- Start the simulation in PICSimLab.
- Open the Blynk app to monitor and control the environment.
  
## Code Explanation

The code is divided into different sections for each functionality:

1. **Temperature Monitoring and Control**:
   - Reads temperature data and sends it to Blynk for monitoring.
   - Controls the relay based on temperature thresholds.
  
2. **Humidity Monitoring**:
   - Reads humidity data and sends it to Blynk for real-time monitoring.
  
3. **Lighting Control**:
   - Toggles lighting via relay when triggered from the Blynk app.

## Blynk Dashboard Setup

- **Temperature Display**: Add a `Value Display` widget linked to the virtual pin receiving temperature data.
- **Humidity Display**: Add a `Value Display` widget linked to the virtual pin for humidity.
- **Light Control Button**: Use a `Button` widget to toggle light relay on/off.

## Future Enhancements

- Add security features like door lock/unlock control.
- Integrate voice commands or AI-based environment prediction.
- Expand to other IoT platforms for broader compatibility.
