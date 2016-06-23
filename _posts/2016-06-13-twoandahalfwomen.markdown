---
title: "How To Build The Qube"
categories: instructions
layout: post
date:   2016-04-29 15:09:51 +0200
---

## Ziel/POV:
Ziel unseres Projektes ist es Studenten bzw. Interessenten für die Informatik und die Hochschule Mannheim zu begeistern und den Kommunikationsaustausch zu fördern. Ausserdem soll mit Hilfe dieses Projektes einefreundlichere Atmosphäre geschaffen werden, damit sich Studierende gerne in der Fakultät für Informatik aufhalten und w. 

## Projektbeschreibung:
Qube der Würfel der Wissen schafft. Unser Projekt umfasst ein Quiz, das mit Hilfe eines Raspberry Pi und einem Arduino realisiert wurde. Das Projekt ist in der Form eines Würfels dargestellt, an welchem die verwendeten Bauteile angebracht sind. Den Spielern ist es möglich einen Einspieler- oder auch Zweispielermodus zu wählen. Die Steuerung bzw. Navigation des Quiz ist mithilfe der am Würfel angebrachten Buttons möglich.

Die Seuerung der grafischen Oberfläche sowie die dahinterliegende Logik übernimmt ein Raspberry Pi 3. Der LED Streifen der den Würfel nochmals aufwertet wird mit einem Arduino Uno gesteuert. Dieser wird wiederum über den Raspberry Pi angesprochen.

Dieses Projekt wurde auch mit einem Raspberry Pi 2 Revision B erfolgreich getestet wir empfehlen aber dennoch ein Raspberry Pi 3 zu verwenden da dieser bereits mit WLAN und Bluetooth ausgestattet ist und sich somit steuern lässt ohne eine USB Maus oder Tastatur zu verwenden bzw. der Einsatz von zusätzlichen WLAN- Bluetooth-Donglen entfällt.

## Verwendete Materialien und Werkzeuge:

