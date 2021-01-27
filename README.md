# NotSoBasicArduino
 The follwing files are my second foray into Arduino
 
 
## Table of Contents
* [Table of Contents](#TableOfContents)
* [LED_Fade](#LED_Fade)
* [Hello_LCD](#Hello_LCD)
* [FillMeInLAter](#FillMeInLAter)
---

## LED_Fade

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
// set the brightness of pin 9:
  analogWrite(led, brightness);

  // change the brightness for next time through the loop:
  brightness = brightness + fadeAmount;

  // reverse the direction of the fading at the ends of the fade:
  if (brightness <= 0 || brightness >= 255) {
    fadeAmount = -fadeAmount;
  }
```
Talk about how the fade works, here....
Once the brightness h
### Evidence
https://create.arduino.cc/editor/helmstk1/9e044cca-43d7-4d93-885f-e6dec5b4f769/preview

### Images
![led](https://user-images.githubusercontent.com/71342179/105392979-d1c83a80-5be9-11eb-94cc-38b8c1660e23.png)

### Reflection

This was very hard because I didn't learn any code in Buford so im going to have to watch tons of tutorials and stuff to catch myself up and hopefully succeed.

## Hello_LCD

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
Code goes here
```
Talk about how the code works, here....

### Evidence
link goes here

### Images
draw it yourself, take a picture, make a fritzing, whatever you want to EFFECTIVELY communicate how its put together.

### Reflection




## Finite_LED_Blinker

### Description & Code


```C++
int ledPin = 13;              // LED connected to digital pin 13

void setup() {
  pinMode(ledPin, OUTPUT);    // sets the digital pin as output
}

void loop() {
  digitalWrite(ledPin, HIGH); // sets the LED on
  delay(1000);                // waits for a second
  digitalWrite(ledPin, LOW);  // sets the LED off
  delay(1000);                // waits for a second
}
```


### Evidence
https://create.arduino.cc/editor/jaust80/1cbdaf40-41ad-44d1-b06d-bc525368b117
### Images
![Finite_Led_Blinker](https://user-images.githubusercontent.com/71342179/105927365-dccc0200-6011-11eb-80cd-1a1f2673fda7.PNG)
### Reflection




## Photoresistor

### Description & Code

```C++
int ledPin = 3;
int photocellInput = 0;
 
void setup()  {
  pinMode(ledPin, OUTPUT);
}
 
 
void loop()  {
 
  photocellInput = (analogRead(0)/4); // Divides input 0-1023 to resemble to 0-255
 
  analogWrite(ledPin, photocellInput);  
  // The delay can be change to get the desired dimming effect
  delay(20);                            
}
```

### Evidence
https://create.arduino.cc/editor/jaust80/580ee2e9-14a5-4107-9f9f-673b2e87416d
### Images
![Wiring](https://user-images.githubusercontent.com/71342179/105926833-c4a7b300-6010-11eb-9313-209dfbcccfea.png)
### Reflection
I have no idea what I'm doing but google helped me so that's nice.
