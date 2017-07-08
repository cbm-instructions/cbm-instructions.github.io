---
title: "Informatik-Rangers: Akustik-Wand"
categories: instructions
layout: post
date: 2017-07-05 11:59:59 +0200
--- 

<img src="/images/informatik_rangers/intro.jpg" height="1024">

## Einleitung
Die Akustik-Wand wurde im Rahmen der Vorlesung Challenge Based Making an der Hochschule Mannheim vom Team Informatik-Rangers erstellt. Zu Beginn der Vorlesung wurde den Studenten eine Challenge gestellt. Diese sollte dann unter Verwendung des menschenzentrierten Lösungsansatzes "Design Thinking" bewältigt werden.

### Challenge
Wie könnten Menschen in der „Smart HS Mannheim“ durch deren intelligente Geräte und Objekte dabei unterstützt werden, angenehmer und spielerischer zu arbeiten?

### Point of View
Wie können wir den Studenten im ~Helpdesk~ studentischen Arbeitsraum helfen, eine ruhigere Arbeitsumgebung zu schaffen, damit sie konzentrierter arbeiten können?

### Beschreibung des fertigen Produkts

Bei der Akustik-Wand handelt es sich um eine Trennwand, welche in Arbeitsräumen mit vielen Menschen aufgestellt werden kann, um eine angenehmere Akustik zu schaffen. Gleichzeitig wird Rückmeldung bei zu starker Lärmentwicklung geboten und somit indirekt die Lautstärkeentwicklung reduziert.

## Materialien und Werkzeug

