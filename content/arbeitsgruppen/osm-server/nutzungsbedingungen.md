# Nutzungsbedingungen OSM-Server des FOSSGIS e.V.

Die vom FOSSGIS e.V. betriebenen Services werden von Ehrenamtlichen
mit Spendenmitteln betrieben. Ihr Hauptzweck ist, die Nutzung auf unserer
Website sowie die Beitragenden zu OpenStreetMap bei ihrer Arbeit zu unterstützen.
Wir sind grundsätzlich erfreut darüber, wenn unsere Services von Dritten für
kreative und innovative Anwendungen genutzt werden.
Aber eine zu starke Nutzung schränkt die Nutzbarkeit ein. Daher
verlangen wir, dass alle Nutzer der Services des FOSSGIS e.V. sich an diese
Nutzungsbedingungen halten.

**OpenStreetMap-Daten können [von jedem frei und kostenlos genutzt
werden](https://www.openstreetmap.org/copyright). Unsere Services hingegen
nicht.**

Im Folgenden sind die Mindestvoraussetzungen aufgeführt, die die Nutzer
einhalten müssen.

Auch viele andere Organisationen stellen ähnliche Services auf Basis von
OpenStreetMap-Daten zur Verfügung. Falls dein Projekt den Anforderungen hier
nicht gerecht wird, kannst du das selbe von anderen Anbietern beziehen (siehe
unten).

## Geltungsbereich

Diese Nutzungsbedingungen gelten für
* die Tileserver des FOSSGIS e.V. (tile.openstreetmap.de).
* die Routingserver des FOSSGIS e.V. (routing.openstreetmap.de, valhalla1.openstreetmap.de)

Sie gelten nicht für die Routing- oder Tileserver anderer Betreiber (z.B.
tile.openstreeetmap.org der OpenStreetMap Foundation und diverse gewerbliche
Anbieter) und auch nicht für die Nutzung der OpenStreetMap-Rohdaten. Die
Nutzung der OpenStreetMap-Daten unterliegt den Bedingungen der Open Database
License 1.0.

## Allgemeine Regeln

### Voraussetzungen

* Klare Anzeige der Quellenangabe, wie sie von der Lizenz und der
  OpenStreetMap Foundation
  [verlangt](https://www.openstreetmap.org/copyright) wird.
* Ergänzen Sie einen Link zu
  [https://www.openstreetmap.org/fixthemap](https://www.openstreetmap.org/fixthemap),
  um Ihren Nutzern zu erlauben, Fehler in unseren Daten zu melden und zu beheben.
  Der folgende HTML-Code erfüllt diese Regeln:

```html
  Daten © <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</code>-Mitwirkende
  (<a href="https://opendatacommons.org/licenses/odbl/index.html">ODbL</a>), <a
  href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, <a
  href="https://openstreetmap.org/fixthemap">mitmachen/Fehler melden</a>
```
  Bei Medien, bei denen Links technisch nicht möglich sind, genügt `Daten: ©
  OpenStreetMap-Mitwirkende (ODbL), Grafik: CC-BY-SA`.
* Bei Websites muss eine E-Mail-Adresse des Betreibers leicht erkennbar und
  unmittelbar erreichbar sein, um diesen bei Bedarf kontaktieren zu können. Bei
  Apps gilt dies für die Website der App und deren Einträge in App-Stores.
* Ausdrücklich empfohlen: Die URLs unserer Services sollten nicht in der App
  fest einprogrammiert werden.

### Technische Nutzungsvoraussetzungen

* **Gültiger HTTP-User-Agent**, der die Anwendung identfiziert. Die User-Agents
  von Bibliotheken sind nicht ausreichend. Das Vortäuschen einer anderen Anwendung
  führt sicher zur Sperrung.
* Eine gültige Angabe der Ursprungsseite (HTTP-Referrer) sofern dies
  technisch möglich ist.
* **Maximal zwei herunterladende Verbindungen.** (Die unmodifizierten
  Einstellungen der üblichen Website-Betrachter sind akzeptabel.)

Anmerkung: Übliche Web-Browser ohne modifizierte Konfiguration halten
normalerweise alle der oben stehenden technischen Nutzungsvoraussetzungen ein.

### Nicht erlaubte Nutzungen

* Die gewerbliche Nutzung ist nur gestattet, wenn die Nutzung der Dienste keinen
  wesentlichen Teil eines Onlineangebots darstellt. Beispiel für keinen
  wesentlichen Teil: Anfahrtsskizzen auf Websites.
* Webseiten mit hohem Trafficaufkommen dürfen unsere Services grundsätzlich
  nicht nutzen.
* Das massenhafte Herunterladen von Daten ist verboten.

## Zusätzliche Bedingungen für die Nutzung der Tileserver (tile.openstreetmap.de)

* **Die Tiles müssen lokal so lange zwischengespeichert werden**, wie es die
  HTTP-Kopfzeile "Expires:" angibt. Alternativ muss diese Zeit mindestens
  sieben Tage betragen.
* **No-Cache-HTTP-Header dürfen nicht gesendet werden** (`Cache-Control:
  no-cache`, `Pragma: no-cache` usw.).
* Die Nutzung in Apps, die selbständig Tiles von tile.openstreetmap.de laden,
  ist ohne vorherige Zustimmmung des Betreibers untersagt. Für Alternativen sei
  auf die folgenden Abschnitte dieser Nutzungsbedingungen verwiesen.
* Das Herunterladen von Tiles größerer Gebiete (z.B. zur Offline-Nutzung) ist
  untersagt.
* Die Tiles von tile.openstreetmap.de unterliegen der Lizenz CC-BY-SA 2.0.

## Zusätzliche Bedingungen für die Nutzung der Routingserver (routing.openstreetmap.de, valhalla1.openstreetmap.de)

* Maximal eine Anfrage pro Sekunde.

## Datenschutz

Informationen zum Datenschutz finden Sie in der
[Datenschutzerklärung des FOSSGIS e.V.](https://www.fossgis.de/datenschutzerkl%C3%A4rung/)

## Änderungen dieser Nutzungsbedingungen und Verfügbarkeit

Wir behalten uns vor, Dienste jederzeit ohne Angabe von Gründen oder eine
Vorankündigung einzustellen. Änderungen der Nutzungsbedingungen sind ebenfalls
ohne Vorankündigung möglich.

Wir weisen darauf hin, dass die Nutzungserlaubnis der Services unsererseits
jederzeit ohne Angabe von Gründen widerrufen werden kann. Dies ist insbesondere
bei Regelverstößen und missbräuchlicher Nutzung der Fall.

Bitte bedenken Sie, dass hinter den Services jeweils nur ein einziger Server
steht. Wir garantieren keine Verfügbarkeit.

## Alternative Anbieter

* [Liste anderer Tileserver](https://wiki.openstreetmap.org/wiki/TMS)
* [Dienstleister und kommerzieller Support](https://wiki.openstreetmap.org/wiki/Commercial_OSM_Software_and_Services)
* [Anleitung zur Installation eigener Tileserver](http://switch2osm.org/)
* [Anleitung zur Installation von OSRM](https://github.com/Project-OSRM/osrm-backend/wiki)
* [Anleitung zur Installation von Valhalla](https://github.com/valhalla/valhalla)

## Kontakt

Zum [Impressum](https://www.fossgis.de/impressum.html) des FOSSGIS e.V.

Für Fragen wenden Sie sich bitte an info@fossgis.de.
