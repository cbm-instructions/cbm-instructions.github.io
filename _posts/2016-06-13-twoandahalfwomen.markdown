---
title: "Qube"
categories: instructions
layout: post
date:   2016-04-29 15:09:51 +0200
---

## Ziel/POV:
Ziel unseres Projektes ist es Studenten bzw. Interessenten für die Informatik und die Hochschule Mannheim zu begeistern und den Kommunikationsaustausch zu fördern. Ausserdem soll mit Hilfe dieses Projektes eine  freundlichere Atmosphäre geschaffen werden, damit sich Studierende gerne in der Fakultät für Informatik aufhalten. 

## Projektbeschreibung:
Unser Projekt umfasst ein Quiz, das mit Hilfe eines Raspberry Pi und einem Arduino realisiert wurde. Das Projekt wird in der Form eines Würfels dargestellt, an welchem die verwendeten Bauteil angebracht sind. Den Spielern ist es möglich einen Einspieler- oder auch Mehrspielermodus zu wählen. Die Steuerung bzw. Navigation des Quiz ist mithilfe der am Würfel angebrachten Buttons möglich. 

Erste 2 Sätze als Elevator Pitch für Social Media:
???

## Verwendete Materialien und Werkzeuge:

### Materialien:
  - 4x Plexiglas (25cmx25cm)
  - 2x Holz
  - 1x Raspberry Pi
  - 1x HDMI-Kabel für Raspberry Pi
  - 1x Mini USB-Kabel für Raspberry Pi Stromversorgung
  - 1x Arduino
  - 1x Netzteil für Arduino
  - 1x Breadboard
  - 2 x Push Dome Buttons (https://www.sparkfun.com/products/11274)
  - 5 x Happ Standard Arcade Button (blau, gelb, rot, grün, schwarz)
  - 2x Black IL Concave Arcade Start Button (http://www.arcadeworlduk.com/products/Black-IL-Concave-Arcade-Start-Button.html)
  - Kabel
  - Insulated Daisy Chain Harness with 32 Crimp Connections (http://www.arcadeworlduk.com/products/insulated-daisy-chain-harness-with-32-crimp-connections.html)
  - Pins
  - Verbindungen Pins
  - 1x Universalzylinderschloss
  - 1x 19 Zoll Monitor
  - 

### Werkzeuge:
  - Lötkolben
  - Lötzinn
  - Dremel
  - Bohrer
  - Standbohrmaschine
  - Kleber
  - 
  - 
  - 
  - ??
- Alles genau beschreiben (ID des Bauteils; genauer Name; auch für Kabel, ...)
- Mengenangaben für alle Bauteile
- Evtl. Links zu Shops und Datasheets




## Step 2:
## Step 3:
## Step 4:
## Step 5:

## Step 1: Grundlagen verstehen - Raspberry Pi und GPIO-Pins

_Für diesen Schritt brauchen wir: nichts - Grundlagenkapitel_

Das Raspberry Pi ist ein Einplatinencomputer mit besonders kleiner Baugröße und vielen programmierbaren Ein- und Ausgängen. Neben den USB-Anschlüssen für verschiedene Geräte, dem HDMI-Ausgang für Monitore und der LAN-Buchse, ist vor allem die GPIO-Pin-Leiste als Ein- und Ausgabeschnittstelle von Bedeutung. Über diese frei programmierbaren Pins können verschiedene digitale und analoge Ein- und Ausgabemedien angeschlossen werden, unter anderem: Buttons, LEDs und Sensoren.

Das Raspberry Pi kann unter anderem mit verschiedenen Linux-Distributionen betrieben werden. Hierdurch kann die Programmierung in allen unter Linux verfügbaren Programmiersprachen erfolgen. Zusätzlich können die verschiedenen Dienste von Linux genutzt werden, um beispielsweise Programme automatisch auszuführen und zu verwalten. Auch können Programme wie der Browser genutzt werden, welcher über den bereits integrierten Netzwerkstack mit dem Internet kommunizieren kann.

Diese Bandbreite an Funktionalitäten grenzt das Raspberry Pi gegenüber anderen Microcontrollern (bspw. Arduino) ab und macht es zu einer idealen Plattform für das vorliegende Projekt des Familienportraits. Wir verwenden hierbei das Raspberry Pi 2, Modell B. Dieses liefert im Vergleich zu seinen Vorgängern deutlich mehr Rechenleistung, was bei der Verarbeitung von Bildern in diesem Projekt sehr wichtig ist.

![Raspberry PI](/images/familienportrait/fp1.jpg)

## Step 2: Raspberry Pi an ein Steckbrett anschließen

_Für diesen Schritt brauchen wir: 1x Raspberry Pi 2, 1x Breadboard, Kabel in rot und schwarz, Steckbrücken für Breadboard_

Für den Zusammenbau der elektonischen Bauteile empfiehlt sich ein Steckbrett (Breadboard). Auf diese Weise können die einzelnen Bauteile schnell und ohne Werkzeuge zusammengesteckt, getestet und auch wieder auseinandergebaut werden. Wie ein Steckbrett funktioniert, wird hier erklärt: [http://deskfactory.de](http://deskfactory.de/funktion-breadboard) .Wichtig dabei ist zu verstehen, wie die einzelnen Pins des Steckbretts miteinander verbunden sind.

Nachdem die Funktionsweise des Steckbretts geklärt ist, müssen noch die einzelnen GPIO-Pins des Raspberry Pi betrachtet werden. Dabei hilft die folgende Seite: [http://de.pinout.xyz](http://de.pinout.xyz/). Im Rahmen dieses Tutorials werden immer die Pin-Nummer (schwarze Zahl direkt neben dem Pin) und die Funktion (größerer Text mit etwas Abstand zum Pin) angegeben.

Zunächst müssen der 5V-Pin und der Masse-Pin (GND) des Raspberry Pi mit dem Steckbrett verbunden werden. Wir verbinden in unserem Fall den Pin 2 (5v Stromversorgung) mit der roten Außenleiste des Breadboards und den Pin 6 (Masse, Ground) mit der blauen Außenleiste des Breadboards. Außerdem müssen die beiden Seiten der Außenleisten farblich korrekt miteinander verbunden werden.

![Steckbrett](/images/familienportrait/fp2.jpg)
![Steckbrett](/images/familienportrait/fp3.jpg)

## Step 3: Verlängerung der Komponenten durch Kabel

![Kabel](/images/familienportrait/fp4.jpg)

Für diesen Schritt brauchen wir: Abisolierzange, Kabellitzen, Kabel (male-male), Isolierband, Buttons und LEDs zum Testen

Im Rahmen dieses Projekts wollen wir eine Box bauen, welche über verschiedene Buttons und LEDs zur Ein- und Ausgabe verfügt. Deshalb ist es notwendig, dass wir diese Komponenten nicht nur auf dem Steckbrett anbringen, sondern sie auch an der Box befestigen. Hierzu müssen die Buttons und LEDs so bedrahtet werden, dass wir sie frei einbauen, aber dennoch auf dem verwendeten Steckbrett anschließen können.

Im Projekt haben wir dazu die folgende Vorgehensweise für jede einzelne Komponente genutzt:

  1. Schneidet von den Kabellitzen (am besten mit 2 verschiedenen Farben, vor allem bei LEDs) zwei gleichlange Stücke ab, die für die Länge zwischen dem Steckbrett und dem Befestigungsort ausreichen. Seid dabei großzügig, da wir einen Teil dieser Länge durch das Zusammenbauen wieder verlieren.
  2. Isoliert die Enden der Kabellitzen ab.
  3. Schneidet euch ca. 5cm lange Kabel mit male-Steckern zurecht und isoliert auch diese ab.
  4. Verbindet nun ein Ende der abisolierten Kabellitze mit dem abisolierten Ende des Kabels mit dem male-Stecker. Dazu könnt ihr die Enden miteinander verdrehen oder verlöten. Isoliert die Stelle mit dem Isolierband gut ab.
  5. Verbindet nun die andere Seite der Kabellitze mit dem Button oder der LED. Bei einigen Komponenten habt ihr dazu eine Schlaufe, durch welche ihr die Kabellitze durchziehen könnt. Bei anderen Komponenten (bswp. LED) müsst ihr eine solche Schlaufe erst zurechtbiegen. Sobald ihr die Kabellitze mit der Komponente verbunden habt, müsst ihr diese Verbindung ebenfalls isolieren.

Auf diese Weise könnt ihr die Komponenten an der Box befestigen und sie trotzdem ganz einfach auf dem Steckbrett ein- und ausstecken. Diese Technik wird für alle Buttons und LEDs in diesem Tutorial genutzt.

## Step 5: Buttons am Raspberry Pi

![Taster](/images/familienportrait/fp6.jpg)

_Für diesen Schritt brauchen wir: den bisherigen Aufbau, 8x Buttons, Kabel in rot und blau, 8x Steckverbinder male, Isolierzange, Isolierband_

Nun schließen wir die Buttons am Steckbrett an. In unserem Fall sind das die fünf Buttons für die Auslöser, der Button für das Neuladen der Website, der Button zum Umverteilen der Bilder und der Neustart-Button.

Zunächst wird jeder Button mit der einen Kontaktseite an die rote 5V-Leiste angeschlossen. Als nächstes muss die jeweils andere Seite der Buttons an jeweils einen bestimmten GPIO-Pin des Raspberry Pi angeschlossen werden. In diesem Tutorial müssen die folgenden GPIO-Pins verwendet werden, da diese im Code fest hinterlegt sind:

Die Auslöser werden an die Pins

  * 32 (BCM 16),
  * 35 (BCM 19),
  * 36 (BCM 16),
  * 37 (BCM 26) und
  * 38 (BCM 20) angeschlossen.


## Step 15: Webseite hochladen und einrichten

![Eingabemaske](/images/familienportrait/fp7.jpg)

Klicke in der Liste deiner Hosting-Konten in den Optionen deiner eingerichteten Webseite auf "Verwalten" und dann auf den Button "Webseite importieren". Du wirst auf eine neue Seite geleitet, welche eine Datei für die Webseite benötigt. Die nötige Datei heißt portrait-webseite.zip, diese findest du am Ende von diesem Step. Lade sie herunter und ziehe die zip-Datei per Drag & Drop in das graue Feld in der Mitte der Webseite. Nach kurzer Zeit solltest du eine positive Meldung erhalten haben, dass die Webseite erfolgreich importiert wurde. Wenn du nun wieder deine Webseite mit dem Zusatz "/portrait-webseite" im Browser aufrufst (in diesem Beispiel also http://portraitinstructable.esy.es/portrait-webseite), solltest du eine Testseite sehen, welche weiße Kästen mit den Zahlen Eins bis Fünf zeigt.

Wir sind jedoch noch nicht ganz fertig...

### PubNub-Schlüssel eintragen

Damit diese Webseite nun auch später mit unserem Raspberry Pi kommuniziert, müssen wir zwei Dateien der Webseite verändern und dort unsere Schlüssel von PubNub eintragen. Gehe zurück auf das Dashboard (Hosting -> Verwalten - dort wo du auf "Webseite importieren" geklickt hast) und scrolle zum Button "Dateiverwaltung 2". Klicke drauf und du wirst auf eine Seite weitergeleitet, welche die Ordnerstruktur deiner Webseite anzeigt. Klicke auf den Order "public_html" und danach auf den Ordner `portrait-webseite`. Du solltest eine Auflistung von mehreren Dateien und Ordnern sehen. Uns interessieren hier die Dateien `index.php` und `upload.php`. In diesen beiden Dateien müssen wir unsere Schlüssel von PubNub eintragen.

Du kannst beide Dateien direkt in dieser Dateiverwaltung editieren. Klicke hierfür auf einfach auf "edit", was sich rechts neben der jeweiligen Datei befindet.

Zunächst editieren wir die Datei `index.php`. Ein Fenster mit einem großen Textfeld sollte sich öffnen. Scrolle herunter bis du die folgende Zeilen findest:

```php
var pubnub = PUBNUB({
  subscribe_key: 'HIER SUBSCRIBE KEY EINTRAGEN'
});
```

Ersetze nun den Text "HIER SUBSCRIBE KEY EINTRAGEN" durch den von dir notierten Subscribe-Key von PubNub. Wichtig hierbei ist, dass du die Anführungszeichen nicht ersetzt. Tust du dies, wird es nicht funktionieren. Speichere deine Veränderungen, indem du auf das "Speichern"-Symbol am oberen Ende der angezeigten Seite klickst und danach auf den blauen Pfeil, um wieder in die Dateiverwaltung zu gelangen.

Das Gleiche machst du nun auch mit der `upload.php`-Datei. Hier musst du zwei Stellen editieren. Am unteren Ende der Datei befindet sich folgende Zeile:

```php
$pubnub = new Pubnub('HIER PUBLISH KEY EINTRAGEN', 'HIER SUBSCRIBE KEY EINTRAGEN');
```

Wie eben ersetzt du die beiden Texte jeweils durch den Publish- und Subscribe-Key von PubNub. Achte auch hier darauf, dass die Anführungszeichen erhalten bleiben. Speichern nicht vergessen!

Die Webseite ist nun fertig eingerichtet. Wir müssen in den folgenden Schritten noch das Raspberry Pi konfigurieren, sodass es die von der Webcam aufgenommenen Bilder auf die Webseite hochlädt und anzeigt.
