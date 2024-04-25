# Voice-Controlled Maqueen Robot Using OpenAI API and Raspberry Pi

This project demonstrates the integration of advanced natural language processing capabilities from the OpenAI API to control a Maqueen robot via voice commands, with a Raspberry Pi serving as the central control unit. This setup includes local or cloud-based speech-to-text conversion, command processing, and command execution through the Raspberry Pi and micro:bit controller on the Maqueen robot.

## Project Components

- **Maqueen Robot**: A small, versatile robot controlled by a micro:bit.
- **Micro:bit**: A microcontroller used for executing commands on the Maqueen robot.
- **Raspberry Pi**: Serves as the central processing unit, handling speech-to-text, command interpretation with OpenAI API, and command transmission.
- **Speech-to-Text Service**: Implemented locally on the Raspberry Pi or through cloud services such as Google Cloud Speech-to-Text.
- **OpenAI API**: Processes the text to understand commands and generate appropriate responses.
- **Command Translator**: Custom scripts on the Raspberry Pi translate OpenAI's responses into actions for the Maqueen robot.
- **Hardware Interface**: Communication between the Raspberry Pi and the Maqueen robot's micro:bit via Bluetooth or WiFi.

## System Diagram

Here is a diagram that illustrates the system architecture:

![image](https://github.com/TheTechieTailor/Voice-Controlled-Robotics-and-Automation-using-AI/assets/164169172/6b3a26cf-6b71-4185-a03f-2eaefeed13e4)


## Getting Started

### Prerequisites

- Micro:bit
- Maqueen robot
- Raspberry Pi with Raspbian installed
- Microphone or another voice input device
- Active internet connection, if using cloud-based speech-to-text services
- Access to OpenAI API

### Installation

1. **Set Up Your Raspberry Pi**: 
   - Install necessary software and libraries for speech-to-text and OpenAI API interaction.
   
2. **Set Up Your Micro:bit and Maqueen Robot**: 
   - Ensure your Maqueen robot is assembled and that the micro:bit is properly connected and programmed to receive commands via Bluetooth or WiFi.

3. **Install Necessary Libraries**:
   - Ensure Python and other required libraries are installed on the Raspberry Pi:
     ```bash
     pip install -r requirements.txt
     ```

4. **Configure API Keys**:
   - Obtain and securely store API keys for both Google Cloud Speech-to-Text and OpenAI.
   - Update the configuration files on your Raspberry Pi accordingly.

### Configuration

- Edit the `config.py` file on the Raspberry Pi to include your API keys and other necessary settings like network configuration for communication protocols.

## Usage

1. **Start the System**:
   - Run the main script on the Raspberry Pi to initiate the voice control interface:
     ```bash
     python main.py
     ```

2. **Issue Voice Commands**:
   - Speak directly to the microphone to control the Maqueen robot. Supported commands include "move forward", "turn left", etc.

## Development

- **Customize Commands**:
  - Add more commands by modifying the command translator script on the Raspberry Pi and updating the micro:bit's firmware to recognize new actions.
