---
title: "Hackweekend Berlin April 2026"
date: "2026-04-17T11:00:00+02:00"
author: "Lars Lingner"
description: Das Hackweekend im April 2026 in Berlin brachte die OpenStreetMap Community zusammen, um an Tools, Renderern, Datenworkflows und Mapping Projekten zu arbeiten.
images:
  - /news/images/2026-04-17_hackweekend_berlin_platzmonitor.png
categories:
  - fossgis
  - openstreetmap
---

## Gemeinsam hacken, mappen und Ideen teilen

Beim Hackweekend Berlin 04/2026 kommt die OpenStreetMap Community zusammen, um in entspannter Atmosphäre gemeinsam an Ideen zu arbeiten. Ein Hackweekend ist kein reiner Programmier Marathon. Es ist ein offenes Treffen, bei dem neue und erfahrene Leute zusammenkommen, sich gegenseitig helfen und am Ende konkrete Verbesserungen mitnehmen.

Wir danken Wikimedia Deutschland herzlich für die erneute Gastfreundschaft: für die Räume, die gute Arbeitsatmosphäre und die tolle Verpflegung.

Die Beispiele aus diesem Wochenende zeigen die Bandbreite sehr gut. Es ging um kleine, nützliche Tools für Events wie Platzmonitor oder Abfahrtsmonitor, um Daten und Darstellung wie externe WMS Layer in BBBike oder einen Rust Renderer im Browser, und genauso um Austausch und Mapping Themen rund um Micromapping und Strassenraumdetails. Du kannst an deinem eigenen Projekt weiterarbeiten, dich an etwas dranhängen oder einfach erst mal zuschauen und Fragen stellen.

Wenn du neu dabei bist, reicht oft schon ein Laptop und Neugier. Du kannst aber auch ganz ohne Technik mitmachen, zum Beispiel beim Mapping, Testen, Dokumentieren oder einfach im Austausch. Hilfreich sind ein OSM Account und, je nach Themengebiet, Smartphone oder Kamera, aber notwendig ist das nicht. Vor Ort gibt es kein festes Programm, stattdessen entstehen spontan Aufgaben und Mini Sessions, und jemand findet sich fast immer, um dich beim Einstieg zu unterstützen.

