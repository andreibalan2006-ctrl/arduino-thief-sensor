# Arduino Ultrasonic Radar with NeoPixel Display

This repository contains an Arduino-based radar simulation built in Tinkercad. The project uses an ultrasonic sensor to detect objects and maps their position on a NeoPixel LED ring, creating a visually appealing "radar sweep" and a fading trail effect.

## 🛠️ Components Used
- 1x Arduino Uno
- 1x HC-SR04 Ultrasonic Sensor
- 1x Micro Servo
- 1x NeoPixel Ring 12 (Adafruit)
- Breadboard & Jumper Wires

## 🔌 Circuit Diagram & Connections

Make sure to wire the components exactly as follows:

**HC-SR04 Ultrasonic Sensor:**
- `VCC` ➔ Arduino 5V
- `GND` ➔ Arduino GND
- `Trig` ➔ Arduino Pin 10
- `Echo` ➔ Arduino Pin 11

**Micro Servo:**
- `Power` (Red) ➔ Arduino 5V
- `Ground` (Brown/Black) ➔ Arduino GND
- `Signal` (Orange/Yellow) ➔ Arduino Pin 9

**NeoPixel Ring 12:**
- `PWR` (5V) ➔ Arduino 5V
- `GND` ➔ Arduino GND
- `IN` (Data Input) ➔ Arduino Pin 6
- *Note: The `OUT` pin on the NeoPixel ring must remain disconnected.*

## 🚀 How It Works
1. **Mechanical Sweep:** The servo motor sweeps from 0 to 180 degrees and back.
2. **Object Detection:** The HC-SR04 sensor measures the distance to any object in front of it during the sweep.
3. **Visual Mapping:** The 180-degree field of view is mapped to the 12 LEDs
