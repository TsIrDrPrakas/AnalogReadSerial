# AnalogReadSerial

This guide demonstrates how to test serial data reading using an Arduino Uno via Wokwi.

## Project Links
- [Wokwi Project Simulation](https://wokwi.com/projects/403540223948784641)

## Instructions
1. Refer to the wiring diagram provided in the attachment.
2. Copy and upload the following code to your Arduino Uno:

```cpp
void setup() {
  // Initialize serial communication at 9600 bits per second:
  Serial.begin(9600);
}

void loop() {
  // Read the input on analog pin A0:
  int sensorValue = analogRead(A0);
  // Print the sensor value to the Serial Monitor:
  Serial.println(sensorValue);
  // Wait for a millisecond:
  delay(1);
}
