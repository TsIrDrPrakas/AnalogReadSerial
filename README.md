# AnalogReadSerial
This is guide to test Serial data reading using Aurdino Uno via Wokwi

>> Refer the wiring diagram in attachment
>> Copy the following code

void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
}

void loop() {
  // put your main code here, to run repeatedly:
  int sensorValue = analogRead(A0);
  Serial.println(sensorValue);
  delay(1);
}