### Material
- 1x Pin Stellwand (200cm hoch, 110cm Breite)
- 12x [Akustikschaumstoff Platten](https://www.amazon.de/Noppenschaumstoff-Akustik-Schaumstoff-Akustikschaumstoff-D%C3%A4mmung/dp/B004JVY8A4/ref=sr_1_2) (50cm x 50cm)
- 2x [Arduino Uno](http://www.exp-tech.de/arduino-uno-smd-r3)
- 2x [Electret Microphone Amplifier](http://www.exp-tech.de/adafruit-electret-microphone-amplifier-max4466-with-adjustable-gain)
- 1x [LED-Streifen](http://www.exp-tech.de/adafruit-neopixel-digital-rgb-led-weatherproof-strip-60-led-4m-white)
- 1x Pappschachtel (ca. 20 cm x 20 cm)
- 6x Plexiglasstreifen normal (150 cm x 3 cm)
- 1x [Steckplatine](https://www.amazon.de/Neuftech-Breadboard-Steckbrett-Experimentierboard-Steckplatine/dp/B00PIMRREC/ref=sr_1_4)
- 22x [Drahtbrücken Kabel](https://www.amazon.de/wiederverwendbare-Steckbrett-Drahtbr%C3%BCcke-Schaltung-Schaffen/dp/B008U4ZOLI/ref=sr_1_40?s=ce-de&ie=UTF8&qid=1498597569&sr=1-40&keywords=breadboard)
- 1x [10er Set Schaltlitzen](https://www.amazon.de/Original-Donau-Kupfer-Litzen-Germany/dp/B01BI1G88C/ref=sr_1_1)
- 1x [Rolle Klebeband](https://www.amazon.de/Klebeband-Gewebeband-Panzerband-Panzertape-schwarz/dp/B00BZ5EXO8/ref=sr_1_15)
- 1x [Rolle Backpapier Weiß](https://www.amazon.de/Ibili-200730-Backpapier-10-m-x-30-cm/dp/B00717TA56/ref=sr_1_1)
- 1x [Rolle Klebefilm](https://www.amazon.de/tesa-Klebebandabroller-Kompakter-Tischabroller-Anti-Rutsch-Technologie/dp/B00EEAIPVS/ref=sr_1_4)
- 1x [USB 2.0 Kabel A-Stecker auf B-Stecker](https://www.amazon.de/AmazonBasics-USB-2-0-Druckerkabel-Stecker-B-Stecker/dp/B00NH13DV2/ref=sr_1_1)
- 2x [Netzteil](https://www.amazon.de/Goobay-NTS-1000-MW-Schaltnetzteil/dp/B002E4WNWI/ref=sr_1_19)
- Ca. 90x [Pinnadeln](https://www.amazon.de/Outus-Karte-Nagel-Pinnadeln-Plastik/dp/B01LX88MBN/ref=sr_1_1)

### Werkzeug
- 1x [Lötkolben](https://www.amazon.de/Einstellbare-Temperatur-Unterschiedliche-L%C3%B6tspitzen-Verschiedentlich/dp/B01LXH7BLN/ref=sr_1_3)
- 1x [Heißklebepistole](https://www.amazon.de/Blusmart-Hei%C3%9Fklebepistole-Klebesticks-Klebepistole-Handwerkprojekte/dp/B01K1Z0OAO/ref=sr_1_4)
- 1x [Schere](https://www.amazon.de/AmazonBasics-Schere-weichem-Griff-Titan-Scherenbl%C3%A4tter/dp/B01BRGUC9Y/ref=sr_1_4)
- 1x [Kabelzange](https://www.amazon.de/Br%C3%BCder-Mannesmann-Werkzeug-M10989-Abisolierzange/dp/B002QZT7CO/ref=sr_1_7)

## Vorkenntnisse und Vorbereitung

### Benötigte Vorkenntnisse

Löten, die Benutzung einer Heißklebepistole sowie der grundlegende Umgang mit einem Arduino werden in dieser Anleitung vorausgesetzt.

### Vorbereitung

Zu Beginn sollte die Mitte der Trennwand ausgemessen werden auf der später der LED-Streifen befestigt wird. Zudem kann die Anordnung der Akustikplatten geplant werden. Hierbei ist zu beachten, das auf beiden Seiten ein Freiraum für den Geräusch-Sensor gelassen werden muss.

<img src="/images/informatik_rangers/layout-0.jpg" height="256">

<img src="/images/informatik_rangers/layout-1.jpg" height="512">

## Step-by-Step Guide

### Übersicht

1. LED-Streifen
1. Plexiglas Verzierung
1. Akustikplatten
1. Geräusch-Sensoren
1. Schaltungen
1. Code
1. Verkleidung
1. Quellcode

### LED-Streifen

<img src="/images/informatik_rangers/led.jpg" height="256">

1. Abmessen der Länge jedes LED-Streifens. (Hinweis: Streifen auf der Rückseite muss länger sein, da dieser unter der Pinnwand hindurch bis in den Schaltkasten geführt wird.)
1. Zuschneiden des LED-Streifens in die passende Länge.
1. Löten der Kabel an die Input-Seite der LED-Streifen. (Hinweis: "CI" Pin befindet sich auf der Input-Seite, "CO" Pin auf der Output-Seite der LED-Streifen.)

#### Befestigung der LED-Streifen

<img src="/images/informatik_rangers/led-attachment-0.jpg" height="256">
 
<img src="/images/informatik_rangers/led-attachment-1.jpg" height="256">

1. Anpinnen des Streifens am oberen Ende der Pinnwand mit der ("CO") Output-Seite oben. (Hinweis: Zum anpinnen können die nicht verwendeten Lötstellen des Streifens verwendet werden um Pinnadeln durch zu stecken.)
1. Einklemmen der LED-Streifen mit zwei Pinnadeln am unteren Ende.

### Plexiglas Verzierung

<img src="/images/informatik_rangers/decoration-draft.jpg" height="256">

1. Befestige zwei Plexiglasstreifen auf einem dritten Plexiglasstreifen mit Heißkleber zum erzeugen einer U-Förmigen Röhre. (Siehe Abbildung oben.)
1. Zuschneiden eines langen Streifens Backpapier, welcher die komplette Röhre füllen kann.
1. Befestigen des Backpapiers mit Klebefilm.
1. Wiederholen der Schritte für die zweite Plexiglas Verzierung der Rückseite.

Tipp: Alternativ kann bereits milchiges Plexiglas benutzt werden. So erspart man sich das Backpapier.

#### Befestigung der Plexiglas Verzierung

<img src="/images/informatik_rangers/decoration-0.jpg" height="512">

<img src="/images/informatik_rangers/decoration-1.jpg" height="512">

1. Beide Seiten der Plexiglas Verzierung mit Klebeband versehen.
1. Das überstehende Klebeband mit der nicht klebenden Seite an die Plexiglas Verzierung klappen und mit einem zusätzlichen kleinen Streifen Klebeband in dieser Position fixieren. (Erleichtert das anbringen an der Pinnwand)
1. Plexiglas Verzierung an Pinnwand anbringen.
	1. Anheben der Plexiglas Verzierung an die gewünschte Position.
	1. Zusätzliche Klebebandstreifen entfernen und Plexiglas Verzierung mit dem Klebeband an der Pinnwand fixieren.
1. Klebeband an der Pinnwand mit Pins befestigen, für zusätzliche Stabilität.
1. Wiederholen für die zweite Plexiglas Verzierung an der Rückseite.

### Akustikplatten

<img src="/images/informatik_rangers/acoustic_foam.jpg" height="256">

1. Anpinnen der Platten an der Pinnwand, bevorzugt mit Pinnadeln mit einem schwarzem Kopf. (Anordnung aus Planung entnehmen.)

### Geräusch-Sensoren
Die Geräusch-Sensoren werden in den horizontalen Zwischenräumen der Akustikplatten platziert.

<img src="/images/informatik_rangers/sound-sensor.jpg" height="256">

1. Länge der benötigten Leitungen messen. (Etwas mehr schadet hier nicht.)
1. Anbringen der Leitungen an den Sensoren.
	1. Zuschneiden der Leitungen auf gewünschte Länge.
	1. Abisolieren der Leitungsenden.
	1. Löten der Leitungen an die Geräusch-Sensoren.
1. Anpinnen der Sensoren an der Pinnwand.
1. Verstecken der Leitungen hinter den Akustikplatten.
	1. Führen der Leitungen in die Mitte der Pinwand.
	1. Verstecken der Leitungen hinter dem LED-Streifen.

### Schaltungen

<img src="/images/informatik_rangers/schaltungende.jpg" height="512">

1. Ankleben der Steckplatine mittig am unteren Ende der Pinnwand.
1. Anpinnen der Arduinos rechts über der Platine, sodass die Kabelanschlüsse nach rechts aussen gerichtet sind.
1. Verkabelung der Schaltung
	1. Plus- und Minuspole der LED-Streifen werden an den Plus- und Minuspol des oberen Arduinos angeschlossen.
	1. Die CI Anschlüsse der beiden LED-Streifen werden an den PIN 5 des oberen Arduinos angeschlossen.
	1. Der DI Anschluss des LED-Streifens der Vorderseite wird an den PIN 3 des oberen Arduinos angeschlossen.
	1. Der DI Anschluss des LED-Streifens der Rückseite wird an den PIN 4 des oberen Arduinos angeschlossen.
	1. Plus- und Minuspole der Laustärkesensoren werden an den Plus- und Minuspol des unteren Arduinos angeschlossen.
	1. Der Output des Lautstärkesensors der Vorderseite wird an den PIN A0 des unteren Arduinos angeschlossen.
	1. Der Output des Lautstärkesensors der Rückseite wird an den PIN A1 des unteren Arduinos angeschlossen.
	1. Verbinden der Minuspole der beiden Arduinos.
	1. Ein weiteres Kabel wird für die Kommunikationsverbindung der Arduinos benötigt. Dieses sollte aber erst im nächsten Kapitel, nachdem die Programme aufgespielt wurden, angeschlossen werden.
1. Anschließen der Netzteile an die Arduinos

#### Schaltplan
<img src="/images/informatik_rangers/schaltung.png" height="800">

### Code

Nachdem die Komplette Schaltung und alle elektronischen Komponenten an der Wand befestigt sind, wird es Zeit die Programme aufzuspielen.

1. Verbinden der Arduinos mit einem Rechner.
1. Starten der Arduino IDE und öffnen der Programme "Sender" und "Receiver".
1. Falls die Kommunikationsverbindung der Arduinos besteht, muss diese getrennt werden. (Pins Tx - Rx)
1. Aufspielen des "Sender" Programms auf den unteren Arduino. (Der der mit den Sensoren verbunden ist)
1. Aufspielen des "Receiver" Programms auf den oberen Arduinos. (Der der mit den LED-Streifen verbunden ist)
1. Trennen der USB-Verbindung zum unteren Arduino (dem Sender).
1. Verbinden der Kommunikationsverbindung der Arduinos. (Pins Tx - Rx.)

Nun sind die Programme und somit auch die ganze Schaltung voll funktionsfähig. Jedoch müssen unter Umständen noch einige Konstanten im Programm an die Schaltung bzw. an die Sensoren angepasst werden. Mehr hierzu im nächsten Kapitel.

Hinweis: Wird die USB-Verbindung zum Arduinos mit dem Sender Programm nicht getrennt, werden die Messwerte der Sensoren verfälscht.

#### Test, Kalibrierung und Fehlerbehandlung
Da jeder Raum seine eigene Akustik besitzt und die Wertebereiche je nach Anwendungsgebiet variieren können, müssen noch einige Konstanten an die Gegebenheiten des Einsatzgebietes angepasst werden. Hierfür sind folgende Schritte durchzuführen:

1. Öffnen des seriellen Plotters des Empfänger Arduinos.
1. Definieren der Schwellwerte
	1. Ermitteln eines Grenzwertes für den jeweiligen Sensor, ab dem es zu laut ist und die Anzeige steigen soll.
	1. Setzen der Konstanten "lowerLimitFront" und "lowerLimitBack" auf die ermittelten Grenzwerte.
	1. Ermitteln eines Grenzwertes für den jeweiligen Sensor, ab dem es viel zu laut ist und die Anzeige noch schneller ansteigen soll.
	1. Setzen der Konstanten "higherLimitFront" und "higherLimitBack" auf die ermittelten Grenzwerte.
1. Trennen der Kommunikationsverbindung der Arduinos (Tx - Rx)
1. Neu aufspielen des "Receiver" Programms.
1. Verbinden der Kommunikationsverbindung der Arduinos (Tx - Rx)

Hinweis: Füllt sich die LED-Anzeige nicht, obwohl es zu laut ist, so sollte man die Schwellwerte für den entsprechenden Sensor etwas herabsetzen. Füllt sich die LED-Anzeige, obwohl es leise genug ist, so sollten die Randwerte des entsprechenden Sensors etwas erhöht werden.

### Verkleidung

<img src="/images/informatik_rangers/panel.jpg" height="256">

1. Ausschneiden eines Freiraums an den Seiten, für die ausgehenden Leitungen. (Arduino, Netzteil und LED-Streifen.)
1. Dekorieren, einfärben, bemalen der zur Verkleidung verwendeten Pappschachtel.
1. Anbringen der Verkleidung mithilfe von Pinnadeln.

## Ideen zur Weiterentwicklung

* Wenn die Lautstaerkeanzeige auf dem Maximalwert ist könnte ein zusätzlicher Effekt auftreten, beispielsweise könnte die LED-Leiste anfangen zu blinken um noch mehr Aufmerksamkeit auf sich zu ziehen.

## Quellcode

### Sound Receiver

```CPP
#include <Adafruit_DotStar.h>

// Because conditional #includes don't work w/Arduino sketches...
#include <SPI.h>         // COMMENT OUT THIS LINE FOR GEMMA OR TRINKET
//#include <avr/power.h> // ENABLE THIS LINE FOR GEMMA OR TRINKET


// Number of LEDs per strip
#define NUMPIXELS_FRONT 105 
#define NUMPIXELS_BACK  132

// LED stripe pins
#define DATAPIN_FRONT 3
#define DATAPIN_BACK  4
#define CLOCKPIN      5

// Colors
#define COLOR_BLACK 0x000000
#define COLOR_GREEN 0xFF0000
#define COLOR_YELLOW 0xFFFF00
#define COLOR_RED 0x00FF00

// Sensor pins
#define SENSOR_INPUT_FRONT  A0 //sensor nr.: 515
#define SENSOR_INPUT_BACK   A1 //sensor nr.: 510.5


Adafruit_DotStar strip = Adafruit_DotStar(
  NUMPIXELS_FRONT, DATAPIN_FRONT, CLOCKPIN, DOTSTAR_BRG);
Adafruit_DotStar strip2 = Adafruit_DotStar(
  NUMPIXELS_BACK, DATAPIN_BACK, CLOCKPIN, DOTSTAR_BRG);  
// The last parameter is optional -- this is the color data order of the
// DotStar strip, which has changed over time in different production runs.
// Your code just uses R,G,B colors, the library then reassigns as needed.
// Default is DOTSTAR_BRG, so change this if you have an earlier strip.

// Hardware SPI is a little faster, but must be wired to specific pins
// (Arduino Uno = pin 11 for data, 13 for clock, other boards are different).
//Adafruit_DotStar strip = Adafruit_DotStar(NUMPIXELS, DOTSTAR_BRG);

void setup() {
  Serial.begin(9600);
  #if defined(__AVR_ATtiny85__) && (F_CPU == 16000000L)
    clock_prescale_set(clock_div_1); // Enable 16 MHz on Trinket
  #endif

  strip.begin(); // Initialize pins for output
  strip.show();  // Turn all LEDs off ASAP

  strip2.begin();
  strip2.show();

  strip.setBrightness(100);
  strip2.setBrightness(100);
}


// led strip start positions
const int startPositionFront = 13;
const int startPositionBack = 40;

const int displayLength = 90;
const int stateLowerLimit = 0;
const int stateHigherLimit = displayLength / 2;

const int minBrightness = 10;
const int maxBrightness = 200;
const double brightnessFactor = (maxBrightness - minBrightness) / displayLength;

// threshold values:
const double lowerLimitFront = 15.0;         // quiet -> noisy
const double higherLimitFront = 20.0;        // noisy -> loud
const double lowerLimitBack = 18.5;
const double higherLimitBack = 20.5;

int stateSensor1 = 0;
int stateSensor2 = 0;

double rmsFrontSensor = 0, rmsBackSensor = 0;


void loop() {
  if (Serial.available()) {
    readNewSoundValues();
    
    Serial.print("Sound Values (Front, Back): ");
    printValues(rmsFrontSensor, rmsBackSensor);
    
    // update thermostates
    stateSensor1 = updateThermoState(rmsFrontSensor, stateSensor1, lowerLimitFront, higherLimitFront, true);
    stateSensor2 = updateThermoState(rmsBackSensor, stateSensor2, lowerLimitBack, higherLimitBack, false);
    //printValues(stateSensor1, stateSensor2);

    // update led strips
    updateThermoLed(strip, stateSensor1, startPositionFront);
    updateThermoLed(strip2, stateSensor2, startPositionBack);
  }
}


void readNewSoundValues() {
  int i = 0;
  char str[10];
  
  if (Serial.available()) {
    delay(100); //allows all serial sent to be received together

    while(Serial.available() && i < 20) {
      char nextChar = Serial.read();
      
      if (nextChar == ',') {
        str[i++] = '\0';
        rmsFrontSensor = atoi(str) / 100.0;
        i = 0;
      } else {
        str[i++] = nextChar;
      }
      
    }
    str[i++] = '\0';
    rmsBackSensor = atoi(str) / 100.0;
  }
}


// returns the new state
int updateThermoState(double rms, int state, double lowerLimit, double higherLimit, bool front) {
  if (rms < lowerLimit) { // quiet
    if (state > stateLowerLimit) {  // state is too high
      state -= 2;
    }
  } else if (rms < higherLimit) { // noisy
    if (state < displayLength) {
      state += 3;
    }
  } else {  // loud
      if (state < displayLength) {  // state is too low
        state += 6;
      }
  }

  return state;
}


void updateThermoLed(Adafruit_DotStar &ledStrip, int state, int startPosition) {
  uint32_t color = 0xFFFF00;    // start color
  uint32_t newColor;

  // color stepsize
  uint32_t subtrahend = (0x0000FF / displayLength) + 1;
  subtrahend = subtrahend << 16;
  
  for(int i = 1; i <= displayLength; i++){
    if(state >= i) {    // turn LED on

      newColor = color - subtrahend;
      if (newColor < color) {     // no underflow
        color = newColor;
      }
      ledStrip.setPixelColor(i + startPosition, color);
      
    } else {    // turn LED off
      ledStrip.setPixelColor(i + startPosition, COLOR_BLACK);
    }
  }

  //ledStrip.setBrightness(state * brightnessFactor);
  ledStrip.show();
}


void printValues(double value1, double value2) {
  Serial.print(value1);
  Serial.print(',');
  Serial.println(value2);
}


bool hoch = true;
void testReceivingValues() {
  if (Serial.available()) {
    readNewSoundValues();
    
    Serial.print("Sound Values: ");
    Serial.print(rmsFrontSensor);
    Serial.print(",");
    Serial.println(rmsBackSensor);
    
    for(int i = 1; i <= displayLength; i++){
      if(i < stateSensor1) {    // turn LED on
        strip.setPixelColor(i + startPositionFront, COLOR_RED);
      } else {
        strip.setPixelColor(i + startPositionFront, COLOR_BLACK);
      }
      if(i < stateSensor2) {    // turn LED on
        strip2.setPixelColor(i + startPositionBack, COLOR_RED);
      } else {
        strip2.setPixelColor(i + startPositionBack, COLOR_BLACK);
      }
    }

    if(hoch) {    // turn LED on
      stateSensor1 += 8;
      stateSensor2 += 8;
    } else {
      stateSensor1 -= 8;
      stateSensor2 -= 8;
    }

    strip.show();
    strip2.show();

    if (stateSensor1 > 90){
      hoch = false;
    }
    
    if (stateSensor1 <= 0) {
      hoch = true;
    }
  }
}
```


### Sound Sender

```CPP
// Sensor pins
#define SENSOR_INPUT_FRONT  A0 //sensor nr.: 515
#define SENSOR_INPUT_BACK   A1 //sensor nr.: 510.5

double rmsFrontSensor = 0, rmsBackSensor = 0;


void setup() {
  Serial.begin(9600);   
}

void loop() {
  measureAndCalculateRMS();
  sendValuesAsIntegerPerPrint(rmsFrontSensor, rmsBackSensor);
}


void measureAndCalculateRMS() {
  double sum = 0, sum2 = 0;

  int delayBetweenMeasures = 1;
  int measureCount = 2000;
  
  for(int i = 0; i < measureCount; i++) {
    //sensor 1
    double rawValue = analogRead(SENSOR_INPUT_FRONT) - 500;      //sensor nr.: 515
    sum += rawValue * rawValue;

    //sensor 2
    double rawValue2 = analogRead(SENSOR_INPUT_BACK) - 500;   //sensor nr.: 510.5
    sum2 += rawValue2 * rawValue2;

    delay(delayBetweenMeasures);
  }
  
  rmsFrontSensor = rootMeanSquare(sum, measureCount);
  rmsBackSensor = rootMeanSquare(sum2, measureCount);
}

double rootMeanSquare(double valueSum, int valueCount) {
  return sqrt(valueSum / valueCount);
}


// Print two values in one graph
void sendValuesAsIntegerPerPrint(double value1, double value2) {
  int v1 = value1 * 100;
  int v2 = value2 * 100;
  
  Serial.print(v1);
  Serial.print(',');
  Serial.println(v2);
}
```
