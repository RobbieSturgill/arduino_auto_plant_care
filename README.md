Automated Plant Watering System
This Arduino-based project aims to create an automated plant watering system that monitors the soil moisture levels of multiple plants and controls the water pumps accordingly. The system also features an OLED display for visual feedback and a rotary encoder for user input.

Hardware Components
Arduino board (e.g., Arduino Uno, Nano, or Mega)
Soil moisture sensors (4x)
Relay modules (4x)
Water pumps (4x)
OLED display (I2C compatible)
Rotary encoder
Breadboard, jumper wires, and power supply

Pin Connections

Soil moisture sensors:
MOISTURE_1: A0
MOISTURE_2: A1
MOISTURE_3: A2
MOISTURE_4: A3

Relay modules:
RELAY_1: 2
RELAY_2: 3
RELAY_3: 4
RELAY_4: 5

Rotary encoder:
ENCODER_A: 6
ENCODER_B: 7
ENCODER_BUTTON: 8

OLED display (I2C protocol):
SCL: A5 (default SCL pin on most Arduino boards)
SDA: A4 (default SDA pin on most Arduino boards)

Software Dependencies
Arduino IDE
U8g2 library for the OLED display
Encoder library for the rotary encoder

Setup
Install the required libraries using the Arduino IDE.
Connect the hardware components according to the pin definitions.
Upload the provided code to your Arduino board.
Adjust the desired moisture level using the rotary encoder.
How it works
The system reads the moisture levels from the soil moisture sensors and computes the error based on the desired moisture level. A PID loop is used to calculate the appropriate pump time for each plant. The relay modules control the water pumps based on the calculated pump times. The OLED display shows the current moisture levels and pump times for each plant. The rotary encoder allows the user to adjust the desired moisture level, and the system recalculates the pump times accordingly.

Customization
You can customize the code to suit your specific needs, such as adding more plants, adjusting the PID constants, or implementing different control algorithms. Make sure to update the pin definitions and hardware connections accordingly if you make any changes to the project.




Regenerate response