Wenn du die naechsten Termine nicht verpassen willst, beobachte die verlinkte Wiki Seite oder [osmcal.org](https://osmcal.org/).

Das nächste Hackweekend in Berlin wird am [24. und 25. Oktober 2026](https://wiki.openstreetmap.org/wiki/Berlin_Hack_Weekend_Oktober_2026) stattfinden.

Im Folgenden sind einige der Themen gesammelt, an denen gearbeitet wurde.

---

## Lars: Platzmonitor und Fahrplan Druck

- [github.com/gislars/platzmonitor](https://github.com/gislars/platzmonitor) erstellt, um freie Plätze für Workshops und Exkursionen auf der FOSSGIS Konferenz anzuzeigen

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_platzmonitor.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

- [github.com/gislars/fossgis-fahrplan-druck](https://github.com/gislars/fossgis-fahrplan-druck) kleinere Änderungen, unter anderem in `config.js` ausgelagert
- Mobile Version mit Favourite Funktion: [gislars.github.io](https://gislars.github.io/fossgis-fahrplan-druck/events/fossgis2026/?columns=mobile)

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_fossgis_fahrplan_druck_mobile.png" width="500" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Christopher: Abfahrtsmonitor für die FOSSGIS Konferenz

Abfahrtsmonitor für die FOSSGIS Konferenz:

- [github.com/britiger/fossgis-abfahrtsmonitor](https://github.com/britiger/fossgis-abfahrtsmonitor/tree/cl_c3tofossgis)

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_abfahrtsmonitor.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Christian (Jaller): Kassenbondrucker und MapSCII

Wir hatten einen Kassenbondrucker vor Ort und natürlich haben wir darauf Karten gedruckt:

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_kassenbondrucker.jpg" width="600" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

### MapSCII

[MapSCII](https://github.com/rastapasta/mapscii) ist ein Braille und ASCII Renderer für das Terminal. Ein grosser Wunsch ist es, aktuelle Karten in MapSCII anzuzeigen. Der offizielle Server hat einen Kartenstand aus 2016 ohne Chance auf Updates von der ursprünglichen Quelle.

Dank [Pull Request 155 von ionmeo](https://github.com/rastapasta/mapscii/pull/155) gibt es nun die Option, auf einen topaktuellen Datensatz von OpenFreeMap umzusteigen. Der Pull Request wurde an dem Wochenende gelesen und freigegeben. Ein weiteres Ziel war es, den Quellcode nach TypeScript zu übersetzen.

Aktionsplan für ein neues Release:

- [github.com/rastapasta/mapscii issue 159](https://github.com/rastapasta/mapscii/issues/159)

---

## Murphy (StrangeGirlMurph): Mapping und Diskussionen

- Kleistpark weiter gemappt
- Fahrradwege in der Kolonnenstrasse hinzugefügt
- Fotogrammetrie diskutiert

---

## Wolfram: BBBike Map Compare mit externen WMS

[BBBike Map Compare](https://mc.bbbike.org/mc/) ist ein spezialisiertes Kartentool, mit dem man verschiedene Online Karten direkt miteinander vergleichen kann.

Neu ist auch die Einbindung externer WMS Services. In der [Admin Console](https://mc.bbbike.org/mc/console.html) lassen sich zum Beispiel Karten aus Geoportalen einbinden und neben oder über eine OpenStreetMap Karte legen. Das funktioniert mit allen gängigen WMS Servern.

{{< rawhtml >}}

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-bottom: 20px;">
<div>
<a><img src="/news/images/2026-04-17_hackweekend_berlin_bbbike_wms_1.png" width="400" style="border: 1px solid #808080; border-radius: 3px;"/></a>
</div>
<div>
<a><img src="/news/images/2026-04-17_hackweekend_berlin_bbbike_wms_2.png" width="400" style="border: 1px solid #808080; border-radius: 3px;"/></a>
</div>
</div>
{{< /rawhtml >}}

---

## Oliver: Geldautomaten Layer in der Obstbaumkarte

Geldautomatenlayer in [obstbaumkarte](https://obstbaumkarte.de/ml) eingebaut, auch zur weiteren Verwendung als Vektortile Layer in [geldautomaten-suche.org](https://geldautomaten-suche.org/).

Dazu wurden mittels [osm2pgsql](https://osm2pgsql.org/) zwei Postgis-Tabellen mit Geldautomaten und Geschäften, bei denen Bargeldauszahlungen vom Bankkonto möglich sind, [angelegt](https://github.com/rudzick/Myosm2pgsql-themepark/blob/eede7782473f27b637fc74580da9dc2f3104289d/themes/shortbread_v1/topics/atm.lua). Für die Geldautomaten werden die OSM-Tags [amenity=atm](https://wiki.openstreetmap.org/wiki/DE:Tag:amenity%3Datm) und [atm](https://wiki.openstreetmap.org/wiki/DE:Tag:atm%3Dyes) ausgewertet. Für die Geschäfte wird der Key [cash_withdrawal](https://wiki.openstreetmap.org/wiki/DE:Key:cash_withdrawal) ausgewertet; außerdem wird über die Keys [brand](https://wiki.openstreetmap.org/wiki/DE:Key:brand) und [operator](https://wiki.openstreetmap.org/wiki/DE:Key:operator) festgestellt, ob das Geschäft zu einer Kette gehört, die Barabhebungen in ihren Filialen ermöglicht.  Über eine [Postgis-Abfrage](https://github.com/rudzick/Myosm2pgsql-themepark/blob/eede7782473f27b637fc74580da9dc2f3104289d/Server_Update/views_for_atm.sql) werden Polygone herausgefiltert, die als Möglichkeit zum Bargeldabheben getaggt sind und zuzätzlich Geldautomaten oder entsprechende Geschäfte als Nodes enthalten. Das Ergebnis dieser Postgis-Abfragen wird als Mapbox-Vektotiles ausgeliefert und kann als Layer in andere Karten eingebunden werden. Auf diese Weise werden die Daten zu Bargeldabhebemöglichkeiten zusammen mit den Kacheln der Hingrundkarte in den Client geladen, so dass sich eine Abfrage über die Overpass-API erübrigt. Der Vorteil dieser Vorgehensweise ist, dass auch Informationen für große Gebiete angezeigt werden können. So lassen sich Geldautomaten und Geschäfte auch auf niedriegeren Zoomstufen darstellen (hier ein [Beispiel für Zoomlevel 9](https://obstbaumkarte.de/ml/#9/52.8767/13.5103) ). Ein nächster Schritt könnte z.B. sein, clientseitig durch Auswertung der Öffnungszeiten tageszeitabhängig zu filtern, so dass nur die Automaten und Geschäfte angezeigt werden, bei denen man zum Zeitpunkt des Aufrufs der Karte tatsächlich Geld abheben kann. 

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_obstbaumkarte_geldautomaten_z9.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Sven: Rust Renderer für area:highway im Browser

Experimenteller Rust basierter Renderer für `area:highway` und `barrier=kerb`, der per WebAssembly direkt im Browser läuft:

- [github.com/svenpilz/highway_area_map](https://github.com/svenpilz/highway_area_map)

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_highway_area_map.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Slaven: BBBike Optimierung, Converter und Bugfixes

- Fahrradstrassen Optimierung in BBBike, zunächst nur in der Desktop Anwendung, am Beispiel Bundesallee vs Handjerystraesse plus Prinzregentenstrasse
- Mapillary Vector Tiles nach BBBike Datenformat Converter
- Bugfixes
- Nominatim Issue zu problematischen neighbourhood und quarter Angaben in den Ergebnissen angestossen

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_bbbike_fahrradstrassen.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Alex: Austausch, QGIS Rendering und Modernisierung der Prozessierung

- Viel Austausch zu Micromapping, Mapping von Strassenraumdetails und Diskussionen über Vibe Coding
- Experimente mit komplexen Rendering Reihenfolgen in QGIS, um Features auf oder unter Brücken abhängig ihres `layer` Taggings zu rendern. Die nächste Version der [Strassenraumkarte](https://strassenraumkarte.osm-berlin.org/?map=micromap) soll übereinander liegende Features besser darstellen.
- Modernisierung der Prozessierung der Strassenraumkarte auf einen osm2pgsql plus SQL Stack. Arbeit an der Generierung von Strassenmarkierungen ging weiter voran.

{{< rawhtml >}}
<a><img src="/news/images/2026-04-17_hackweekend_berlin_strassenraumkarte.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}
