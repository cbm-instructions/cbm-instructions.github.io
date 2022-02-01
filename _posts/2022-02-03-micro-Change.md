#  How to build Ben the Bin
Thema des diesjährigen CBM-Projekts ist Nachhaltigkeit. Unsere Gruppe hat sich dafür auf die Müllproduktion eines Haushalts fokussiert. Mit unserem Produkt zeigen wir dem Nutzer diese auf und schaffen Anreize, das Verhalten nachhaltig positiv zu verändern.

<p align="center">
  <img width="400" height="650" src="/images/microChange/Ben_the_bin.png">
</p>

## Unser Produkt
*Ben* eignet sich am Besten für Papier- und Verpackungsmüll. In der Basis des smarten Mülleimers befinden sich Wägezellen, da wir die Müllproduktion anhand des Gewichts ermitteln. Dem Nutzer werden auf einem Display Statistiken und Errungenschaften angezeigt. Er kann Punkte sammeln, wenn er sein Konsumverhalten zum positiven verbessert bzw. sie bei Fehlverhalten wieder verlieren. Achievements wie *Baumtöter* visualisieren dies.

## Material

- Arduino Uno R3
- 2x HX711 ADC-Modul mit 5kg Wägezelle
	- z.B. hier bei [Conrad](https://www.conrad.de/de/p/joy-it-sen-hx711-10-waegezelle-passend-fuer-einplatinen-computer-arduino-raspberry-pi-1-st-2475885.html) zu kaufen
	- optional: Schnittstelle(n) zwischen Arduino und Wägezellen kaufen um sich das Löten zu sparen
- 5 Platten DIN A2 4mm Sperrholz, idealerweise aus Pappel  
	- z.B. hier bei [Bauhaus](https://www.bauhaus.info/sperrholzplatten/sperrholz/p/14453914) zu kaufen
-  Raspberry Pi 7 Display mit kapazitiven Touchscreen
- Breadboard klein
- 8x Jumperkabel (male to male)
- 4 Schraube und 8 Mutter 
- Holzleim
-  Klebeband
- Lötzinn


## Werkzeuge:
- LaserCutter
- Lötkolben
- Bohrmaschine
- Schraubenzieher

## Empfohlene Vorkenntnisse
* Hardwarenahe Programmiersprache wie C++
* Python und Javascript
* Umgang mit Mikrocontrollern
* Lasercutterworkshop

## Bauanleitung
### Die Bodenplatte bauen
Jede Wägzelle muss mit einer geraden Fläche oben und unten verschaubt sein. Dafür lasercutten wir zwei Quadrate á 20x20cm. 
Die Wägezellen werden parallel zueinander mit passenden Schrauben und Muttern befestigt:
<p align="center">
  <img width="350" height="350" src="/images/microChange/bodenplatte.jpg">
</p>
<p align="center">
  <img width="350" height="350" src="/images/microChange/waegzellen.jpeg">
</p>
Da die Schrauben überstehen, wurden auf der Unterseite noch Reststücke vom Lasercutten angeklebt. Ansonsten würde die Bodenplatte wackeln; auf der Oberseite ist dies nicht zwingend nötig. So sieht das ganze später von oben aus:
</p>
<p align="center">
  <img width="350" height="350" src="/images/microChange/oben.jpeg">
</p>

### Den Mülleimer bauen
Die [.svg Datei](../images/microChange/Konsole.svg) hierfür wurde auf [festi.info](https://www.festi.info/boxes.py/)  erstellt. Dabei haben wir das Preset _Console2_ ausgewählt, weil wir die Schräge für unser Display wollten. Wichtig dabei war, den Parameter  _thickness_ auf unser Holz anzupassen. _Burn correction_ wurde von 0,1 auf 0,09 reduziert. Dadurch hat man beim Zusammenstecken etwas mehr Spiel, was bei der Größe unserer Box hilfreich ist. Vor dem Lasercutten sollte man sich vergewissern, dass die Linienstärke bei 0,035mm und die Farbe schwarz (RGB000) ist. Dies sieht man z.B. in _Adobe Illustrator_ oder _Inkscape._ Wir haben Pappelsperrholz als Material gewählt.  Die hiermit erstellten Pläne lassen sich einfach zusammenstecken und sind optisch ansprechend. Für die Breite und Tiefe wurde sich nach der Bodenplatte gerichtet, theoretisch lassen sich die Maße abändern solange die Bodenplatte noch rein passt.

<p align="center">
  <img width="400" height="600
  " src="/images/microChange/mülleimer_seitlich.jpeg">
</p>
Zusätzlich haben wir eine Trennwand ausgeschnitten, die Müll und Elektronik trennt. Die svg-Datei hierfür befindet sich 
[hier](../images/microChange/Trennwand.svg). Da wir die Trennwand herausnehmen wollen, haben wir an beiden Seiten eine Art Schiene gebastelt:
<p align="center">
  <img width="300" height="400" src="/images/microChange/schiene.jpeg">
</p>
Wichtig ist,  alles erst zusammenzustecken, wenn der nächste Schiritt, der Einbau der Elektronik vollendet ist.
Um das ganze optisch abzurunden wurde auf der Rückseite ein kleines Loch für das Netzkabel sowie ein Rechteck mit den Maßen 21,7x1,7cm ausgeschnitten. Letzteres schließt den Spalt zwischen Trennwand und Display. Dies ist allerdings nur Kosmetik.

#### Einbau der Elektronik
Zuerst wird das Display auf der Frontstück des Mülleimers geschraubt. Hierfür sollte vorgebohrt werden, damit das Holz nicht bricht.
</p>
<p align="center">
  <img width="400" height="300" src="../images/microChange/.front.jpeg">
</p>
</p>
<p align="center">
  <img width="400" height="300" src="../images/microChange/.front_display.jpeg">
</p>
Die restliche Elektronik wird in dem Kompartment vor der Trennwand untergebracht. Dabei sollte kein starker Zug auf den Kabeln sein.
<p align="center">
  <img width="250" height="400" src="/images/microChange/.arduino_eingebaut.jpeg">
</p>
<p align="center">
  <img width="250" height="400" src="/images/microChange/.elektronik_innen.jpeg">
</p>
Nun können alle Holzwände zusammengesteckt und das Frontstück mit Holzleim gefestigt werden.

## Ausblick
Als Nächstes wäre eine Vernetzung mit anderen smarten Mülleimern denkbar. So könnte man sich mit Freunden, Fremden und dem aktuellen Durchschnitt vergleichen. Eine feinere Unterscheidung des Abfalls mittels Bilderkennung und maschinellem Lernen ist ebenfalls denkbar aber nicht trivial umzusetzen.

Die Basis mit den Wägezellen hat sich als sehr genau bewiesen und ist  damit auch für andere Anwendungszwecke geeignet.