### Materialien:
  - 4x Plexiglas (24,75cm x 24,75cm x 0,4cm) | ca. 12€
  - 4x Plexiglas (25,25cm x 25,25cm x 0,4cm) | ca. 5€
  - 1 x Plexiglas (24,05cm x 25,25cm x 0,04cm) | ca. 2€
  - Milchglasfolie (gibt es im Bauhaus von d-c-fix) | ca. 6€
  - 1x MDF Platte schwarz (27cm x 30cm x 0,19cm) | ca. 3€
  - 1x Raspberry Pi 3 | [Gibt es hier zu kaufen](https://www.amazon.de/Raspberry-Pi-3-Model-B/dp/B01CEFWQFA)
  - 1x Mini USB-Kabel Ladegerät für Raspberry Pi 3 Stromversorgung | [Gibt es hier zu kaufen](https://www.amazon.de/Raspberry-Pi-Micro-USB-Netzteil/dp/B00SVALHXU)
  - 1x USB oder Bluetooth Maus für den Raspberry Pi 3
  - 1x USB oder Bluetooth Tastatur für den Raspberry Pi 3
  - 1x Arduino Uno | [Gibt es hier zu kaufen](https://www.amazon.de/Arduino-Uno-Rev-3-Mikrocontroller-Board/dp/B008GRTSV6/ref=sr_1_1?ie=UTF8&qid=1466531263&sr=8-1&keywords=Arduino+uno)
  - 1x Netzteil für Arduino Uno - Goobay 2798 - Universal Netzgerät 3-12 V | [Gibt es hier zu kaufen](https://www.amazon.de/Goobay-2798-Universal-Netzgerät-3-12/dp/B0038WU2Z0)
  - 1x Laptop/PC um den Arduino zu programmieren
  - 2 x Push Dome Buttons blau | [Gibt es hier zu kaufen](https://www.amazon.de/Big-Dome-Push-Button-Blue/dp/B008FZJ2WE)
  - 5 x Einbautaster 35mm(blau, gelb, rot, grün, schwarz) | [Gibt es hier zu kaufen](http://www.watterott.com/index.php?page=search&page_action=query&desc=on&sdesc=on&keywords=Einbautaster&x=0&y=0)
  - 2x Black IL Concave Arcade Start Button ("One Player" und "Two Player") | [Gibt es hier zu kaufen](http://www.arcadeworlduk.com/products/Black-IL-Concave-Arcade-Start-Button.html)
  - Kabel
  - Insulated Daisy Chain Harness with 32 Crimp Connections [dt. Isolierter verketteter Kabelstrang mit 32 Crimpverbindungen] | [Gibt es hier zu kaufen](http://www.arcadeworlduk.com/products/insulated-daisy-chain-harness-with-32-crimp-connections.html)
  - Verbindungskabel RB-CB3-25 (die Pins sind da schon dabei)| [Gibt es hier zu kaufen](https://www.conrad.de/de/raspberry-pi-verbindungskabel-rb-cb3-25-1182193.html)
  - Pins (Male) für Verbindungskabel
  - Kabelhülsen
  - Isolierband
  - 1x Universalzylinderschloss | [Gibt es hier zu kaufen](https://www.bauundhobby.ch/maschinen-%2B-werkstatt/sicherheit/schlösser-%2B-zylinder/univ.zylinderschloss-zs-77-sb/C041202/P3191726/de)
  - 1x 19 Zoll Monitor
  - 1x Adapterkabel HDMI auf DVI | [Gibt es hier zu kaufen](https://www.amazon.de/AmazonBasics-Adapterkabel-HDMI-auf-DVI-Schwarz/dp/B00NH11X64)
  - 2x Acryl Scharniere 64mm | [Gibt es hier zu kaufen](https://www.amazon.de/gp/product/B00R0BCWNU/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1)
  - Tesa Power Strips Small | [Gibt es hier zu kaufen](https://www.amazon.de/tesa-Powerstrips-Strips-SMALL-Packung/dp/B000KJR2ES/)
  - Tesa Powerbond | [Gibt es hier zu kaufen](https://www.amazon.de/tesa-doppelseitiges-Montageband-Powerbond-TRANSPARENT/dp/B001BVR8XE/ref=pd_sim_60_3?ie=UTF8&dpID=51gaFg9WxNL&dpSrc=sims&preST=_AC_UL160_SR147%2C160_&psc=1&refRID=21V96PHT0CDHP76F9ZMY)
  - Neopixel 1 Meter | [Gibt es hier zu kaufen](https://www.adafruit.com/product/1460)
  - 5x Kabelbinder
  - Pattex Kraftkleber transparent | [Gibt es hier zu kaufen](https://www.amazon.de/Pattex-PXT2C-Kraftkleber-125-transparent/dp/B0000WPL70)

### Werkzeuge:
  - Lötkolben
  - Dremel
  - Aufsatz Dremel Schleifscheibe/Trennscheibe
  - Aufsatz Dremel Minikreissägeblatt
  - Standbohrmaschine
  - Lochsäge Ø25mm
  - 6er Bohrer  
  - Forstner Bohrer Ø6mm für Zylinderschloss
  - Schere
  - Abisolierzange
  - Cutter Messer
  - Geodreieck
  - Kugelschreiber
  - Feuerzeug / Heißluftfön
  - Multimeter

## Step-by-Step Guide - Arcade Buttons & Push Dome Buttons

### Step 1: Kabel an Switchcontroller der Arcade Buttons und Push Dome Buttons löten
Für diesen Schritt benötigen wir: Abisolierzange, Lötkolben, Kabelhülse, Kabel, Feuerzeug, Schere

Damit die Arcade Buttons verwendet werden können, müssen an den Switch Coontrollern der Arcade Buttons und der Push Dome Buttons Kabel angebracht werden. So, dass diese zu einem späteren Zeitpunkt an die GPIO-PINS des Raspberry PI angeschlossen werden können.

Dazu haben wir in unserem Projekt die folgende Vorgehensweise für alle 7 Arcade Buttons und die 2 Push Dome Buttons genutzt:
  1. Schneide dir ein Kabel in ausreichender Länge von ca. 25cm  zurecht, da beim verbauen ein Stück der Länge verloren geht. Am besten du nimmst Kabel in den Farben der Arcade Buttons und Push Dome Buttons, um diese besser zu unterscheiden.
  2. Isoliere jeweils beide Kabelenden mit einer Abisolierzange ab.
  
  ![Kabel](/images/taahw/01.jpg)

  3. Als nächstes nimmst du eines der Kabelenden und lötest dies mit Hilfe des Lötkolben an den Microswitchcontroller eines Buttons/Buzzers.

  ![Kabel_Button](/images/taahw/02.jpg)

  4. Nun musst du das verlötete Kabel mit einer Kabelhülse oder einem Isolierband am Switchcontroller isolieren.
  
  ![Kabelhülse](/images/taahw/03.jpg)

  5. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt. 
  
  ![Kabelhülse](/images/taahw/04.jpg)
  
Dieses Vorgehen wurde für alle Arcade Buttons und Push Dome Buttons dieses Projektes angewandt.

### Step 2: Kabel der Arcade Buttons und Push Dome Buttons verlängern
Um Step 2 durchzuführen benötigen wir: Schere, Abisolierzange, Lötkolben, Kabelhülse, Verbindungskabel RB-CB3-25, Feuerzeug

Das in Step 1 verlötete Kabel solltest du noch mit einem Verbindungskabel RB-CB3-25 erweitern. Dieser Schritt ist notwendig, damit du die Arcade Buttons und Push Dome Buttons an die GPIO-PINS des Raspberry PI anschließen kannst.

Hierzu haben wir uns im Rahmen des Projektes für nachfolgende Vorgehensweise entschieden:
  1. Nehmt das Verbindungskabel RB-CB3-25 und schneidet es an gewünschter Stelle ab, so das noch eine ausreichende Länge zum verlöten vorhanden ist.
  2. Danach solltest du an der abgeschnittenen Seite mit einer Abisolierzange die Kabelstränge freilegen.

  ![Verbindungskabel](/images/taahw/05.JPG)

  3. Nun nimmst du einen Arcade Button oder Push Dome Button, an dem Step 1 bereits durchgeführt wurde und verbinde die jeweiligen abisolierten Kabelenden mit Hilfe des Lötkolbens.

  ![Verbindung](/images/taahw/06.jpg)  

  4. Danach solltest du die Kabelhülse über das Ende des Verbindungskabel (Female) bis zur Lötstelle ziehen.
  
  ![Kabelhülse](/images/taahw/07.jpg)

  5. Nun solltet du die Lötstelle mit der überzogenen Kabelhülse oder einem Isolierband isolieren.
  6. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.
  
  ![Verbindungskabel](/images/taahw/08.jpg)

Auch dieses Vorgehen wurde für alle Arcade Buttons und Push Dome Buttons dieses Projektes angewandt.

### Step 3: Kabel an die LED der Push Dome Buttons anbringen
Benötigte Materialien: Schere, Abisolierzange, Lötkolben, Kabel, Kabelhülse, Feuerzeug

Für die LED der Push Dome Buttons werden ähnliche Schritte wie in Step 1 durchgeführt. Auch hier ist es ratsam verschiedenfarbige Kabel wie z.B. blau und rot wie in unserem Projekt zu verwenden, um - und + zu unterscheiden.

Im Gegensatz zu einer "normalen LED" sind bei diesen LED's die Beinchen nicht verschieden lang um so + und - zu unterscheiden.
Um die Kabel am richtigen Beinchen anzulöten benötigst du einen Multimeter mit dem du Heraus finden kannst welches Beinchen + oder - ist. Weitere Einzelheiten findest du [hier](http://www.ledhilfe.de/viewtopic.php?f=23&t=1223).
Falls du kein Multimeter zur Hand hast musst du einfach ausprobieren :-) 

Hierfür gehst du wie folgt vor:
  1. Schneide dir zwei Kabel in ausreichender Länge von ca. 25cm zurecht, da beim verbauen ein Stück der Länge verloren geht. Du solltest hierfür ein blaues und ein rotes Kabel zur besseren Unterscheidung benutzen.
  2. Isoliere jeweils beide Kabelenden des blauen und roten Kabels mit einer Abisolierzange ab.
  3. Als nächstes nimmst du das Kabelende des blauen Kabel und lötest dies mit Hilfe des Lötkolben an den Minuspol an.
  4. Nun nimmst du eines der Kabelenden des roten Kabel und lötest dies an die gegenüberliegende Seite an. 
  4. Nun musst du die verlöteten Kabel mit einer Kabelhülse oder einem Isolierband am Minus- und Pluspol isolieren.
  5. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.
  
![Push Dome Button](/images/taahw/09.jpg)

### Step 4: Micro Switches der Arcade Buttons und Push Dome Buttons mit dem Insulated Daisy Chain Kabelstrang verbinden
Benötigt werden: Insulated Daisy Chain Kabelstrang, Schere, Alle Buttons

Mit Hilfe des Crimp Kabelstrangs werden die einzelnen Micro Switches der Buttons und der Buzzer verbunden. Folgendes Bild zeigt den Aufbau eines Micro Switches.

![Aufbau Micro Switch](/images/taahw/cherry.gif)

Hierfür werden 10 Steckverbindungen des Crimp Kabelstrangs benötigt. Die Reihenfolge der Anschlüße spielt hierbei keine Rolle.

![Kabelstrang](/images/taahw/10.jpg)

In unserem Projekt haben wir die Verbindungen zwischen den Komponenten in der Reihenfolge
  - Arcade Button rot
  - Arcade Button grün
  - Arcade Button gelb
  - Arcade Button blau
  - Push Dome Button 2
  - Push Dome Button 1
  - Arcade Button (1 Player)
  - Arcade Button (2 Player)
  - Arcade Button schwarz

gewählt.

Dazu gehen wir folgendermaßen vor:
  1. Als erstes nimmst du den ersten Crimp Stecker des Kabelstrangs und befestigt diesen an dem COMMON (der Untere) Anschluss des Micro Switches des roten Arcade Buttons. Die Verbindung zum Microswitch sollte jetzt so aussehen wie auf dem folgenden Bild 
  
  ![Verbindungskabel](/images/taahw/11.jpg)

  2. Danach widerholst du Schritt eins bis alle Switches miteinander verbunden sind.
  6. Nach der letzten Verbindung - in unserem Fall der Arcade Button schwarz - musst du das Kabel mit einer Schere trennen, um das Kabel im nächsten Schritt zu verlängern. Dieses Kabel wird am Ende an den GROUND Pin des Raspberry's angeschlossen.

### Step 5: Insulated Daisy Chain Harness verlängern
Wir benötigen: Verbindungskabel RB-CB3-25, Schere, Kabelhülse, Lötkolbe, Kabelstrang

Wie schon erwähnt verbinden wir nun das Ende des Kabelstrangs mit einem Verbindungskabel RB-CB3-25, damit dieses an den GROUND Pin des Raspberry's angeschlossen werden kann. 

Hierfür führt ihr folgende Steps aus:
  1. Den zehnten Crimp Stecker trennen wir nun ebenfalls mit einer Schere.
  
![Verbindungskabel](/images/taahw/12.jpg)

  2. Danach solltet ihr das Kabelende mit einer Abisolierzange abisolieren.

![Verbindungskabel](/images/taahw/13.jpg)  

  3. Nun nimmst du das Verbindungskabel RB-CB3-25, welches die gleiche Farbe wie der Kabelstrang haben sollte, zur Hand und schneidest eines der Female Stücke ab, sodass das Kabel ausreichend lang ist.
  
![Verbindungskabel](/images/taahw/05.JPG)

  4. Auch dieses Kabel musst du am abgeschnittenen Ende abisolieren.
  5. Als nächstes verlötest du das Ende des Crimp Kabelstrangs mit dem zuvor isolierten Verbindungskabel.
  6. Nun musst du die verlöteten Kabel mit einer Kabelhülse oder einem Isolierband isolieren.
  ![Verbindungskabel](/images/taahw/07.jpg)
  7. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.
  ![Verbindungskabel](/images/taahw/08.jpg)

### Step 6: Arcade Buttons und Push Dome Buttons mit GPIO von Raspberry Pi 3 verbinden

In diesem Schritt werden wir die angebrachten Verbindungskabel an die GPIO Pins des Raspberry Pi 3 anschließen.
Im Gegensatz zu dem Arduino Uno sind die Pins des Raspberry's nicht beschriftet um denoch den Überblick zu behalten ist es ratsam folgende Abbildung zur Hilfe zu nehmen:

![GPIO](/images/taahw/14.png)

> :warning:
Um die Pins korrekt lesen bzw. zuordnen zu können, sollten sich die GPIO Pins des Raspberry's auf der rechten Seite befinden wenn er vor dir liegt. Siehe nächstes Bild.

![korrekte Ausrichtung des Raspberry Pi um die GPIO Pins anzubringen](/images/taahw/rpi_ausrichtung.jpeg)

Arcade Button Blau: PIN 22

Arcade Button Gelb: PIN 29

Arcade Button Grün: PIN 16

Arcade Button Rot: PIN 18

Arcade Button Schwarz: PIN 13

Arcade Button Player 1: PIN 12

Arcade Button Player 2: PIN 11

Push Dome Button 1: PIN 15

Push Dome Button 2: PIN 31

Auch das Kabelende des oben verwendeten Kabelstrangs aus Step 5 solltest du an einen GPIO Pin anschließen, so benötigst du kein Breadboard und habt später mehr Platz im Würfel.

Button mit Kabelstrang-Ende: PIN 6 (GROUND)

![GPIO](/images/taahw/16.jpg)

Für einen besseren Überblick hier nochmal das ganze Szenario als Fritzing Schaltplan:

![Raspberry Pi Fritzing](/images/taahw/qube_raspberry_Steckplatine.jpg)

### Step 7: Push Dome Button LED an Arduino anschließen
Hierfür benötigen wir: Push Dome Button LED, Arduino, Pins (Male)

Vorgehensweise:
  1. Damit die Kabel der LED von Push Dome Button 2 an den Arduino angeschlossen werden können, musst du auf die Kabelenden der LED jeweil ein Pin (Male) stecken, da der Arduino im Gegensatz zum Raspberry weibliche Anschlüsse besitzt.
  
![LED Push Dome Button](/images/taahw/17.jpg)

  2. Das blaue Kabel wird an GND angeschlossen.
  3. Das rote solltet ihr an Pin 13 anschließen
  4. Für den Push Dome Button 1 verfahrt ihr ebenso, jedoch unterscheidet sich hier die Pin Belegung
  5. Blaues Kabel an GND anschließen
  6. Rotes Kabel an Pin 12 anschließen
  
Für einen besseren Überblick hier nochmal das ganze Szenario als Fritzing Schaltplan:

![Arduino Uno Fritzing](/images/taahw/qube_arduino_Steckplatine.jpg)


### Step 8: Kabel an Neopixelstreifen löten
Hierfür benötigt ihr folgendes: Lötkolben, Abisolierzange, Neopixelstreifen, Isolierband

Der Neopixelstreifen hat sowohl Input als auch Output. In unserem Projekt benötigen wir die Input Seite. Dort werden drei verschiedenfarbige Kabel angeschlossen, in unserem Projekt haben wir die Farben 
  - rot = 5V 
  - gelb = Dh (Mitte) 
  - grau = GND 
verwendet.

!Neopixel(/images/taahw/led_streifen/ada.jpg)

Hinweis: Die Kabel bzw. der Lötzinn sollte sich untereinander nicht berühren, da der Neopixelstreifen sonst nicht funktionieren wird.

Die folgenden Schritte solltet ihr dabei beachten:
  1. Als erstes benötisgt du 3 Kabel in den Farben rot, gelb und grau (Im Normalfall werden rot, weiß und schwarz verwendet). Die Kabel sollten eine Länge von ca. 15cm haben.
  2. An allen drei Kabeln solltest du beide Kabelenden mit einer Abisolierzange absisolieren.
  2. Nachdem du die Kabel abisoliert hast, nimmst du nun das rote Kabel und lötet dies an den Punkt des Neopixelstreifen welcher mit 5V markiert ist an. 
  3. Das selbe machst du mit dem grauen Kabel. Dies sollte allerdings an den Punkt, welcher mit GND markiert ist, gelötet werden.
  4. Auch mit dem gelben Kabel verfahrst du wieder so. Hierbei musst du auch auf den korrekten Punkt, welcher Dh ist, achten.
  
![Neopixel](/images/taahw/19.jpg)

  5. Als letztes solltest du die gelöteten Stelle mit einem Isolierband isolieren.
  
![Neopixel](/images/taahw/20.jpg)

### Step 9: Verbindungskabel RB-CB3-25 an Kabel von Neopixelstreifen löten
Bnötigt werden: Verbindungskabel, Schere, Kabelhülse, Lötkolben, Feuerzeug

Auch der Neopixelstreifen benötigt eine Verlängerung mit den Verbindungskabeln, um diese später an die PINS des Raspberry bzw. Arduino anschließen zu können. Es werden drei Verbindungskabel benötigt, diese solltet ihr nach den entsprechenden Farben (weiß, schwarz, rot) wählen.

Die Vorgehensweise lautet wie folgt:
  1. Zu Beginn nimmst du das Verbindungskabel RB-CB3-25 in der Farbe weiß und schneiden es an gewünschter Stelle ab, so das noch eine ausreichende Länge zum verlöten vorhanden ist.
  2. Danach solltest du es an der abgeschnittenen Seite mit einer Abisolierzange abisolieren.
  3. Nun nimmst du das weiße Kabel welches in Step 7 an den Neopixelstreifen gelötet wurde und verbindest die jeweiligen abisolierten Kabelenden mit Hilfe des Lötkolben.
  4. Danach solltest du die Kabelhülse über das Ende des Verbindungskabel bis zur Lötstelle ziehen. 
  5. Nun isolierst du die Lötstelle mit der überzogenen Kabelhülse.
  6. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.

### Step 10: Neopixelstreifen mit Arduino verbinden
Benötigte Materialien: Neopixel LED Streifen, Arduino Uno

Hinweis: Im Gegensatz zum Raspberry sind die Pins des Arduinos auf dessen Platine beschrieben.

grau (GND): PIN GND
gelb (Dh): PIN 6
rot (5V): PIN 5V

Vorgehensweise:
  1. Das graue Kabel an den GROUND Pin des Arduinos anschließen
  2. Das rote Kabel schließt du an den 5V Pin des Arduinos an. 
  3. Das letzte Verbindungskabel (gelb) kommt an PIN Nummer 6 des Arduinos.

### Step 11: Arduino und Raspberry verbinden

Benötigte Materialien: Raspberry Pi 3, Arduino Uno, USB Kabel

Die Verbindung zwischen Arduino und Raspberry stellt ihr mittels USB-Kabel her. Im Regelfall ist dieses Verbindungskabel im Lieferumfang des Arduinos enthalten.

![Verbindung zwischen Raspberry Pi und Arduino Uno](/images/taahw/21.jpeg)

### Step 12: Raspberry und Monitor verbinden
Benötigte Materialien: Monitor, Raspberry Pi 3, HDMI Kabel oder -Adapter

Um die Grafische Oberfläche an einem Monitor anzeigen zu lassen, muss ein Monitor an den Raspberry angeschlossen werden. Dies geschieht entweder direkt über ein HDMI Kabel oder mit einem entsprechenden Adapter.

## Step-by-Step Guide - Würfel

### Step 1: Löcher für die Buttons und Buzzer bohren

Benötigte Materialien:
1. Oberplatte (24,75 x 24,75cm)
2. Vorderplatte (25,25 x 25,25cm)
2. Lochfräse
3. 6er Bohrer zum vorbohren
4. Dremel
5. Standbohrer

Damit die Bauteile an den Plexiglasscheiben angebracht werden können müssen zunächst Löcher an den Scheiben gebohrt werden.

Auf der oberen Platte müssen vier Löcher für die farbigen Buttons und zwei Löcher für die Buzzer gebohrt werden mit jeweils einem Durchmesser von 28mm bzw. 24mm.

Die Anordnung der Löcher siehst du auf der Abbildung "fertige Oberplatte".

Um die Löcher zu bohren wird zuerst ein Loch mit dem kleinen Bohrer vorgebohrt bevor dann mit der Lochfräse (25mm) die Löcher gebohrt werden können.

![Lochfräse](/images/taahw/bohrer/lochfraese.jpg)

Am besten spannt man die Lochfräse in einen Standbohrer, um mehr Stabilität zu bekommen und damit ein sauberes rundes Loch entsteht.

![Standbohrer](/images/taahw/bohrer/stand.jpg)

Beim Bohren darf nicht mit zu hohen Umdrehungen gebohrt werden, da ansonsten die Platten zu schmelzen beginnen. Dies erkennt man an einem immer stärker werdenden beißenden Geruch.

Da das Schmelzen nicht komplett verhindert werden kann müssen die Löcher bzw. die Schmelzrückstände an den Löchern mit einem Dremel weggeschliffen werden.

Da die 25mm für die farbigen Buttons zu klein sind muss mit einem Dremel mit passendem Schleifaufsatz nach geholfen werden, damit die Buttons passen.

Im Falle der Buzzer müssen die Löcher nur noch von den Schmelzrückständen entfernt werden und dann passen die Buzzer in die Löcher.
Die Buzzer sitzen sehr locker in den gebohrten Löcher aber das ist nicht weiter schlimm da die Buzzer zusätzlich befestigt werden können.

Wenn du mit den Löchern fertig bist sollte das Ergebnis ungefähr so aussehen.

![fertige Oberplatte](/images/taahw/wuerfel/platte_oben.jpeg)

Den Schlitz den du hier siehst wird im nächsten Schritt angebracht

Auf der Vorderseite (die zukünftige Vorderseite des Würfeln) müssen noch drei weitere Löcher angebracht werden. Zwei Löcher für jeweils den Ein - und Zweispielerbutton sowie ein Loch für den Navigationsbutton.
Dabei haben wir das Loch für den Aracde Button schwarz rechts außen und das Loch für den Ein Spieler Button links außen angebracht. Jeweils mit einem Abstand von 3cm zur äußeren Plattenkante. Rechts neben dem Ein Spieler Button befindet sich das Loch für den Zwei Spieler Button (mit einem Absatnd von 2-3cm von Loch für den Arcade Button schwarz.)

Um die Löcher zu bohren und zu schleifen musst du genauso vorgehen wie zuvor auch.

Das fertige Ergebnis sieht dann so aus:

![fertige Oberplatte](/images/taahw/wuerfel/platte_vorne.jpeg)

### Step 2: Loch und Schlitz für das Zylinderschloss bohren

Benötigte Materialien:
1. Rückplatte (24,05cm x 25,25cm x 0,04cm)
2. Dremel mit Mini Sägen Aufsatz
3. 6er Bohrer zum vorbohren

Um die Sicherheit des Qubes zu erhöhen bzw. zu verhindern, dass nichts geklaut wird ist es sinnvoll noch zusätzlich ein Schloss anzubringen. Zusätzlich zu diesem Schloss werden noch Scharniere an die Rückplatte angebracht damit sich diese leicht öffnen lässt.
Diese Scharniere werden mit Pattex Kraftkleber an der Bodenplatte angebracht. Das ankleben der Scharniere wird erst in Schritt Step 6 erfolgen sollte aber an dieser Stelle schonmal erwähnt werden.

Um das Loch für das Schloss zu bohren wird zuerst die Mitte der Platte festgelegt und mit einem Abstand zur oberen Kante von 2cm eine Markierung gesetzt. Mit Hilfe dieser Markierung wird zuerst wieder ein Loch vorgebohrt bevor dann mit dem Forstner Bohrer das Loch gebohrt werden kann.

Um den Schließmechanismus des Schlosses zu vervollständigen muss zusätzlich ein Schlitz an der Oberseite des Würfels (Step 1) eingefräst werden. Der Schlitz muss 4cm lang sein und 1,5 cm von der Unterkante der Oberplatte entfernt sein. Falls du ein anderen Schloss als das angegebene gekauft hast sollten die Mase dementsprechend angepasst werden damit das Schloss ordnungsgemäß schließt. 

Um den Schlitz zu fräsen nimmst du einen speziellen Mini Kreissägen Aufsatz für den Dremel. In dem nachfolgenden Bild wird die Mini Säge dargestellt.

![Mini Kreissäge für den Dremel](/images/taahw/dremel/minisaege.jpg)

### Step 3: Aussparung für Raspberry und Arduino sägen

Benötigte Materialien:
1. Rückplatte (24,05cm x 25,25cm x 0,04cm)
3. Schleife
4. Dremel mit Mini Kreissägen Aufsatz

Damit der HDMI Eingang sowie die Eingänge für die Netzteile für das Raspberry und den Arduino zugänglich sind muss am unteren Ende der Rückplatte eine Aussparung gefräst werden.

Neben der Aussparung für die Kabel muss rechts und links noch Platz gelassen werden für die Scharniere damit die Rückwand geöffnet werden kann.
Die Aussparung hat eine Breite von 6cm und eine Höhe von 2cm und sitzt in der Mitte der Rückplatte. Dies passt genau um direkt dahinter den Raspberry anzubringen und damit ein wenig Luft bleibt für die externe Stromzufuhr des Arduinos.

Nachfolgende Abbildung zeigt den Sitz der Aussparung.
Die äußeren beiden Linien sind markieren jeweils den Anfang der zwei Scharniere die in Step 6 befestigt werden und das dazwischen mittig liegende "Gerät" ist der Raspberry. Die Ausparrung beginnt ca. 10mm entfernt von dem linken Scharnier.

![Ausparung](/images/taahw/wuerfel/platte_hinten.jpeg)

Das fräsen der Ausparung erfolgt wieder mit dem Dremel und dem Mini Kreissägen Aufsatz der für den Schlitz für das Schloss verwendet wurde.

Das folgende Bild zeigt die Aussparung und das dahinter liegende Gehäuse des Raspberry Pi's.

![Ausparung](/images/taahw/wuerfel/schlitz_II.jpeg)

### Step 4: Milchglasfolie anbringen

Benötigte Materialien:
1. Milchglasfolie
2. Oberplatte, Rückplatte und Vorderplatte des Würfels
3. Klebefolien Befestigungsset
4. Cutter Messer

Uns war es wichtig, dass Nutzer des Qubes in den Würfel hinein blicken konnten und so die Elektronik sehen können. Deswegen haben wir uns dafür entschieden nur die zwei Seitenplatten sowie die Oberplatte mit Michglasfolie zu bekleben.

Damit der spätere Lichteffekt des LED Streifens besser zur Geltung kommt kann aber auch der komplette Würfel mit Folie beklebt werden.

Um die Milchglasfolie auf die Platten anzubringen ist es das einfachste wenn die Klebeseite der Milchglasfolie zuerst freigelegt und dann die Folie mit der Klebeseite nach oben flach auf einem Tisch ausgebreitet wird. Nun kannst du eine Platte mit der Rückseite auf die Klebefolie legen und dann die Klebefolie entlang der Kanten abschneiden.
Danach musst du die Klebefolie sofort mit dem Schaber des Klebefolien Befestigungssets glatt streichen, um die restlichen Luftblässchen zu entfernen. Sollten nach ein paar Stunden weiter Bläschen entstehen so kannst du die mit einer Nadel einstechen und mit dem Schaber glattstreichen.

Da du jetzt alle gebohrten Löcher mit der Klebefolie verdeckt hast hast, musst du nun die Löcher wieder ausschneiden. Dies funktioniert am besten mit einem Cutter Messer.

Dazu die Platte auf den "Kopf" legen und an den Lochkanten entlang die Löcher ausschneiden.

![Ausparung](/images/taahw/wuerfel/folie_schneiden.jpeg)

### Step 5: Plexiglasscheiben miteinander verkleben

Benötigte Materialien:
1. Alle Plexiglas Platten (außer die für die Rückwand da die zur Klapptür umgebaut wird)
2. Pattex Kraftkleber
3. alter Pinsel
4. Cutter Messer
5. Behälter für den Kleber
6. großes Geodreieck

Wenn alle Platten gebohrt und mit Milchlasfolie versehen wurden kann nun das Zusammenkleben der Platten erfolgen.

Damit der Würfel auch wirklich quadratisch wird müssen die vier kleinen Platten (24,75 x 24,75cm) in einer ganz bestimmten Anordnung miteinander verklebt werden.

Dies ist auf nachfolgender Zeichnung zu erkennen. Hinweis: Die Zeichnung zeigt den Würfel von HINTEN.

![Querschnitt der Platten des Würfels](/images/taahw/wuerfel/reihenfolge.jpeg)

Damit die Platten bestmöglichst aufeinander kleben empfiehlt es sich auf der vorgesehenen Klebefläche (4mm breit) die zuvor angebrachte Michglasfolie zu entfernen. Das machst du am indem man die Folie vorsichtig mit dem Cutter Messer einschneidet (sodass die Platte nicht beschädigt wird) und dann abziehst.

Wenn du das erledigt hast kann wirklich mit dem Bekleben begonnen werden.

Zum Bekleben fülle ein biscchen von dem Patex Kraftkleber in ein Behälter. Jetzt kannst du mit Hilfe des alten Pinsels den Kleber auf die Klebefläche aufbringen. Wichtig ist, dass nicht nur eine Seite sondern beide Seiten die verklebt werden sollen mit dem Kleber versehen werden. Anschließend kannst du den Kleber leicht antrocknen lassen und stark zusammenpressen.

![Platten kleben](/images/taahw/wuerfel/kleber_anbringen.jpeg)

Damit die inneren Winkel auch hundertprozentig rechtwinklig werden kann ein Geodreieck, zur Unterstützung, zwischen die Platten gelegt werden. 

![Geodreieck zur Ermittlung eines rechten Winkels](/images/taahw/wuerfel/geodreieck.jpeg)

Sobald die ersten Vier Platten verklebt worden sind wird zum Schluss die Vorderplatte (die mit den drei Löcher) angeklebt.
Es hat sich Bewährt, dass den Kleber ein paar Stunden trocknen lässt bevor die Frontplatte aufgeklebt wird. 

### Step 6: Scharniere an Holzplatte/Plexiglas verkleben
Benötigte Materialien: Scharniere, Pattex Kraftkleber, hintere Seite Plexiglas, MDF Platte

Vorgehensweise:
  1. Als erstes solltet ihr euch eine kleine Markierung jeweils rechts und links an der unteren Seite des Plexiglases machen, damit ihr ungefähr wisst wo es anzubringen ist.
  2. Den selben Schritt führt ihr auch auf der hinteren Seite des Würfels durch, da diese zwei Seiten miteinander verbunden werden
  3. Danach verteilt ihr den Kleber auf einer Seite eines Scharnieres und drückt dieses nun fest an die untere Seite des Würfels.
  3. Nun solltet ihr das Scharnier eine Weile trocknen lassen bis es fest ist.
  4. Schritt 3 wiederholt ihr für die hintere Seite des Würfels und lasst das Scharnier ebenfalls trocknen.
  5. Die Schritte 1-4 sind auch für das zweite Scharnier durchzuführen.

### Step 7: Arcade Buttons und Push Dome Buttons anbringen

Um die Buttons und Buzzer anzubringen musst du diese in Ihre Einzelteile zerlegen (wenn das noch nicht der Fall ist).
Das heißt den Micro Switch und den Befestigungsring von den Buttons/Buzzer trennen.

Dann kannst du ein Buttons in das dafür vorgesehende Loch stecken bzw. drehen und von unten innen mit dem Befestigungsring befestigen. Nachdem der Button fest sitzt wird zum Schluss der Micro Switch angebracht. Das erfolgreiche Anbringen der Micro Switches kannst du testen indem du auf den Button drückst und ein deutliches Klicken zu hören ist. 

Dies wiederholst du nun so lange bis alle Buttons angeschlossen sind.

Das Befestigen der Buzzer funktioniert nach dem gleichen Prinzip.

Das fertige Ergebis sollte dann so aussehen:
 ![angebrachte Buttons auf der Operplatte](/images/taahw/wuerfel_komplett.jpeg)
 ![angebrachte Buttons auf der Vorderplatte](/images/taahw/wuerfel_komplett_II.jpeg)
 
### Step 8: Zylinderschloss befestigen
Benötigte Materialien: Zylinderschloss, hintere Plexiglasscheibe

Vorgehensweise:
  1. Zuerst nimmst du das Zylinderschloss zur Hand und schraubt dieses auf, sodass du es an der hinteren Plexiglasseite einsetzen kannst.
  2. Als nächstes setzt du das Zylinderschloss ein und schraubst es fest.
  3. Nun richtest du es so aus, dass der Würfel mit der oberen Seite abschließbar ist.

 ![Zylinderschloss](/images/taahw/22.jpeg)

### Step 9: Würfel an Holzplatte kleben
Benötigte Materialien:
1. Würfel
2. MDF Platte
3. Kleber
4. Bleistift
5. Geodreieck
6. Pinsel

Vorgehensweise:
  1. Als erstes nimmst du die MDF Platte zur Hand und markierst, wo du den Würfel anbringen möchtest.
  2. Dazu zeichnest du ein Quadrat mit den entsprechenden Maßen.
  3. Nun verteilst du den Kleber mit einem Pinsel in dem eben gezeichneten Quadrat.
  4. Kurz antrocknen lasse.
  5. Als nächstes nimmst du den Würfel und drückt diesen auf die MDF Platte.
  6. Zum Schluß solltest du ihn eine Weile trocknen lassen, so das die Bauteile fest miteinander verbunden sind.

![Würfel mit MDF Platte](images/taahw/wuerfel_komplett_mdf.jpeg)

### Step 10: Raspberry an Würfel anbringen
Benötigte Materialien:
1. Raspberry mit Gehäuse
2. Würfel
3. Tesa Powerbond
4. Schere

Vorgehensweise:
  1. Als erstes schneidest du dir zwei Streifen Tesa Powerstrips zurecht.
  2. Diese klebst du jeweils rechts und links an die Unterseite des Raspberry Gehäuse.
  3. Entferne nun das Schutzpapier und drücke das Gehäuse an den Boden des Würfels.
  4. Hierbei solltest du darauf achten, dass in der Aussparrung der hinterseite des Würfels genug Platz für das Stromkabel des Arduinos vorhanden ist.
  
![Aussparrung](/images/taahw/23.jpeg)

### Step 11: Arduino an Würfel anbringen
Benötigte Materialien:
1. Arduino mit Gehäuse
2. Würfel
3. Tesa Powerbond
4. Schere

Vorgehensweise:
  1. Als erstes schneidest du dir zwei Streifen Tesa Powerstrips zurecht.
  2. Diese klebst du jeweils rechts und links an die Unterseite des Arduino Gehäuse.
  3. Entferne nun das Schutzpapier und drücke das Gehäuse an den Boden des Würfels.
  4. Den Arduino solltest du im hinteren Berecih des Würfels platzieren, so das der Raspberry ausreichend Platz hat.

### Step 12: Kabelsalat aufräumen
Verwendete Materialien:
1. Kabelbinder

Um den Kabelsalat innerhalb des Würfels ein wenig zu verringern solltest du hierzu Kabelbinder verwenden, mit dem du mehrere Kabel zusammenschnüren kannst.

## Programmierung

### Step 1: Entwicklung auf dem Raspberry Pi 3						

Die grafische Oberfläche des Qube wurde mit dem QT4 Designer realisiert. Dies ist ein Tool um die GUI per Drag & Drop zu erstellen.
Mit dem Python Framework PyQT4 kann man dann die erstellte Oberfläche einbinden und die dazugehörige Logik implementieren.
Der komplette Quellcode wurde mit Version 3 von Python realisiert.
Um die Resourcen des Raspberry's zu schonen wurde auf eine MySQL Datenbank verzichtet und eine SQLite3 Datenbank eingesetzt.
Um CRUD Operationen auf die Datenbank zu vereinfachen kommt das Python Toolkit und ORM SQLAlchemy zum Einsatz.
Um die Kommunikation zwischen dem Raspberry Pi und dem Arduino zu ermöglichen wird die Bibliothek python3-serial verwendet.

### Step 2: Raspbian installieren.
Falls noch nicht geschehen installiere Raspbian auf dem Raspberry Pi.
Am einfachsten geht das mit NOOBS. [Hier](https://www.raspberrypi.org/help/noobs-setup/) findet man die Anleitung dazu.

### Step 3: Benötigte Libraries installieren

> :warning:
  Die folgende Kommandos funktionieren NUR unter LINUX. Falls ein anderes Betriebssystem verwendet wird (z.B.: Windows 10 IoT) müssen diese entsprechend angepasst werden
  
Führe folgende Kommandos auf dem LX Terminal aus um die erforderlichen Libraries und den dazugehörigen Quellcode zu installieren.
Nachfolgendes Bild zeigt den LX Terminal und wo du ihn findest:

![LX Terminal](/images/taahw/lxterminal.jpg)

1. `$ sudo apt-get update`
2. `$ sudo apt-get upgrade`
3. `$ sudo apt-get install python3`
4. `$ sudo apt-get install sqlite3`
5. `$ sudo apt-get install python3-sqlalchemy` 
6. `$ sudo apt-get install python3-pyqt4`
7. `$ sudo apt-get install qt4-designer`
9. `$ sudo apt-get install python3-serial`
10. `$ git clone https://github.com/cbm-instructions/two-and-a-half-women.git`

Wenn du nur die Software installieren will ohne eigene Modifikationen an der GUI vorzunehmen muss Schritt 7 nicht ausgeführt werden.
Der Qt4 Designer wird nur benötigt um die GUI zu erstellen bzw. zu modifizieren.

### Step 4: Entwicklung für den Arduino Uno
Der Programmcode für den Arduino hast du mit Schritt 10 (siehe oben) schonn geladen sie befindet sich in src/arduino/arduino2pi/.
Du kannst auf deinem Raspberry Pi die Arduino IDE herunterladen und dann den Quellcode auf den Arduino hochladen. Dafür musst du die IDE mit dem Kommand `$ sudo apt-get install arduino`. Diese findest du dann unter Start->Elektronik->Arduino IDE.
Leider führte dies in unserem Fall zu erheblichem Problemen und wir entschieden uns dafür den Arduino an einen Windows PC/ Mac anzuschließen und den Quellcode von dort hochzuladen.
Die Arduino IDE bekommst du [Hier](https://www.arduino.cc/en/Main/Software).

### Step 5: Quellcode auf den Arduino laden
Sobal die IDE installiert wurde kannst du die Datei arduin2pi.ino öffnen. Diese befindet sich in dem Ordner src/arduino/arduino2pi/ in dem GitHub Repo, dass du vorher herunter geladen hast.

Mit einem einfachen Klick auf "Hochladen" wird das Programm auf den Arduino geladen. Dieser bestätigt das erfolgreiche Hochladen mit einem Blinken der eingebauten LED.

Es kann sein, dass der USB Port bzw. der Arduino an dem USB Port nicht richtigt erkannt wird. In diesem Fall muss der Port manuell geändert werden. Dies kannst du unter Werkzeuge->Port einstellen.

Wenn alle Buzzer, Knöpfe Kabel und Geräte miteinander verbunden worden sind kann deine erste Runde mit Qube erfolgen.

### Step 6: Jetzt geht's los. QUBE starten.
1. Gehe mit dem Terminal in das Verzeichnis in dem die Datei Qube.py liegt.
2. `$ python3 Qube.py`
3. Alternativ kannst du auch mit IDLE (Der Python IDE von Raspian) enweder Qube.py oder QubeHub.py öffnen und F5 drücken.

###Herzlichen Glückwunsch!!!
Du hast dir deinen eigenen Qube gebaut, benutze jetzt das Skript QubeHub.py um neue Fragen zu erstellen. Dies kannst du auf die gleiche Weise starten wie in Schritt 6 beschrieben.

Hier noch ein paar Eindrücke des kompletten Würfels.

![Finale I](/images/taahw/finale_I.jpeg)
![Finale II](/images/taahw/finale_II.jpeg)
![Finale III](/images/taahw/finale_III.jpeg)

## nützliche Quellen

PyQt API

http://pyqt.sourceforge.net/Docs/PyQt4/classes.html

sqlite3

http://www.einplatinencomputer.com/sqlite-statt-mysql/

gpiozero

https://gpiozero.readthedocs.io/en/v1.2.0/

GPIO and Interrupts

http://raspi.tv/2013/how-to-use-interrupts-with-python-on-the-raspberry-pi-and-rpi-gpio

QT4 Designer

http://www.rspilab.com/gui-application-development-using-qt4-designer-and-pyqt-in-raspbian-for-raspberry-pi/

SQLAlchemy

http://pythoncentral.io/introductory-tutorial-python-sqlalchemy/

http://www.sqlalchemy.org/

Verbindung zwischen dem Raspberry und Arduino herstellen

https://oscarliang.com/connect-raspberry-pi-and-arduino-usb-cable/

http://www.raspberry-pi-geek.de/Magazin/2013/05/Raspberry-Pi-und-Arduino-Uno-verbinden
