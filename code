#define CUSTOM_SETTINGS
#define INCLUDE_GAMEPAD_MODULE
#include <DabbleESP32.h>

const int ENA = 21;
const int IN1 = 22;   // left motor
const int IN2 = 23;

const int IN3 = 25;
const int IN4 = 26;  // Right Motor
const int ENB = 27;

const int ENA_channel = 1;
const int ENB_channel = 2; // pwm configuration
const int pwmFreq = 5000;
const int pwmResolution = 8;

void setup() {

pinMode(IN1, OUTPUT);
pinMode(IN2, OUTPUT);

pinMode(IN3, OUTPUT);
pinMode(IN4, OUTPUT);

ledcSetup(ENA_channel, pwmFreq, pwmResolution);
ledcAttachPin(ENA, ENA_channel);

ledcSetup(ENB_channel, pwmFreq, pwmResolution);
ledcAttachPin(ENB, ENB_channel);

Dabble.begin("WirelesslyCar");

}



void loop() {

Dabble.processInput();

if (GamePad.isUpPressed()) {
  digitalWrite(IN1, HIGH); digitalWrite(IN2, LOW); digitalWrite(IN3, HIGH); digitalWrite(IN4, LOW);
  ledcWrite(ENA_channel, 255); ledcWrite(ENB_channel, 255); }

else if(GamePad.isDownPressed()) {
  digitalWrite(IN1, LOW); digitalWrite(IN2, HIGH); digitalWrite(IN3, LOW); digitalWrite(IN4, HIGH); 
  ledcWrite(ENA_channel, 255); ledcWrite(ENB_channel, 255);  }

else if (GamePad.isRightPressed()) {
  digitalWrite(IN1, LOW); digitalWrite(IN2, LOW); digitalWrite(IN3, HIGH); digitalWrite(IN4, LOW); 
  ledcWrite(ENA_channel, 0); ledcWrite(ENB_channel, 180); }

else if(GamePad.isLeftPressed())  {
 digitalWrite(IN1, HIGH); digitalWrite(IN2, LOW); digitalWrite(IN3, LOW); digitalWrite(IN4, LOW); 
  ledcWrite(ENA_channel, 180); ledcWrite(ENB_channel, 0); }

else {
  digitalWrite(IN1, LOW); digitalWrite(IN2, LOW); digitalWrite(IN3, LOW); digitalWrite(IN4, LOW); 
  ledcWrite(ENA_channel, 0); ledcWrite(ENB_channel, 0); }



}
