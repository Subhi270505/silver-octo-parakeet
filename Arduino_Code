int mq3Pin = A0; // MQ3 sensor connected to A0
int buzzer = 8;  // Buzzer or LED connected to pin 8
int threshold = 400; // Adjust based on your sensor's output

void setup() {
  Serial.begin(9600);
  pinMode(buzzer, OUTPUT);
}

void loop() {
  int sensorValue = analogRead(mq3Pin);
  Serial.print("Alcohol Level: ");
  Serial.println(sensorValue);

  if (sensorValue > threshold) {
    digitalWrite(buzzer, HIGH); // Alert ON
  } else {
    digitalWrite(buzzer, LOW);  // Alert OFF
  }

  delay(500);
}
