int rojo = 13;
int amarillo = 12;
int verde = 11;

void setup() {
  pinMode(rojo, OUTPUT);
  pinMode(amarillo, OUTPUT);
  pinMode(verde, OUTPUT);
}

void loop() {
  // Verde encendido
  digitalWrite(verde, HIGH);
  digitalWrite(amarillo, LOW);
  digitalWrite(rojo, LOW);
  delay(3000);

  // Amarillo encendido
  digitalWrite(verde, LOW);
  digitalWrite(amarillo, HIGH);
  digitalWrite(rojo, LOW);
  delay(800);

  // Rojo encendido
  digitalWrite(verde, LOW);
  digitalWrite(amarillo, LOW);
  digitalWrite(rojo, HIGH);
  delay(3000);
}
