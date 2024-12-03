# Arduino Temperature and Humidity Display

This repository contains code for an Arduino project that reads ambient temperature and humidity using a **DHT22 sensor** and displays the data on an **LCD screen**. This project is perfect for beginners learning about sensors, displays, and microcontroller programming.

---

## Features
- Reads **temperature** (°C/°F) and **humidity** (%) using the DHT22 sensor.
- Displays the readings on a **16x2 LCD screen** with real-time updates.
- Easy-to-follow wiring and setup instructions.

---

## Components
1. **DHT22 Sensor**  
   Measures ambient temperature and humidity.

2. **16x2 LCD Display**  
   Displays the temperature and humidity readings. Uses the **I2C backpack** for easy connection.

3. **Arduino Board**  
   Compatible with boards like Arduino Uno, Nano, or Mega.

4. Miscellaneous:
   - Breadboard
   - Jumper wires
   - Resistors (if needed)

---

## Circuit Diagram
Connect the components as shown below:

| Component      | Arduino Pin |
|----------------|-------------|
| DHT22 Data Pin | D2          |
| LCD SDA        | A4          |
| LCD SCL        | A5          |
| Power (VCC/GND)| 5V/GND      |

> **Note:** Pins for SDA and SCL may vary based on your Arduino board.

---

## Libraries Used
- [Adafruit DHT Library](https://github.com/adafruit/DHT-sensor-library)  
  For reading data from the DHT22 sensor.
  
- [LiquidCrystal_I2C Library](https://github.com/johnrickman/LiquidCrystal_I2C)  
  For controlling the LCD display via I2C.

---

## Installation
1. Clone this repository:
   ```bash
   https://github.com/Kirroslink/simple-weather-checker/blob/main/Code%20file
   ```
2. Install the required libraries via Arduino IDE:
   - Open **Library Manager** (`Sketch > Include Library > Manage Libraries...`).
   - Search for "DHT" and install the **Adafruit DHT sensor library**.
   - Search for "LiquidCrystal I2C" and install the library.

3. Open the `dht22_lcd.ino` file in the Arduino IDE.

---

## Usage
1. Wire the components as described in the circuit diagram.
2. Upload the code to your Arduino board.
3. Open the Serial Monitor (optional) to see real-time temperature and humidity readings.
4. The LCD screen will display the following:
   ```
   Temp: 25.3°C
   Humidity: 60.5%
   ```

---

## Customization
- Modify the code to:
  - Switch between Celsius and Fahrenheit.
  - Add alerts for specific temperature or humidity thresholds.
- Use a different display or sensor as needed.

---

## Troubleshooting
- If the LCD doesn't display anything, ensure:
  - The I2C address in the code matches your LCD's address (default: `0x27`).
  - The SDA/SCL pins are correctly connected.
  
- If the sensor readings are incorrect, check:
  - The wiring and power supply to the DHT22.
  - Sensor compatibility with the library version.

---

## Contributing
Feel free to fork this repository, make improvements, and submit pull requests! Any contributions are welcome.

---

## License
This project is licensed under the GNU General Public License. See `LICENSE` for details.

---

Happy coding! 😊

