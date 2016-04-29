---
title: "Projekt Wortwecker"
featured: images/wortwecker01.jpg
categories: instructions
layout: post
date:   2016-04-29 15:09:51 +0200
---

Im September war es dann soweit: Dirk, Jens und Thomas fanden sich ein, damit wir gemeinsam 4 Tage und Nächte lang Pizza essen, Cola trinken und basteln konnten.

Unser Ziel war es, dass am Ende jeder der vier Bastler einen fertigen Wortwecker mit nach Hause nimmt - also eine Uhr, welche die aktuelle Zeit in Form von Sätzen anzeigt. Dabei werden die Buchstaben durch einzelne LEDs mit entsprechendem Passepartout dargestellt.

Geplanter Funktionsumfang des Wortweckers:

  * Anzeige der Uhrzeit
  * Automatische Zeitstellung per Funkuhr
  * Helligkeit der Leuchtdioden je nach Umgebungshelligkeit
  * Weck-Zeit einstellbar
  * Weck-Melodie definierbar

![Arbeitsplatz](/images/wortwecker01.jpg)

Insgesamt sind pro Wecker 112 LEDs verbaut, welche alle einzeln angesteuert werden möchten. Da der Arduino natürlich nicht über so viele Ports verfügt, muss noch eine entsprechende Schaltung zwischen Arduino und LEDs eingesetzt werden. Kern dieser Schaltung sind bei unserem Projekt 14 Stück TPIC6C595 Schieberegister pro Uhr. 

![Plan](/images/wortwecker02.jpg)

Da wir nicht nur ein reines Löt- und Bestückungs-Projekt durchführen wollten, entschieden wir uns für die Verwendung von Lochrasterplatinen statt geätzte Platinen zu designen. Eine Wahl, welche wir bei einem „nächsten Mal“ sicher überdenken würden ;-)

## Tag 1

Los ging es am ersten Tag mit der Programmierung des Arduino, wobei dieser Tag eigentlich nur ein halber war, da wir erst am späten Nachmittag begannen und zu diesem Zeitpunkt auch erst zu dritt waren.

Während Dirk und Thomas die LED-auf-Worte-Übersetzung und die Beschickung des Schieberegisters vorbereiteten, konnte ich mich mit dem Auslesen des Funkuhr-Modules befassen.

## Arduino und die Arrays

Offenbar initialisiert ein Arduino Programm ein Byte-Array auf dem Heap mit Nullen, während es auf dem Stack den Speicher bereit stellt wird, jedoch der vorherige Inhalt der betroffenen Speicherzellen unverändert bleibt. Das frühe Testprogramm mit ausschließlich statischem Array funktionierte daher wunderbar. Für den Test der fertigen Platine hingegen waren die identischen Code-Zeilen bereits in Methoden ausgelagert worden und verhielten sich daher anders. Aber wer soll so etwas erahnen? Da liegt es näher, nach Fehlern auf der umfangreich verdrahteten und verlöteten Platine zu suchen... und das dauert dann durchaus mal mehrere Stunden.

```C
for( i = 0; i < 7; i++ )
{
    summe += umsatz[ i ];
    if( hoechsterWert < umsatz[i] )
        hoechsterWert = umsatz[i];
    //
    if( niedrigsterWert > umsatz[i] )
        niedrigsterWert = umsatz[i];
}

printf( "Gesamter Wochengewinn: %f \n", summe );
printf( "Hoechster Umsatz: %f \n", hoechsterWert );
printf( "Niedrigster Umsatz: %f \n", niedrigsterWert );
return 0;
```

## Nummerierte Aufzählung

  1. Erstens
  2. Zweitens
  3. Drittens
