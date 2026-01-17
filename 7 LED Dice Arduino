const int tlpin = 13; //RED
const int tmpin = 12; //YELLOW
const int trpin = 11; //GREEN

const int mpin = 10; //BLUE

const int blpin = 9; //GREEN
const int bmpin = 8; //YELLOW
const int brpin = 7; //RED

//These were the colors I those that I liked the best :D 

const int startpin = 2;

void setup() {
  //You still be defining those pins :) 
  pinMode(tlpin, OUTPUT);
  pinMode(tmpin, OUTPUT);
  pinMode(trpin, OUTPUT);
  
  pinMode(mpin, OUTPUT);
  
  pinMode(blpin, OUTPUT);
  pinMode(bmpin, OUTPUT);
  pinMode(brpin, OUTPUT);

  pinMode(startpin, INPUT_PULLUP);

  randomSeed(analogRead(0)); //Avoids repeating same dice rolls each boot-up :) 
}

void loop() {
  bool set = digitalRead(startpin); //If pressed, it will result in 1

    if(set == LOW) {

      int rollResult = random(1,7);

      delay(200);

      if (rollResult == 1) {
        digitalWrite(mpin, HIGH);
        delay(20);
      }

      if(rollResult == 2) {
        digitalWrite(tmpin, HIGH);
        digitalWrite(bmpin, HIGH);
        delay(20);
      }
      if(rollResult == 3) {
        digitalWrite (trpin, HIGH);
        digitalWrite(mpin, HIGH);
        digitalWrite(blpin, HIGH);
        delay(20);
      }
      if(rollResult == 4) {
        digitalWrite(trpin, HIGH);
        digitalWrite(tlpin, HIGH);
        digitalWrite(brpin, HIGH);
        digitalWrite(blpin, HIGH);
        delay(20);
      }
      if(rollResult == 5) {
        digitalWrite(trpin, HIGH);
        digitalWrite(tlpin, HIGH);
        digitalWrite(brpin, HIGH);
        digitalWrite(blpin, HIGH);
        digitalWrite(mpin, HIGH);
        delay(20);
      }
      if(rollResult == 6) {
        digitalWrite(trpin, HIGH);
        digitalWrite(tlpin, HIGH);
        digitalWrite(brpin, HIGH);
        digitalWrite(blpin, HIGH);
        digitalWrite(bmpin, HIGH);
        digitalWrite(tmpin, HIGH);
        delay(20);
      }
      //That was a lot of writing of "digitalWrite", thankfully, copy & paste exists, W function 

      delay(10000); //Waits 10 seconds rq

      //Resets the pins back to off for the next time it is rolled
      digitalWrite(trpin, LOW);
      digitalWrite(tlpin, LOW);
      digitalWrite(brpin, LOW);
      digitalWrite(blpin, LOW);
      digitalWrite(bmpin, LOW);
      digitalWrite(tmpin, LOW);
      digitalWrite(mpin, LOW);
      
    }
}
//Arduino Dice :D
//January 17th, 2026
