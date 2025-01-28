---
title: "Hackweekend Berlin November 2024"
date: "2024-11-04T11:00:00+02:00"
author: "Lars Lingner"
description: Das Hackweekend 2024 in Berlin brachte die OpenStreetMap-Community für ein inspirierendes Wochenende zusammen.
images:
  - /news/images/2024-11-04_Hack_Berlin_2024.jpg
categories:
- fossgis
- openstreetmap
---

## Kreatives Tüfteln der OpenStreetMap-Community

Das Hackweekend 2024 in Berlin brachte die OpenStreetMap-Community für ein inspirierendes Wochenende zusammen. Über 20 Teilnehmende aus ganz Deutschland fanden sich ein – neben den zahlreichen Gästen aus Berlin und Brandenburg reisten auch Community-Mitglieder aus Nordrhein-Westfalen, Baden-Württemberg, Sachsen und Sachsen-Anhalt an. Die Veranstaltung bot einen Raum, um Ideen auszutauschen, kreative Projekte voranzutreiben und gemeinsam an neuen Entwicklungen zu arbeiten. 

Im Fokus standen nicht nur technische Herausforderungen und Detailfragen, sondern auch Projekte mit sozialem Mehrwert. Diese vielfältigen Ansätze und Themen sorgten dafür, dass das Wochenende eine lebendige Mischung aus Innovation und praktischen Anwendungen bot, die die Community bereichern und inspirieren.

Für alle, die noch nie an einem Hackweekend teilgenommen haben, bietet ein solches Event die perfekte Gelegenheit, die OSM-Community kennenzulernen und selbst aktiv zu werden. Egal ob Du bereits technisch versiert bist oder einfach neugierig auf die Welt der offenen Kartographie – hier findest Du Gleichgesinnte, die ihre Erfahrungen teilen und Dich unterstützen. Gemeinsam zu arbeiten, neue Ideen umzusetzen und Projekte voranzutreiben, macht unglaublich viel Spaß und gibt Dir die Möglichkeit, Deine eigenen Fähigkeiten weiterzuentwickeln.

