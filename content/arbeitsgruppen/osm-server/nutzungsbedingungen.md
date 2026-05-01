---
title: "Nutzungsbedingungen OSM-Server des FOSSGIS e.V."
---

English see below.
## Deutsche Version

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

### Geltungsbereich

Diese Nutzungsbedingungen gelten für
* die Tileserver des FOSSGIS e.V. (tile.openstreetmap.de).
* die Routingserver des FOSSGIS e.V. (routing.openstreetmap.de, valhalla1.openstreetmap.de)
* die Overpass-Server des FOSSGIS e.V. (overpass-api.de)
* die umap-Server des FOSSGIS e.V. (umap.openstreetamp.de)

Sie gelten nicht für die umap-, Overpass-, Routing- oder Tileserver anderer Betreiber (z.B.
tile.openstreeetmap.org der OpenStreetMap Foundation und diverse gewerbliche
Anbieter) und auch nicht für die Nutzung der OpenStreetMap-Rohdaten. Die
Nutzung der OpenStreetMap-Daten unterliegt den Bedingungen der Open Database
License 1.0.

### Allgemeine Regeln

#### Voraussetzungen

* Klare Anzeige der Quellenangabe, wie sie von der Lizenz und der
  OpenStreetMap Foundation
  [verlangt](https://www.openstreetmap.org/copyright) wird.
* Ergänzen Sie einen Link zu
  [https://www.openstreetmap.org/fixthemap](https://www.openstreetmap.org/fixthemap),
  um Ihren Nutzern zu erlauben, Fehler in unseren Daten zu melden und zu beheben.
  Der folgende HTML-Code erfüllt diese Regeln:

```html
  Daten © <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>-Mitwirkende
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

#### Technische Nutzungsvoraussetzungen

* **Gültiger HTTP-User-Agent**, der die Anwendung identfiziert. Die User-Agents
  von Bibliotheken sind nicht ausreichend. Das Vortäuschen einer anderen Anwendung
  führt sicher zur Sperrung.
* Eine gültige Angabe der Ursprungsseite (HTTP-Referrer) sofern dies
  technisch möglich ist.
* **Maximal zwei herunterladende Verbindungen.** (Die unmodifizierten
  Einstellungen der üblichen Website-Betrachter sind akzeptabel.)
  **Skripte** sind auf eine Verbindung zu beschränken.

Anmerkung: Übliche Web-Browser ohne modifizierte Konfiguration halten
normalerweise alle der oben stehenden technischen Nutzungsvoraussetzungen ein.

#### Nicht erlaubte Nutzungen

* Die gewerbliche Nutzung ist nur gestattet, wenn die Nutzung der Dienste keinen
  wesentlichen Teil eines Onlineangebots darstellt. Beispiel für keinen
  wesentlichen Teil: Anfahrtsskizzen auf Websites.
* Webseiten mit hohem Trafficaufkommen dürfen unsere Services grundsätzlich
  nicht nutzen.
* Das massenhafte Herunterladen von Daten ist verboten.

### Zusätzliche Bedingungen für die Nutzung der Tileserver (tile.openstreetmap.de)

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

### Zusätzliche Bedingungen für die Nutzung der Routingserver (routing.openstreetmap.de, valhalla1.openstreetmap.de)

* Maximal eine Anfrage pro Sekunde.

### Datenschutz

Informationen zum Datenschutz finden Sie in der
[Datenschutzerklärung des FOSSGIS e.V.](https://www.fossgis.de/datenschutzerkl%C3%A4rung/)

### Änderungen dieser Nutzungsbedingungen und Verfügbarkeit

Wir behalten uns vor, Dienste jederzeit ohne Angabe von Gründen oder eine
Vorankündigung einzustellen. Änderungen der Nutzungsbedingungen sind ebenfalls
ohne Vorankündigung möglich.

Wir weisen darauf hin, dass die Nutzungserlaubnis der Services unsererseits
jederzeit ohne Angabe von Gründen widerrufen werden kann. Dies ist insbesondere
bei Regelverstößen und missbräuchlicher Nutzung der Fall.

Bitte bedenken Sie, dass hinter den Services jeweils nur ein einziger Server
steht. Wir garantieren keine Verfügbarkeit.

### Alternative Anbieter

* [Liste anderer Tileserver](https://wiki.openstreetmap.org/wiki/TMS)
* [Dienstleister und kommerzieller Support](https://wiki.openstreetmap.org/wiki/Commercial_OSM_Software_and_Services)
* [Anleitung zur Installation eigener Tileserver](https://switch2osm.org/)
* [Anleitung zur Installation von OSRM](https://github.com/Project-OSRM/osrm-backend/wiki)
* [Anleitung zur Installation von Valhalla](https://github.com/valhalla/valhalla)

### Kontakt

Zum [Impressum](https://www.fossgis.de/impressum.html) des FOSSGIS e.V.

Für Fragen wenden Sie sich bitte an info@fossgis.de.




## English version

The services operated by FOSSGIS e.V. are run by volunteers using donated funds. Their primary purpose is to support usage on our website and to assist OpenStreetMap contributors in their work. We are generally pleased when third parties use our services for creative and innovative applications. However, excessive use restricts usability. Therefore, we require that all users of FOSSGIS e.V. services comply with these terms of use.

**OpenStreetMap data can be [used freely and at no cost by anyone](https://www.openstreetmap.org/copyright). Our services, however, cannot.**

The following are the minimum requirements that users must meet.

Many other organizations provide similar services based on OpenStreetMap data. If your project does not meet the requirements here, you may obtain the same from other providers (see below).

### Scope

These terms of use apply to:
- the FOSSGIS e.V. tile servers (tile.openstreetmap.de)
- the FOSSGIS e.V. routing servers (routing.openstreetmap.de, valhalla1.openstreetmap.de)
- the FOSSGIS e.V. Overpass servers (overpass-api.de)
- the FOSSGIS e.V. umap servers (umap.openstreetmap.de)

They do not apply to umap, Overpass, routing, or tile servers operated by other parties (e.g., tile.openstreetmap.org of the OpenStreetMap Foundation and various commercial providers), nor do they apply to the use of raw OpenStreetMap data. The use of OpenStreetMap data is subject to the terms of the Open Database License 1.0.

### General Rules

#### Requirements

- Clear display of attribution as required by the license and the OpenStreetMap Foundation [guidelines](https://www.openstreetmap.org/copyright).
- Include a link to [https://www.openstreetmap.org/fixthemap](https://www.openstreetmap.org/fixthemap) to allow your users to report and correct errors in our data. The following HTML code satisfies these rules:

```html
  Data © <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors
  (<a href="https://opendatacommons.org/licenses/odbl/index.html">ODbL</a>), <a
  href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, <a
  href="https://openstreetmap.org/fixthemap">contribute/report error</a>
```

  For media where links are technically not possible, `Data: © OpenStreetMap contributors (ODbL), Graphics: CC-BY-SA` is sufficient.
- For websites, an email address of the operator must be easily identifiable and directly reachable in order to contact them if necessary. For apps, this applies to the app website and its entries in app stores.
- Explicitly recommended: The URLs of our services should not be hardcoded into the app.

#### Technical Usage Requirements

- **Valid HTTP User-Agent** identifying the application. User agents of libraries are not sufficient. Impersonating another application will result in immediate blocking.
- A valid origin indication (HTTP Referrer) where technically possible.
- **Maximum two downloading connections.** (Unmodified settings of standard web browsers are acceptable.) **Scripts** are limited to one connection.

Note: Standard web browsers without modified configuration normally comply with all of the above technical usage requirements.

#### Prohibited Uses

- Commercial use is only permitted if the use of the services does not constitute a substantial part of an online offering. Example of a non-substantial part: Directions sketches on websites.
- Websites with high traffic volumes are generally not permitted to use our services.
- Mass downloading of data is prohibited.

### Additional Conditions for Use of the Tile Servers (tile.openstreetmap.de)

- **Tiles must be cached locally** for as long as indicated by the HTTP header "Expires:". Alternatively, this time must be at least seven days.
- **No-Cache HTTP headers must not be sent** (`Cache-Control: no-cache`, `Pragma: no-cache`, etc.).
- Use in apps that independently load tiles from tile.openstreetmap.de is prohibited without prior consent from the operator. For alternatives, please refer to the following sections of these terms of use.
- Downloading tiles of larger areas (e.g., for offline use) is prohibited.
- The tiles from tile.openstreetmap.de are licensed under CC-BY-SA 2.0.

### Additional Conditions for Use of the Routing Servers (routing.openstreetmap.de, valhalla1.openstreetmap.de)

- Maximum one request per second.

### Privacy

For information on privacy, please refer to the [FOSSGIS e.V. Privacy Policy](https://www.fossgis.de/datenschutzerkl%C3%A4rung/).

### Changes to These Terms of Use and Availability

We reserve the right to discontinue services at any time without stating reasons or providing advance notice. Changes to the terms of use are also possible without advance notice.

We note that permission to use the services may be revoked by us at any time without stating reasons. This applies in particular in cases of rule violations and abusive use of the services.

Please note that each service is backed by only a single server. We do not guarantee availability.

### Alternative Providers

- [List of other tile servers](https://wiki.openstreetmap.org/wiki/TMS)
- [Service providers and commercial support](https://wiki.openstreetmap.org/wiki/Commercial_OSM_Software_and_Services)
- [Guide to installing your own tile servers](https://switch2osm.org/)
- [Guide to installing OSRM](https://github.com/Project-OSRM/osrm-backend/wiki)
- [Guide to installing Valhalla](https://github.com/valhalla/valhalla)

### Contact

See the [Imprint](https://www.fossgis.de/impressum.html) of FOSSGIS e.V.

For questions, please contact info@fossgis.de.
