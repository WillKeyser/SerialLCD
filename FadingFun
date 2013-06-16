/* Will Keyser
 * 2013
 * Serial LCD with blinking cursor and fade in effect
 */

#include <LiquidCrystal.h>

// initialize the library with the numbers of the interface pins
LiquidCrystal lcd(7, 8, 9, 10, 11, 12);

int ledpin = 3;            //  Pin of the backlight LED on your arduino
int brightness = 0;        //  We start our brightness at zero (nothing)
int fadeDelay = 40;        //  The delay between each new brightness value is written

void setup(){
    // set up the LCD's number of columns and rows: 
  lcd.begin(16, 2);
  // initialize the serial communications and run the fade routine (see bottom)
  // then set the cursor to blink
  Serial.begin(9600);
  pinMode(ledpin, OUTPUT);
  fadein();  
  lcd.blink();

}

void loop()
{
  //This section is the main loop where we: clear the screen, check for data, and display the data.
  if (Serial.available()) {
    lcd.clear();
    delay(90);
    while (Serial.available() > 0) {
    lcd.write(Serial.read());
  
    }
  }
}

void fadein()
/*  This is where we manually write analog values to the 
 *  backlight LED, starting at 0 and (after adding 5, 51 times)
 *  ending in 255.
 *  
 *  0 -> 255 = 0% -> 100%
 *  
 *  Rather verbose, but I was too lazy to do it the right way.
 */
{
   analogWrite(ledpin, brightness); delay(fadeDelay);    //our value is now 0
   brightness = brightness + 5;                          //our value is now 5
   analogWrite(ledpin, brightness); delay(fadeDelay);
   brightness = brightness + 5;                          //our value is now 10
   analogWrite(ledpin, brightness); delay(fadeDelay);    //and so on... :)
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);     
   brightness = brightness + 5;
   analogWrite(ledpin, brightness); delay(fadeDelay);   //255! We've lit up.
}

//Thanks for a fun Saturday evening!