Ein besonderer Dank gilt [Wikimedia Deutschland](https://www.wikimedia.de/), die nicht nur die Räumlichkeiten zur Verfügung stellte, sondern uns auch mit engagierter Betreuung und Verpflegung unterstützte. Durch ihre [Förderung](https://de.wikipedia.org/wiki/Wikipedia:F%C3%B6rderung/Wikimedia_Deutschland) entstanden den Teilnehmenden keinerlei Kosten, was das Event für alle offen und zugänglich machte. 

Falls Du also überlegst, nächstes Mal dabei zu sein: Trau Dich! Das Hackweekend ist eine großartige Chance, ein Teil dieser offenen und kreativen Gemeinschaft zu werden, wertvolle Erfahrungen zu sammeln und das OpenStreetMap-Projekt mitzugestalten. Die zukünftigen Termine werden wie üblich im [OSM-Kalender](https://osmcal.org/?in=Germany) und im [Wiki](https://wiki.openstreetmap.org/wiki/Berlin/Veranstaltungen#Hackweekends) veröffentlicht.

Einen kleinen Einblick geben die folgenden Berichte der Teilnehmenden:

---

### Neue Ideen für den Verkehrswende-Bereich von [tordans](https://www.openstreetmap.org/user/tordans)

Tobias nutzte das Hackweekend, um sich zu verschiedenen Themen rund um das Thema Verkehrswende mit OpenStreetMap auszutauschen:

- Austausch zur Weiterentwicklung des [Verkehrszeichentools](https://trafficsigns.osm-verkehrswende.org/DE)
- Feedbackrunde: Disskusion über neue Logos für die Berlin-Brandenburg-Community (Veröffentlichung folgt in Kürze) und andere verkehrsbezogene Projekte.
- Austausch zu [ODbL](https://wiki.openstreetmap.org/wiki/DE:Open_Database_License)
- Austausch zu [iD](https://wiki.openstreetmap.org/wiki/ID)

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_traffic_tool.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
*Screenshot des Traffic Sign Tool*

---

### Hartmut: [maposmatic](https://print.get-map.org/new/)-vagrant und Mapnik-Themen

- Fehlerbehebung im Provisioning und Aktualisierung des OSM Carto-Stil auf die neueste [Version 5.9](https://github.com/gravitystorm/openstreetmap-carto/releases/tag/v5.9.0)
- lokale Umap-Testinstanz hinzugefügt (WiP)
- [Baumkarte](https://obstbaumkarte.de/)-Stil auf “latest” aktualisert
- Shapefile Installation parallelisiert
- Mapnik - The Missing Manual: https://get-map.org/mapnik-lost-manual/

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_printmap.png" width="1000" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
*Webseite print.get-map.org*

---
### dcz: CartoCSS QGIS Plugin

dcz präsentierte sein **CartoCSS QGIS Plugin** und diskutierte die Möglichkeiten der Nutzung von CartoCSS in [QGIS](https://qgis.org/) für gedruckte Karten. Der Austausch war inspirierend, auch wenn die technische Umsetzung eine Herausforderung bleibt. Im OSM-Forum wurde eine [Disskusion](https://community.openstreetmap.org/t/cartocss-with-qgis-for-printing/121036/5) gestartet.

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_qgis_cartocss.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}    
*Screenshot QGIS-Plugin CartoCss Editor*

---
### Erfahrungsbericht Marcus

Dieses Wochenende habe ich ein neues Projekt gestartet: Mein Ziel ist eine Anwendung, die aus einem GPX-Track und einem Ort einen Wanderplan erzeugt. Der Plan soll so sein, dass jeden Tag ein Stück des Track gewandert werden kann und Abends ein Bus oder Zug zur Verfügung steht, der zu dem Startort zurück führt.

Dieses Hackweekend haben ich nach einen Router für Bus und Bahn gesucht. Angeschaut habe ich mir die [DB-Apis](https://developers.deutschebahn.com/db-api-marketplace/apis/), [öffentliche ÖPNV-Daten](https://www.opendata-oepnv.de), besonders die API des [Verkehrsverbund Rhein-Ruhr](https://www.vrr.de/de/fahrplan-mobilitaet/fahrplanauskunft/app/trip?lng=de&trip=multiModalitySelected%3Dpt). Auf öffenlichen ÖPNV-Daten können der [gtfsrouter](https://urbananalyst.github.io/gtfsrouter/) und der [OpenTripPlaner](https://www.opentripplanner.org/) routen. Überrascht war ich, dass es bei der DB keine Verbindungsdaten - also wie komme ich von A nach B - gibt sondern nur Fahrplandaten.

Zum Glück bin ich am Sonntag (wieder) auf den [public-transport-enabler](https://github.com/schildbach/public-transport-enabler) von Andreas Schildbach gestoßen. Der scheint mir, die beste API für meine Zwecke zu sein. Besonders erfreulich ist, dass sich auch die API des Verkehrsverbund Rhein-Ruhr nutzen lässt.

---
### Erfahrungsbericht: JOSM, StreetComplete von [Pintoch](https://wiki.openstreetmap.org/wiki/User:Pintoch)

Ich habe versucht zu untersuchen, wie schwierig es sein kann, Beiträge zu FOSS-Projekten in der OSM Community zu machen. Das mache ich im Rahmen von einem größeren Projekt: "contribution experience reports" für viele FOSS Projekte zu schreiben. Ich habe zum Beispiel schon [eins für OrganicMaps](https://antonin.delpeuch.eu/posts/contribution-experience-report-organic-maps/) geschrieben.

Ich habe zuerst versucht, eine Pull Request zu StreetComplete zu machen. Die meisten offenen Issues fand ich unpassend: entweder kümmert sich schon jemand darum, oder gibt es kein klarer Design-Vorschlag auf dem Leuten einig sind, oder der Hauptentwickler sieht nicht richtig überzeugt aus, von der vorgeschlagenen Änderung.

Dann habe ich versucht, was bei JOSM beizutragen. Das war ein sehr interessantes Erlebnis, welches ich wahrscheinlich in einem separaten Blogeintrag beschreiben werde.

---
### Fehlende Stolpersteine in Berlin

[Joe](https://github.com/hejjoe) und [Christian](https://chrpaul.de) versuchen mehr Stolpersteine in Berlin zu erfassen. An diesem Wochenende haben wir Karten pro Kiez erstellt, damit lokale  Mapper fehlende Stolpersteine leichter finden können. Unsere GPX-Dateien enhalten nur Punkte, an denen auf OSM kein Stolperstein zu finden ist.
Der Datensatz kommt von der [Koordinierungsstelle Stolpersteine Berlin](https://www.stolpersteine-berlin.de/).

- Ein [Pull Request](https://github.com/pietervdvn/MapComplete/pull/2235) an MapComplete: (inkl [credit ans event](https://github.com/pietervdvn/MapComplete/pull/2235/files#diff-fdc7543839c3a1b3aa6209534f76dd5257384d1bc0b00663e8055cc29354c3f9R116))
- GPX-Dateien pro Kiez zum Ablaufen als [Download](https://osm-check.chrpaul.de/report/stolpersteine-berlin-complete-by-kiez/) 
- Quelltext: https://gitlab.com/jaller94/osm-check-scripts
- [Matrix-Raum](https://matrix.to/#/!iFPOuQBbUgHKXwzdKk:matrix.org?via=matrix.org&via=systemli.org) zur Kommunikation: 

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_stolpersteine.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}    
*Punkte auf einer Karte Kreuzbergs zeigen fehlende Stolpersteine*

---
### MapSCII: Eine Braille-Karte der Welt

[Christian](https://chrpaul.de) hat die Konsolenanwendung [MapSCII](https://github.com/rastapasta/mapscii) von JavaScript nach TypeScript übersetzt und die Abhängigkeiten auf den neusten Stand gebracht. Für ein neues Release ist der Entwicklungs-Branch leider noch zu instabil. Der Code ist in einem neuen [Branch](https://github.com/rastapasta/mapscii/pull/151)

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_mapscii.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}    
*Bildschirmfoto von MapSCII, welches eine bunte Weltkarte mit Braille-Zeichen darstellt*

---
### Karten auf E-Paper-Displays

Mit neuen E-Paper-Displays für digitale Karten ging Christian einen Schritt in Richtung moderne Kartentechnologie:

1. Erstellung eines kontrastreichen OSM-Bilds.
2. Anpassung an die Farbpalette eines 7-Farb-Displays.
3. Übertragung des Bildes auf ein Display mithilfe eines ESP32.

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_epaper.jpg" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}    
*Foto des OSM-Bilds auf einem E-Paper-Display*


1. Bildschirm-Foto von OSM erstellen.
2. Kontraste erhöhen und die Farbpalette des Bildschirms (7 Farben) anwenden.
3. PNG in einen Byte-Array in C++ umwandeln.
4. Code auf einen ESP32 übertragen.
5. Der ESP32 überträgt das Bild über GIPO-Pins auf den E-Paper-Bildschirm.

Hardware:
* [7.3inch ACeP 7-Color E-Paper E-Ink Display Module, 800×480 Pixels](https://www.waveshare.com/7.3inch-e-paper-hat-f.htm) (aktuell ca. 80 €)
* [Universal e-Paper Raw Panel Driver Board, ESP32 WiFi / Bluetooth](https://www.waveshare.com/e-paper-esp32-driver-board.htm) (ca. 15 €)

---
### Voronoi-Flächen für Straßenzüge von [Supaplex030](https://www.openstreetmap.org/user/Supaplex030)

Daten unseres Crowdmap-Experiments zur Prüfung von OSM-Gebäudedaten in Berlin (https://www.osm-verkehrswende.org/crowdmap/) so aufbereitet, dass wir eine [Challenge](https://tasks.openstreetmap.us/projects/704/) zur Aktualisierung von Gebäuden/Baustellen in Berlin starten können

Mit QGIS einen Prototypen erstellt, um “lückenlose” Flächen um  Straßenzüge herum zu erstellen (Voronoi-Flächen). Damit lässt sich  kleinräumig (pro Straßenzug/-segment) nach quantitativen Unterschieden  zwischen verschiedenen Datensätzen suchen:

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_voronoi.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
*Abb.: Voronoi-Flächen für einzelne Straßenzüge, dargestellt nach  quantitativen Unterschieden zwischen OSM-Parkraumdaten und Parkraumdaten der Berliner Senatsverwaltung – wo gibt es signifikante Abweichungen  der Parkplatzanzahl? Teils liegt der Fehler in den Senats-Daten  begründet, teils in OSM – dort kann man die Daten dann bei Bedarf  verbessern.*

Ein paar Gedanken dazu gemacht, wie man mit OSM-Diffs ([Geofabrik](https://download.geofabrik.de/)) ein Monitoring spezieller Änderungen in OSM umsetzen könnte (alles, was  z.B. über [OSMCha](https://osmcha.org/) hinausgeht: z.B. Gib mir alle Changesets, in denen ein User/User XY  Objekte mit bestimmten Tags gelöscht hat, Gib mir alle Changesets, in  denen jemand die Länge einer Linie mit Tags wie “parking:…” verändert  hat etc.)

---

### MapCSS-Styling für Overpass Turbo von [Martin](https://wiki.openstreetmap.org/wiki/User:Tyr)

Overpass turbo hat jetzt einen Wizard für MapCSS styling:

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_overpassturbo_1.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
<a href="https://overpass-turbo.eu/s/1TB8"><img src="/news/images/2024-11-04_hackweekend_overpassturbo_2.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
*Screenshot of the dialog of the new auto styler dialog in overpass turbo* 

Mehr dazu in meinem osm diary: https://www.openstreetmap.org/user/tyr_asd/diary/405486

---
### Suche nach Wikimedia Links in OpenStreetMap (Wolfram)

Die Wikipedia und ihre Schwesterprojekte haben oft Geokoordinaten in ihren Artikeln. Leider sind die Artikel nicht immer erfasst in OpenStreetMap. Ich habe die BBBike tagname Suchmaschine erweitert, dass man nicht nur nach URLs,  sondern auch nach Referenzen zu Wikipedia, Wikidata und Wikimedia Commons suchen kann.
https://search.bbbike.org/

Beispiele:

1) Suche nach allen Stolpersteinen mit Foto bei Wikimedia Commons in Berlin, die in OSM eingetragen sind:   
https://search.bbbike.org/?query=File%3AStolperstein&hits=2000&area=berlin

2) Suche nach (Fotos) von Wasserpumpen in Berlin:   
https://search.bbbike.org/?query=Wasserpumpe&area=berlin

3) Suche nach Nodes, Ways, Relations in Deutschland, die auf den Wikipedia Artikel von "Willy Brandt" verlinken:   
https://search.bbbike.org/?query=de%3AWilly+Brandt&hits=20&area=germany

{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_osmsuche.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
*Suche nach Referenzen zu Wikipedia, Wikidata und Wikimedia Commons* 

---
### Datenverbesserungen

Während des Hackweekends wurden von den Gästen auch das Umfeld bzw. der Anreiseweg in OSM vervollständigt. Direkt im Kiez des Wikimedia-Büros konnten noch Straßenlaternen ([Laternenkarte](https://sb12.github.io/OSMStreetLight/#17/52.49730/13.38244)) und Hydranten ([OSMhydrant.org](https://www.osmhydrant.org/de/#zoom=17&lat=52.497132&lon=13.38142)) nachgetragen werden. 


{{< rawhtml >}}
<a><img src="/news/images/2024-11-04_hackweekend_osmstreetlamps.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
<a><img src="/news/images/2024-11-04_hackweekend_osmhydrant.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}    
*Straßenlampen und Hydranten in OSM*   

---
### Mapillary-Tools zum Kopieren und aussortieren (Christopher)

Meine Tools etwas vorzeigbar gemacht (erste Version) zum Kopieren von Fotos  von der Kamera sortiert nach Datum und Aussortieren von Doppelten Fotos  z.B. an der Ampel und Fotos ohne GPS um diese ggf. mit einem separaten  Track mit Geokoordinaten zu versehen.
 https://github.com/britiger/mapillary_gopro_tools

---
### FOSSGIS-Vereins-Arbeit (Christopher)

- Vorbereitungen für die [FOSSGIS-Konfrenz 2025](https://fossgis-konferenz.de/2025/)
- Erstellung des Zeitrasters für die Programmgestaltung
- Werbung und Review von bereits eingereichten Vorträgen

---
{{< rawhtml >}}
<img src="/news/images/2024-11-04_Hack_Berlin_2024.jpg" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}  
*Gruppenfoto Hackevent Berlin November 2024*
