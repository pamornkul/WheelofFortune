int timeShowRandom = 3000;
int timeShowDecision = 6000;
int timeBlink = 100;
int buttonPin = 1;
int buttonPress = false;
int randomNumber=5;
int previousNo = 0;
int timePassed = 0;
int min=2;
int x=0;
int count=0;

void getRandomNo(int min, int ex) {
  //Serial.println();
 int rand = random(min,ex);
  if (rand == previousNo) {
   getRandomNo(min,ex);
  } else {
    randomNumber = rand;
    previousNo = randomNumber;
  }
  //Serial.println(rand);
}
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
   for (int i=2;i<=13;i++){
    pinMode(i, OUTPUT);
    }
    pinMode(A1, OUTPUT);digitalWrite(A1, LOW);
    pinMode(A2, OUTPUT);digitalWrite(A2, LOW);
    pinMode(A3, OUTPUT);digitalWrite(A3, LOW);
    pinMode(A4, OUTPUT);digitalWrite(A4, LOW);
    pinMode(A5, OUTPUT);digitalWrite(A5, LOW);
    pinMode(A6, OUTPUT);digitalWrite(A6, LOW);
   // pinMode(A7, OUTPUT);digitalWrite(A7, LOW);
    Serial.begin(9600);
}

// the loop function runs over and over again forever
void loop() {
    x=analogRead(A7);
   //Serial.println(x);
 if (x < 100 && buttonPress == false ) {
     buttonPress = true;
     Serial.println(count);
  } if (buttonPress == true ) {
    int j;
    for (j=1;j<=5;j++){
    for (int i=2;i<=13;i++){
      digitalWrite(i, HIGH);
      delay((80*j));
      digitalWrite(i,LOW);
      delay(10); 
     }}
   
      getRandomNo(min,13); // Get random pin number
      for (int i=min;i<=randomNumber;i++){
      digitalWrite(i, HIGH);
      delay((80*j));
      digitalWrite(i,LOW);
      delay(10); 
     }
     digitalWrite(randomNumber, HIGH);
       delay(5000);
     }
   
    
    //count++;
    buttonPress = false;
    //delay(5000);
  }
  
