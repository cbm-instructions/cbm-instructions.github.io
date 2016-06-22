---
title: "How To Build The Qube Quiz"
categories: instructions
layout: post
date:   2016-04-29 15:09:51 +0200
---

## Ziel/POV:
Ziel unseres Projektes ist es Studenten bzw. Interessenten für die Informatik und die Hochschule Mannheim zu begeistern und den Kommunikationsaustausch zu fördern. Ausserdem soll mit Hilfe dieses Projektes eine  freundlichere Atmosphäre geschaffen werden, damit sich Studierende gerne in der Fakultät für Informatik aufhalten und w. 

## Projektbeschreibung:
Qube der Würfel der Wissen schafft. Unser Projekt umfasst ein Quiz, das mit Hilfe eines Raspberry Pi und einem Arduino realisiert wurde. Das Projekt ist in der Form eines Würfels dargestellt, an welchem die verwendeten Bauteile angebracht sind. Den Spielern ist es möglich einen Einspieler- oder auch Zweispielermodus zu wählen. Die Steuerung bzw. Navigation des Quiz ist mithilfe der am Würfel angebrachten Buttons möglich. 

## Verwendete Materialien und Werkzeuge:

### Materialien:
  - 4x Plexiglas (24,75cm x 24,75cm x 0,4cm) | ca. 12€
  - 4x Plexiglas (25,25cm x 25,25cm x 0,4cm) | ca. 5€
  - 1 x Plexiglas (24,05cm x 25,25cm x 0,04cm) | ca. 2€
  - Milchglasfolie (gibt es im Bauhaus von d-c-fix) | ca. 6€
  - 1x MDF Platte schwarz (27cm x 30cm x 0,19cm) | ca. 3€
  - 1x Raspberry Pi 3 (https://www.amazon.de/Raspberry-Pi-3-Model-B/dp/B01CEFWQFA)
  - 1x Mini USB-Kabel Ladegerät für Raspberry Pi 3 Stromversorgung (https://www.amazon.de/Raspberry-Pi-Micro-USB-Netzteil/dp/B00SVALHXU)
  - 1x USB oder Bluetooth Maus für den Raspberry Pi 3
  - 1x USB oder Bluetooth Tastatur für den Raspberry Pi 3
  - 1x Arduino Uno (https://www.amazon.de/Arduino-Uno-Rev-3-Mikrocontroller-Board/dp/B008GRTSV6/ref=sr_1_1?ie=UTF8&qid=1466531263&sr=8-1&keywords=Arduino+uno)
  - 1x Netzteil für Arduino Uno - Goobay 2798 - Universal Netzgerät 3-12 V (https://www.amazon.de/Goobay-2798-Universal-Netzgerät-3-12/dp/B0038WU2Z0) (https://www.amazon.de/Goobay-2798-Universal-Netzger%C3%A4t-3-12/dp/B0038WU2Z0) 
  - 1x Laptop/PC um den Arduino zu programmieren
  - 2 x Push Dome Buttons blau (https://www.amazon.de/Big-Dome-Push-Button-Blue/dp/B008FZJ2WE)
  - 5 x Happ Standard Arcade Button (blau, gelb, rot, grün, schwarz) (http://www.watterott.com/index.php?page=search&page_action=query&desc=on&sdesc=on&keywords=Einbautaster&x=0&y=0)
  - 2x Black IL Concave Arcade Start Button (http://www.arcadeworlduk.com/products/Black-IL-Concave-Arcade-Start-Button.html)
  - Kabel
  - Insulated Daisy Chain Harness with 32 Crimp Connections [= Isolierter verketteter Kabelstrang mit 32 Crimpverbindungen] (http://www.arcadeworlduk.com/products/insulated-daisy-chain-harness-with-32-crimp-connections.html)
  - Verbindungskabel RB-CB3-25 (https://www.conrad.de/de/raspberry-pi-verbindungskabel-rb-cb3-25-1182193.html)
  - Pins (Male) für Verbindungskabel
  - Kabelhülsen
  - Isolierband
  - 1x Universalzylinderschloss (https://www.bauundhobby.ch/maschinen-%2B-werkstatt/sicherheit/schlösser-%2B-zylinder/univ.zylinderschloss-zs-77-sb/C041202/P3191726/de)
  - 1x 19 Zoll Monitor
  - 1x Adapterkabel HDMI auf DVI (z.B. https://www.amazon.de/AmazonBasics-Adapterkabel-HDMI-auf-DVI-Schwarz/dp/B00NH11X64)
  - 2x Acryl Scharniere 64mm (https://www.amazon.de/gp/product/B00R0BCWNU/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1)
  - Tesa Power Strips Small (https://www.amazon.de/tesa-Powerstrips-Strips-SMALL-Packung/dp/B000KJR2ES/)
  - Tesa Powerbond
  - Neopixel 1 Meter (https://www.adafruit.com/product/1460)
  - 1x Styroporkugel Ø8cm
  - 5x Kabelbinder

### Werkzeuge:
  - Lötkolben
  - Dremel
  - Aufsatz Dremel Schleifscheibe/Trennscheibe
  - Aufsatz Dremel Minikreissägeblatt
  - Standbohrmaschine
  - Lochsäge Ø25mm
  - 6er Bohrer  
  - Forstner Bohrer Ø??mm für Zylinderschloss
  - Pattex Kleber
  - Schere
  - Abisolierzange
  - Cutter Messer
  - Geodreieck
  - Kugelschreiber
  - Feuerzeug / Heißluftfön

## Step-by-Step Guide - Arcade Buttons & Push Dome Buttons

### Step 1: Kabel an Switchcontroller der Arcade Buttons und Push Dome Buttons löten
Für diesen Schritt benötigen wir: Abisolierzange, Lötkolben, Kabelhülse, Kabel, Feuerzeug, Schere

Damit die Arcade Buttons verwendet werden können, müssen an den Switch Coontrollern der Arcade Buttons und der Push Dome Buttons Kabel angebracht werden. So dass diese zu einem späteren Zeitpunkt an die GPIO-PINS des Raspberry PI angeschlossen werden können.

Dazu haben wir in unserem Projekt die folgende Vorgehensweise für alle 7 Arcade Buttons und die 2 Push Dome Buttons genutzt:
  1. Schneide dir ein Kabel in ausreichnder Länge von ca. 25cm  zurecht, da beim verbauen ein Stück der Länge verloren geht. Am besten du nimmst Kabel in den Farben der Arcade Buttons und Push Dome Buttons, um diese besser zu unterscheiden.
  2. Isoliere jeweils beide Kabelenden mit einer Abisolierzange ab.
  
  ![Kabel](/image/taahw/01.JPG)

  3. Als nächstes nimmst du eines der Kabelenden und lötest dies mit Hilfe des Lötkolben an den Microswitchcontroller eines Buttons/Buzzers.

  ![Kabel_Button](/images/taahw/02.jpg)

  4. Nun musst du das verlötete Kabel mit einer Kabelhülse oder einem Isolierband am Switchcontroller isolieren.
  
  ![Kabelhülse](/images/taahw/03.jpg)

  5. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt. 
  
![Kabelhülse](images/taahw/04.jpg)
  
Dieses Vorgehen wurde für alle Arcade Buttons und Push Dome Buttons dieses Projektes angewandt.

### Step 2: Kabel der Arcade Buttons und Push Dome Buttons verlängern
Um Step 2 durchzuführen benötigen wir: Schere, Abisolierzange, Lötkolben, Kabelhülse, Verbindungskabel RB-CB3-25, Feuerzeug

Das in Step 1 verlötete Kabel solltest du noch mit einem Verbindungskabel RB-CB3-25 erweitern. Dieser Schritt ist notwendig, damit du die Arcade Buttons und Push Dome Buttons an die GPIO-PINS des Raspberry PI anschließen kannst.

Hierzu haben wir uns im Rahmen des Projektes für nachfolgende Vorgehensweise entschieden:
  1. Nehmt das Verbindungskabel RB-CB3-25 und schneidet es an gewünschter Stelle ab, so das noch eine ausreichende Länge zum verlöten vorhanden ist.
  2. Danach solltest du es an der abgeschnittenen Seite mit einer Abisolierzange abisolieren.

  ![Verbindungskabel](/images/taahw/05.JPG)

  3. Nun nimmst du einen Arcade Button oder Push Dome Button, an dem Step 1 bereits durchgeführt wurde und verbinde die jeweiligen abisolierten Kabelenden mit Hilfe des Lötkolben.

![Verbindung](/images/taahw/06.JPG)  

  4. Danach solltest du die Kabelhülse über das Ende des Verbindungskabel (Female) bis zur Lötstelle ziehen 
  
![Kabelhülse](/images/taahw/07.jpg)

  5. Nun solltet du die Lötstelle mit der überzogenen Kabelhülse oder einem Isolierband isolieren.
  6. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.
  
![Verbindungskabel](/images/taahw/08.jpg)

Auch dieses Vorgehen wurde für alle Arcade Buttons und Push Dome Buttons dieses Projektes angewandt.

### Step 3: Kabel an die LED der Push Dome Buttons anbringen
Benötigte Materialien: Schere, Abisolierzange, Lötkolben, Kabel, Kabelhülse, Feuerzeug

Für die LED der Push Dome Buttons werden ähnliche Schritte wie in Step 1 durchgeführt. Auch hier ist es ratsam verschiedenfarbige Kabel wie z.B. blau und rot wie in unserem Projekt zu verwenden, um - und + zu unterscheiden.

Hierfür gehst du wie folgt vor:
  1. Schneide dir zwei Kabel in ausreichnder Länge von ca. 25cm zurecht, da beim verbauen ein Stück der Länge verloren geht. Du solltest hierfür ein blaues und ein rotes Kabel zur beseseren Unterscheidung benutzen.
  2. Isoliere jeweils beide Kabelenden des blauen und roten Kabels mit einer Abisolierzange ab.
  3. Als nächstes nimmst du das Kabelende des blauen Kabel und lötest dies mit Hilfe des Lötkolben an den Minuspol an.
  4. Nun nimmst du eines der Kabelnenden des roten Kabel und lötest dies an die gegenüberliegende Seite an. 
  4. Nun musst du die verlöteten Kabel mit einer Kabelhülse oder einem Isolierband am Minus- und Pluspol isolieren.
  5. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.
  
![Push Dome Button](/images/taahw/09.jpg)

### Step 4: Switchcontroller der Arcade Buttons und Push Dome Buttons mit dem Insulated Daisy Chain Kabelstrang verbinden
Benötigt werden: Insulated Daisy Chain Kabelstrang, Schere, Alle Buttons

Mit Hilfe des Crimp Kabelstrangs werden die einzelnen Switchcontroller der Buttons und der Buzzer verbunden. Hierfür werden 10 Steckverbindungen des Crimp Kabelstrangs benötigt. Die Reihenfolge der Anschlüße sollte hierbei keine Rolle spielen, da dies über das Programm gesteuert wird.

![Kabelstrang](/images/taahw/10.jpg)

In unserem Projekt haben wir die Verbindungen zwischen den Komponenten in der Reihenfolge
  - Arcade Button rot
  - Arcade Button blau
  - Arcade Button gelb
  - Push Dome Button 1
  - Push Dome Button 2
  - Arcade Button schwarz
  - Arcade Button geün
  - Arcade Button (1 Player)
  - Arcade Button (2 Player)
gewählt.

Dazu gehen wir folgendermaßen vor:
  1. Als erstes nimmst du den ersten Crimp Stecker des Kabelstrangs und befestigt diesen an den den Switchcontroller com Anschluss des blauen Arcade Button.
  
  ![Verbindungskabel](/images/taahw/11.jpg)
  ![Verbindungskabel](/images/taahw/11_1.jpg)
  ![Verbindungskabel](/images/taahw/11_2.jpg)

  2. Der zweite Crimp Stecker wird an den Switchcontroller com Anschluss des roten Arcade Button angeschlossen.
  3. Der dritte und vierte Crimp Stecker an die Switchcontroller com Ports des gelben und grünen Arcade Button.
  4. Danach wird der schwarze Arcade Button verbunden gefolgt von den Player Buttons.
  5. Am achten und neunten Crimp Stecker musst du die zwei Push Dome Buttons anschließen.
  6. Bisher hast du 9 der 35 Stecker verwendet. Die Verbindung musst du nach dem zenhten Crimp Stecker mit einer Schere trennen, um das Kabel im nächsten Schritt zu verlängern.

### Step 5: Insulated Daisy Chain Harness verlängern
Wir benötigen: Verbindungskabel RB-CB3-25, Schere, Kabelhülse, Lötkolbe, Kabelstrang

Wie schon erwähnt verbinden wir nun das Ende des Kabelstrangs mit einem Verbindungskabel RB-CB3-25, damit dieses auch an einen der GPIO Pins am Raspberry angeschlossen werden kann. 

Hierfür führt ihr folgende Steps aus:
  1. Den zehnten Crimp Stecker trennen wir nun ebenfalls mit einer Schere.
  
![Verbindungskabel](/images/taahw/12.jpg)

  2. Danach solltet ihr das Kabelende mit einer Abisolierzange abisolieren.

![Verbindungskabel](/images/taahw/13.jpg)  

  3. Nun nimmst du das Verbindungskabel RB-CB3-25, welches die gleiche Farbe wie der Kabelstrang haben sollte, zur Hand und schenidet eines der Female Stücke ab, sodass das Kabel ausreichend lang ist.
  
![Verbindungskabel](/images/taahw/05.jpg)

  4. Auch dieses Kabel musst du am abgeschnittenen Ende abisolieren.
  5. Als nächstes verlötest du das Ende des Crimp Kabelstrangs mit dem zuvor isolierten Verbindungskabel.
  6. Nun musst du die verlöteten Kabel mit einer Kabelhülse oder einem Isolierband isolieren.
  ![Verbindungskabel](/images/taahw/07.jpg)
  7. Die Kabelhülse musst du mit einem Feuerzeug oder einem Heißluftfön erhitzen, damit sich diese zusammenzieht und so die Lötstelle verdeckt.
  ![Verbindungskabel](/images/taahw/08.jpg)

### Step 6: Arcade Buttons und Push Dome Buttons mit GPIO von Raspberry verbinden

In diesem Schritt werden wir die angebrachten Verbindungskabel an die GPIO Pins des Raspberry PI anschließen.
Die Pinbelegung des Raspberry lautet wie folgt:

![GPIO](/images/taahw/14.png)

Hinweis: Um die Pins korrekt lesen zu können, sollten die USB-Anschlüssen des Raspberry nach unten zeigen.

![GPIO]/images/taahw/15.jpg

Arcade Button Blau: PIN 22
Arcade Button Gelb: PIN 29
Arcade Button Grün: PIN 16
Arcade Button Rot: PIN 18
Arcade Button Schwarz: PIN 13
Arcade Button Player 1: PIN 12
Arcade Button Player 2: PIN 11
Push Dome Button 1: PIN 15
Push Dome Button 2: PIN 31

Auch das Kabelende des oben verwendeten Kabelstrangs aus Stepp 5 solltest du an einen GPIO Pin anschließen, so benötigst du kein Breadboard und habt später mehr Platz im Würfel.

Button mit Kabelstrang-Ende: PIN 6

![GPIO](/images/taahw/16.jpg)

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
  
/images/taahw/18.jpg


### Step 8: Kabel an Neopixelstreifen löten
Hierfür benötigt ihr folgendes: Lötkolben, Abisolierzange, Neopixelstreifen, Isolierband

Der Neopixelstreifen hat sowohl Input als auch Output. In unserem Projekt benötigen wir die Input Seite. Dort werden drei verschiedenfarbige Kabel angeschlossen, in unserem Prrojekt haben wir die Farben 
  - rot = 5V 
  - gelb = Dh (Mitte) 
  - grau = GND 
verwendet.

!Neopixel(images/twoandahalfwomen/???.jpg)

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

/images/twoandahalfwomen/21.jpg

### Step 12: Raspberry und Monitor verbinden
Benötigte Materialien: Monitor, Raspberry Pi 3, HDMI Kabel oder -Adapter

Um die Grafische Oberfläche an einem Monitor anzeigen zu lassen, muss ein Monitor an den Raspberry angeschlossen werden. Dies geschieht entweder direkt über ein HDMI Kabel oder mit einem entsprechenden Adapter.

/images/twoandahalfwomen/??.jpg

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

Um die Löcher zu bohren wird zuerst ein Loch mit dem kleinen Bohrer vorgebohrt bevor dann mit der Lochfräse (25mm) die Löcher gebohrt werden können.

Am besten spannt man die Lochfräse in einen Standbohrer, um die nötige Stabilität zu bekommen.

![Standbohrer](images/taahw/bohrer/stand.jpg

Beim Bohren darf nicht mit zu hohen Umdrehungen gebohrt werden, da ansonsten die Platten zu schmelzen beginnen. Dies erkennt man an einem immer stärker werdenden beißenden Geruch.

Da das Schmelzen nicht komplett verhindert werden kann müssen die Löcher bzw. die Schmelzrückstände an den Löchern mit einem Dremel weggeschliffen werden.

Da die 25mm für die farbigen Buttons zu klein sind muss mit einem Dremel mit passendem Schleifaufsatz nach geholfen werden, damit die Buttons passen.

Im Falle der Buzzer müssen die Löcher nur noch von den Schmelzrückständen entfernt werden und dann passen die Buzzer in die Löcher.
Die Buzzer sitzen sehr locker in den gebohrten Löcher aber das ist nicht weiter schlimm da die Buzzer zustätlich befestigt werden können.

Wenn du mit den Löchern fertig bist sollte das Ergebnis ungefähr so aussehen.

//Bild mit fertigen Löchern zeigen

Auf der Vorderseite (die zukünftige Vorderseite des Würfeln) müssen noch drei weitere Löcher angebracht werden. Zwei Löcher für jeweils den Ein - und Zweispielerbutton sowie ein Loch für den Navigationsbutton.

Um die Löcher zu bohren musst du genauso vorgehen wie zuvor auch.

### Step 2: Loch und Schlitz für das Zylinderschloss bohren

Benötigte Materialien:
1. Rückplatte (24,05cm x 25,25cm x 0,04cm)
2. Dremel mit Mini Sägen Aufsatz
3. 6er Bohrer zum vorbohren
4. Dremel

Um die Sicherheit des Qubes zu erhöhen bzw. zu verhindern, dass nichts geklaut wird ist es sinnvoll noch zusätzlich ein Schloss anzubringen. Zusätzlich zu diesem Schloss werden noch Scharniere an die Rückplatte angebracht damit sich diese leicht öffnen lässt.
Diese Scharniere werden mit Pattex Kraftkleber an der Bodenplatte angebracht. Das ankleben der Scharniere wird erst in Schritt ??? erfolgen sollte aber an dieser Stelle schonmal erwähnt werden.

Um das Loch für das Schloss zu bohren wird zuerst die Mitte der Platte festgelegt und mit einem Abstand zur oberen Kante von ???mm eine Markierung gesetzt. Mit Hilfe dieser Markierung wird zuerst wieder ein Loch vorgebohrt bevor dann mit einem ??? ein Loch mit einem Durchmesser von ??? gebohrt werden kann.

Um den Schließmechanismus des Schlosses zu vervollständigen muss zusätzlich ein Schlitz für den ??? an der Oberseite des Würfels (die Platte mit den meisten Löächern die in Schritt 1 gefertigt wurde) eingefräst werden.

Um den Schlitz zu bohren nimmst du einen speziellen Mini Sägen Aufsatz für den Dremel. In dem nachfolgenden Bild wird die Mini Säge dargestellt.

//Mini Säge bild

### Step 3: Aussparrung für Raspberry und Arduino sägen

Benötigte Materialien:
1. Rückplatte (24,05cm x 25,25cm x 0,04cm)
2. Laubsäge
3. Schleife
4. Dremel

Damit der HDMI Eingang sowie die Eingänge für die Netzteile für das Raspberry und den Arduino zugänglich sind muss am unteren Ende der Rückplatte eine Aussparung gefräst werden.

Neben der Aussparrung für die Kabel muss rechts und links noch Platz gelassen werden für die Scharniere damit die Rückwand geöffnet werden kann.
Abzüglich der Breite der zwei Scharniere bleibt für die Aussparung eine Breite von ca. ???mm übrig. Dies passt genau um direkt dahinter den Raspberry anzubringen und damit ein wenig Luft bleibt für die externe Stromzufuhr des Arduinos.

Aufzeichnen, mit Dremel oder einer Laubsäge sägen, Kanten abschleifen

### Step 4: Milchglasfolie anbringen

Benötigte Materialien:
1. Milchglasfolie
2. alle Platten, die beklebt werden sollen
3. Klebefolien Befestigungsset
4. Cutter Messer

Uns war es wichtig, dass Nutzer des Qubes in den Würfel hinein blicken konnten und so die Elektronik sehen können. Deswegen haben wir uns dafür entschieden nur die zwei Seitenplatten sowie die Oberplatte mit Michglasfolie zu bekleben.

Damit der spätere Lichteffekt des LED Streifens besser zur Geltung kommt kann aber auch der komplette Würfel mit Folie beklebt werden.

Um die Milchglasfolie auf die Platten anzubringen ist es das einfachste wenn die Klebeseite der Milchglasfolie zuerst freigelegt und dann die Folie mit der Klebeseite nach oben flach auf einem Tisch ausgebreitet wird, dann kann man die Klebefolie entlang der Kanten abschneiden.
Danach muss die Klebefolie sofort mit dem Schaber des Klebefolien Befestigungssets glatt gestrichen, werden um die entstandenen Luftblässchen zu entfernen.

Da du jetzt alle gebohrten Löcher mit der Klebefolie beklebt hast, musst du nun die Löcher wieder ausschneiden. Dies funktioniert am besten mit einem Cutter Messer.

Dazu die Platte auf den "Kopf" legen und an den Lochkanten entlang die Löcher ausschneiden.

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

Dies ist auf nachfolgender Zeichnung zu erkennen:

//Patric Bild
Damit die Platten bestmöglichst aufeinander kleben empfiehlt es sich auf der vorgesehenen Klebefläche (4mm breit) die zuvor angebrachte Michglasfolie zu entfernen. Das machst du am indem man die Folie vorsichtig mit dem Cutter Messer einschneidet (sodass die Platte nicht beschädigt wird) und dann abzieht.

Wenn du das erledigt hast kann wirklich mit dem Bekleben begonnen werden.

Zum Bekleben fülle ein biscchen von dem Patex Kraftkleber in ein Behälter. Jetzt kannst du mit Hilfe des alten Pinsels den Kleber auf die Klebefläche aufbringen. Wichtig ist, dass nicht nur eine Seite sondern beide Seiten die verklebt werden sollen mit dem Kleber versehen werden. Anschließend kannst du den Kleber leicht antrocknen lassen und stark zusammenpressen.

Damit die inneren Winkel auch hundertprozentig rechtwinklig werden kann ein Geodreieck, zur Unterstützung,  zwischen die Platten gelegt werden. 

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

### Step 8: Zylinderschloss befestigen
Benötigte Materialien: Zylinderschloss, hintere Plexiglasscheibe

Vorgehensweise:
  1. Zuerst nimmst du das Zylinderschloss zur Hand und schraubt dieses auf, sodass du es an der hinteren Plexiglasseite einsetzen kannst.
  2. Als nächstes setzt du das Zylinderschloss ein und schraubst es fest.
  3. Nun richtest du es so aus, dass der Würfel mit der oberen Seite abschließbar ist.
 ![Zylinderschloss](images/taahw/22.jpeg)

### Step 9: Würfel an Holzplatte kleben
Benötigte Materialien: Würfel, MDF Platte, Kleber, Bleistift, Geodreieck, Pinsel

Vorgehensweise:
  1. Als erstes nimmst du die MDF Platte zur Hand und markierst, wo du den Würfel anbringen möchtest.
  2. Dazu zeichnest du ein Quadrat mit den entsprechenden Maßen.
  3. Nun verteilst du den Kleber mit einem Pinsel in dem eben gezeichneten Quadrat.
  4. Als nächstes nimmst du den Würfel und drückt diesen auf die MDF Platte.
  5. Zum Schluß solltest du ihn eine Weile trocknen lassen, so das die Bauteile fest miteinander verbunden sind.

### Step 10: Raspberry an Würfel anbringen
Benötigte Materialien: Raspberrymit Gehäuse, Würfel, Tesa Powerbond, Schere

Vorgehensweise:
  1. Als erstes schneidest du dir zwei Streifen Tesa Powerbond zurecht.
  2. Diese klebst du jeweils rechts und links an die Unterseite des Raspberry Gehäuse.
  3. Entferne nun das Schutzpapier und drücke das Gehäuse an den Boden des Würfels.
  4. Hierbei solltest du darauf achten, dass in der Aussparrung der hinterseite des Würfels genug Platz für das Stromkabel des Arduinos vorhanden ist.
  
![Aussparrung](/images/taahw/23.jpeg)

### Step 11: Arduino an Würfel anbringen
Benötigte Materialien: Arduino mit Gehäuse, Würfel, Tesa Powerbond, Schere

Vorgehensweise:
  1. Als erstes schneidest du dir zwei Streifen Tesa Powerbond zurecht.
  2. Diese klebst du jeweils rechts und links an die Unterseite des Arduino Gehäuse.
  3. Entferne nun das Schutzpapier und drücke das Gehäuse an den Boden des Würfels.
  4. Den Arduino solltest du im hinteren Berecih des Würfels platzieren, so das der Raspberry ausreichend Platz hat.

### Step 12: Kabelsalat aufräumen
Verwendete Materialien: Kabelbinder

Um den Kabelsalat innerhalb des Würfels ein wenig zu verringern solltest du hierzu Kabelbnder verwenden. Mit Hilfe der Kabelbinder lassen sich mehrere Kabel zusammenschnüren.

## Programmierung:

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

//lxTerminal.jpg

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

#### nützliche Quellen

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
