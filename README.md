# pianola-
codice dell circuito                                                         video https://youtu.be/OtaCyTJjG3g

int pos = 0;

void setup()
{
  pinMode(A0, INPUT);
  pinMode(8, OUTPUT);
  pinMode(A1, INPUT);
  pinMode(A2, INPUT);
  pinMode(A3, INPUT);
}

void loop()
{
  // if button press on A0 is detected
  if (digitalRead(A0) == HIGH) {
    tone(8, 349, 100); // play tone 57 (A4 = 440 Hz)
  }
  // if button press on A1 is detected
  if (digitalRead(A1) == HIGH) {
    tone(8, 329, 100); // play tone 59 (B4 = 494 Hz)
  }
  // if button press on A0 is detected
  if (digitalRead(A2) == HIGH) {
    tone(8, 293, 100); // play tone 60 (C5 = 523 Hz)
  }
  if (digitalRead(A3) == HIGH) {
    tone(8,261, 100); 
  }
  delay(10); // per appunto rendere meglio le note
}
