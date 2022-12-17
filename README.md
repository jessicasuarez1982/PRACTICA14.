// C++ code
//
int on = 0;

void setup()
{
  pinMode(10, INPUT);
  pinMode(13, OUTPUT);
  pinMode(12, OUTPUT);
}

void loop()
{
  if (digitalRead(10) == HIGH) {
    digitalWrite(13, HIGH);
    digitalWrite(12, LOW);
    delay(4000); // Wait for 4000 millisecond(s)
    digitalWrite(13, LOW);
    digitalWrite(12, HIGH);
    delay(2000); // Wait for 2000 millisecond(s)
  }
}
