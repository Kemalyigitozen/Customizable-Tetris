## 🛠️ Installation and Setup Guide

Follow the steps below to build and run this project on your own hardware.

### 1. Installing Required Libraries
To ensure the graphics and game dynamics run smoothly, you need to install the **Adafruit** libraries via the Arduino IDE.

1. Open the Arduino IDE.
2. Go to **Sketch** > **Include Library** > **Manage Libraries...** from the top menu.
3. Use the search bar to find and install the following libraries:
   * **Adafruit GFX Library:** For basic graphics and shape drawing.
   * **Adafruit ILI9341:** The hardware driver for the TFT display.

### 2. Circuit Setup and Wiring
Proper wiring between the Raspberry Pi Pico, the ILI9341 display, and the control buttons is crucial for the components to communicate.

Please wire the circuit on your breadboard exactly as shown in the **pinout diagram** provided in this repository. The basic logic is as follows:
* **ILI9341 Display:** Connect the SPI pins (SCK, MOSI, CS, etc.) to the corresponding SPI pins on the Pico, and VCC to the 3.3V output, as indicated in the diagram.
* **Control Buttons:** Connect one leg of the movement (Right, Left, Down) and rotate buttons to the specified Pico GPIO pins, and the other leg directly to the common GND (Ground) line. (Internal Pull-Up resistors are enabled in the code).

### 3. Uploading the Code
1. Once the wiring is complete according to the schematic, connect your Raspberry Pi Pico to your computer using a USB cable.
2. In the Arduino IDE, make sure you have selected the correct board (Raspberry Pi Pico) and the corresponding Port.
3. Open the main project code and click the **Upload** button.
4. Once the upload is complete, the screen will boot up and the game will be ready to play!
