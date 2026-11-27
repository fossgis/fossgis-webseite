---
title: "Hackweekend Berlin Oktober 2026"
date: "2026-10-30T11:00:00+01:00"
author: "Lars Lingner"
description: Beim Hackweekend im Oktober 2026 in Berlin arbeitete die OpenStreetMap Community an Karten, Tools und Datenworkflows und diskutierte über KI beim Programmieren rund um OSM.
images:
  - /news/images/2026-10-30_hackweekend_berlin_osm2stitch.png
categories:
  - fossgis
  - openstreetmap
---

## Gemeinsam hacken, mappen und diskutieren

Am 24. und 25. Oktober 2026 hat sich die OpenStreetMap Community wieder zum Hackweekend in Berlin getroffen. Mit 25 Teilnehmenden an beiden Tagen war es das bisher größte Hackweekend in Berlin. Ein Hackweekend ist kein reiner Programmier Marathon. Es ist ein offenes Treffen, bei dem neue und erfahrene Leute zusammenkommen, sich gegenseitig helfen und am Ende konkrete Verbesserungen mitnehmen.

Wir danken [Wikimedia Deutschland](https://www.wikimedia.de/) herzlich für die erneute Gastfreundschaft: für die Räume, die gute Arbeitsatmosphäre und die tolle Verpflegung.

Die Themen waren auch diesmal bunt gemischt. Es wurden Karten gestickt, LiDAR Scans zusammengepuzzelt, Quasi-Luftbilder aus 360° Straßenfotos erzeugt und Druckkarten um Seezeichen erweitert. Dazu kamen Verbesserungen an bekannten Diensten wie dem BBBike Extract Service, der Straßenraumkarte und der Obstbaumkarte. Ein Thema, das sich durch viele Gespräche zog, war die Frage, welche Rolle KI und Agentic Coding im OSM Umfeld spielen und spielen sollten.

Wenn du neu dabei bist, reicht oft schon ein Laptop und Neugier. Du kannst aber auch ganz ohne Technik mitmachen, zum Beispiel beim Mapping, Testen, Dokumentieren oder einfach im Austausch. Vor Ort gibt es kein festes Programm, stattdessen entstehen spontan Aufgaben und Mini Sessions, und jemand findet sich fast immer, um dich beim Einstieg zu unterstützen.

Weitere Informationen zum Event finden sich im [Wiki](https://wiki.openstreetmap.org/wiki/Berlin_Hack_Weekend_Oktober_2026). Wenn du die nächsten Termine nicht verpassen willst, beobachte [osmcal.org](https://osmcal.org/).

Im Folgenden sind einige der Themen gesammelt, an denen gearbeitet wurde.

---

## Christopher und Lars: Konferenz-Dashboards und Hackweekends 2027

Die Dashboards für die kommende FOSSGIS-Konferenz in Heidelberg haben sich Christopher und Lars gemeinsam nochmal angesehen und letzte Features hinzugefügt. Es wird eine Abfahrtstafel geben, die alle Fahrplanabweichungen gegenüber dem Programmheft anzeigt, und eine Anzeige, welche Workshops und Exkursionen noch freie Plätze haben. Jetzt warten wir auf die Veröffentlichung des Programms im Dezember 2026.

Auch 2027 soll es wieder zwei Hackweekends geben. Christopher und Lars haben zwei mögliche Termine gefunden, die müssen jetzt aber noch mit anderen Stellen abgeklärt werden. Ziel ist es, Anfang 2027 die Termine zu veröffentlichen.

---

## Lars: uMap Seite, EqualStreetNames und lokale KI

### uMap Seite für openstreetmap.de

Ich habe an einer [uMap Seite für openstreetmap.de](https://github.com/fossgis/openstreetmap.de/issues/106) gearbeitet. Hier besteht noch Review-Bedarf und es muss geklärt werden, wer die hübschen Titelbilder erzeugt.

### EqualStreetNames Berlin

Vor einiger Zeit gab es für Berlin auch ein [EqualStreetNames](https://equalstreetnames.org/)-Projekt. Nach einem Serverumzug und aus weiteren Gründen ist das Projekt leider offline. Ich habe an dem Setup weiter gearbeitet und einige Verbesserungen eingebaut. Es entstand ein neuer Hell-/Dunkel-Stil, der einen besseren Kontrast und damit bessere Lesbarkeit ermöglicht. Gängige Standards für Farbfehlsichtigkeit wurden auch so weit wie möglich berücksichtigt. Ein großer Punkt war die Performance, hier wurde eine deutliche Verbesserung sowohl im Ladeverhalten als auch bei der interaktiven Nutzung der Karte erreicht.

Leider war das Hackweekend dann doch zu kurz, um das Ergebnis online zu stellen. Die Änderungen betrafen zum Schluss nicht nur den Code der Berliner Instanz, sondern auch den Upstream-Code des EqualStreetNames-Projekts. Hier ist im Moment noch unklar, inwieweit der Code separiert werden kann. Außerdem fehlt auch noch der Ansible-Code für das Deployment auf einem FOSSGIS-Server.

### Lokale KI

Bereits im Vorfeld des Hackweekends habe ich mich mit lokaler KI beschäftigt. Mich hat interessiert, wie so ein Setup funktioniert und was für Komponenten man benötigt. Kann ich es in meine Tools (IDE, QGIS) einbinden, und wie sieht die Performance aus? Auf dem Hackweekend habe ich mein lokales Modell tatsächlich benutzt, z. B. für die Arbeit an EqualStreetNames. Außerdem habe ich mir mehrere Chat-Oberflächen angeschaut. Bisher nutze ich [GlyphStream](https://github.com/xiphux/glyphstream), aber es gibt auch noch [Open WebUI](https://openwebui.com/) und [LibreChat](https://www.librechat.ai/). Mein Fazit: Ich werde noch weitere Tests machen und viel ausprobieren. Wenn alles nach Plan läuft, könnte es einen Vortrag auf der nächsten FOSSGIS-Konferenz in Heidelberg geben.

---

## Hartmut: Druckbare OSM Karten mit SeaMap Overlay

Druckbare OSM Karten mit [print.get-map.org](https://print.get-map.org/):

- CartoOSM Stil Version Upgrade
- SeaMap Overlay Implementierung, Work in Progress
- GitHub: [github.com/hholzgra/mapnik-seamap-overlay](https://github.com/hholzgra/mapnik-seamap-overlay)

{{< rawhtml >}}
<a href="/news/images/2026-10-30_hackweekend_berlin_seamap_full.png" target="_blank"><img src="/news/images/2026-10-30_hackweekend_berlin_seamap.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}
*Aktueller Status (Klick auf das Bild öffnet die volle Auflösung, 19866×14043 Pixel)*

---

## Tordanik: 3D-Rendering und Prototype Fund 2027

Tordanik, der Autor von [OSM2World](https://osm2world.org/), hat sich mit 3D-Rendering beschäftigt, unter anderem mit dem 3D-Rendering von Brücken mit `bridge:structure`, `bridge:support` etc. Außerdem ging es um die Planung für den [Prototype Fund](https://www.prototypefund.de/) 2027 (3D, Straßenflächen, Stadtmodelle o. ä.).

---

## Transitous: ÖV Daten aus OSM und Wikidata anreichern

Grundfrage: Wie kann man [Transitous](https://transitous.org/) ÖV Daten mit Linien, Haltestellen, Betreibern etc. aus OSM und Wikidata anreichern?

### Wikidata und/oder OSM

- Nicht zu viel in Wikidata, also eine separate Wikibase Instanz OSMWikibase?
- OSMWB kann in Wikidata freigeschaltet werden für föderiertes SPARQL Querying
- Wikidata Lookups erstmal auf Nicht-Bus beschränken, um zu verhindern, dass zu viele neue Entitäten entstehen
- OSM für Linien priorisieren mit Tagging Alternative (keine Ways)?

### Wie an Wikidata Daten rankommen?

- Wikimedia Enterprise Snapshots für inkrementelle Dumps? Trial/Pay/Exceptions?
- XML vs. RDF vs. Snapshots (nicht kompatibel, also mit dem anfangen, was man wirklich verwenden will)
- Es gibt keine freie Möglichkeit, inkrementelle Dumps zu bekommen
- [wdumps](https://tools.wmflabs.org/wdumps): filtern nach Properties etc.
- Wikidata Dump (oder gefilterten Dump) direkt in MOTIS parsen?
- Wikidata Dump nach "GTFS" konvertieren, für einfachen Import/Merging in MOTIS (Wikidata/Wikibase ist vermutlich mit den Datenmengen queryable, also ist kein direkter Dump Import nötig; GTFS ist ein sinnvolles Zwischenformat, auch von anderen konsumierbar)
- Erster Schritt: primär auf OSM matchen, dann mit Wikidata IDs aus OSM Daten aus Wikidata anziehen
- Agency: Wikidata IDs in OSM, Lookup von speziellen GTFS anhand von IDs
- Linie ebenso?

### Geo Projektidee

OSM wayless route relations shape generator (osm2gtfs -> MOTIS?)

Die ausführlichen englischen Notizen gibt es im [Transitous Wiki](https://github.com/public-transport/transitous/wiki/OSM-Hack-Weekend-Berlin,-October-2026). Einen Bericht über das Wochenende hat außerdem Volker Krause in seinem [Blog](https://www.volkerkrause.eu/2026/10/30/osm-hack-weekend-berlin-october-2026.html) veröffentlicht.

---

## Austausch zu Agentic Coding im OSM Umfeld

- LLM Benutzung in Foren (lieber einfach den Prompt schicken)
- OSM Ressourcen überlastet (Overpass)
- Projekte, die Maintainer selbst nur mit KI Hilfe verstehen. Total demotivierend
- AI Vandalismus (what to do?)

---

## Marcus: Brauchen wir noch eigene Anwendungen?

Meine Frage für das OSM Hacking Weekend war: **Welche Bedeutung hat KI für das Programmieren rund um OpenStreetMap?**

Zunächst habe ich dazu einige Artikel in der c't gelesen. Anschließend wollte ich selbst ausprobieren, wie gut KI beim Programmieren helfen kann.

Als Erstes habe ich meine [Geldautomaten-Suche](https://geldautomaten-suche.org/) mithilfe von KI um einen Vektorlayer erweitert, der zusätzliche Daten zu Geldautomaten von der [Obstbaumkarte](https://obstbaumkarte.de) einbindet. Die Erweiterung war innerhalb einer halben Stunde fertig.

Dann habe ich die KI gefragt, wo sich die nächsten Geldautomaten genossenschaftlicher Banken befinden. Sie hat sie sofort gefunden – und damit den Sinn meiner eigenen Geldautomaten-Suche ein Stück weit infrage gestellt.

Ähnlich ging es mir mit meinem nächsten Projekt: Ich möchte eine Anwendung entwickeln, die einen Wanderweg aus einer GPX-Datei in Tagesetappen zerlegt, deren Endpunkte an Haltestellen des öffentlichen Nahverkehrs liegen. Auch diese Aufgabe habe ich zunächst der KI gestellt. Das hat funktioniert – und damit stand auch der Sinn dieses Projekts infrage.

Eine Frage blieb offen: **Was verbraucht eigentlich mehr Energie und verursacht mehr CO₂ – für jede Anfrage eine KI zu bemühen oder spezielle Such- und Planungsanwendungen zu entwickeln und zu betreiben?** Eine Antwort könnte sein, dass eine selbst programmierte Anwendung weniger CO₂ verbraucht, wenn sie häufiger benutzt wird. Wird sie aber nur ein paar Mal benutzt, könnte die Entwicklungszeit gespart und stattdessen einmal eine KI genutzt werden.

Trotzdem habe ich mit meinem Wanderplanungsprojekt begonnen, natürlich mit Unterstützung der KI. Vielleicht finde ich ja ein Alleinstellungsmerkmal: etwas, das andere Planungsanwendungen nicht bieten und etwas, das eine KI allein nicht so gut kann.

Mein vorläufiges Fazit: KI macht das Programmieren erstaunlich einfach. Gleichzeitig stellt sie die Frage, welche Anwendungen wir überhaupt noch selbst entwickeln sollten.

Und: auch bei meinem Text habe ich mich von einer KI beim Schreiben unterstützen lassen.

---

## Tobias (remote): Find Deleted Data, OSMCha2 und Quasi-Luftbilder

### OSM Find Deleted Data auf API v2

Die ohsome API wird bald abgeschaltet, das Tool läuft jetzt auf der API v2:

- [Demo](https://osmberlin.github.io/osm-find-deleted-data/?z=15.56&lat=52.47482&lng=13.41636&filter=amenity%3Dbench&from=2024-04-01&to=2026-06-19&bbox=[13.41291,52.472494,13.420682,52.476229])

### OSMCha2 weiter poliert

Das Projekt hat zwei Ziele: Ein neues UI explorieren und vor allem ein sehr gutes mobiles UI bauen. Außerdem soll das Kommentieren, Bewerten und Diskutieren verbessert werden. Man kann zum Beispiel Kommentare auf einzelne `key=value` Zeilen machen oder Kommentare mit einem Pin anreichern.

- [Beispiel](https://tordans.github.io/osmcha2/changesets/190898036?page=1&ref=way/317329388/addr:street&map=18/52.474/13.44073)

### Straßenfotos zu Quasi-Luftbild Pipeline

Für dieses Projekt hatte ich schon lange viele LLM Sessions und konnte jetzt erste Erfolge erzielen. [Auf der HOT OpenAerialMap](https://api.imagery.hotosm.org/browser/stac/collections/openaerialmap/items/ef24d727-3830-43be-8e87-ebe887d60e93?.language=de&.asset=asset-original) sieht man eine Quasi-Luftbild Ansicht, die aus 360° Straßenfotos (Fahrrad und Helm mit 360° Kamera) entstanden ist. Das Repo muss ich noch aufräumen, bevor ich es Open Source schalte.

- [Zweiter Testlauf (gehend mit Selfiestick)](https://api.imagery.hotosm.org/browser/stac/collections/openaerialmap/items/1e7cb303-0c37-4904-81bf-374640b500af?.language=de)

---

## Oliver, Pauli und Till: Geodaten sticken

Ziel war es, den Prozess zu vereinfachen und zu automatisieren, mit dem eine Karte im SVG Format erstellt und anschließend in Inkscape mit dem Ink/Stitch Plugin in eine Datei für die Stickmaschine umgewandelt wird.

Entstanden ist ein Prototyp: [osm.tillb.de/stitching](https://osm.tillb.de/stitching/) ([github.com/Tillbtn/osm2stitch](https://github.com/Tillbtn/osm2stitch))

- Konfigurator:
    - Ausschnitt, Format und Maßstab wählen
    - Stil, Farben und Stickkonfiguration anpassen
    - Downloadformate für verschiedene Stickmaschinen und als SVG zur möglichen Nachbearbeitung
- Umsetzung:
    - OSM Daten für das gewählte Gebiet per Postpass laden
    - Straßen verbinden, Gebäudeblöcke zu einfacheren Geometrien zusammenfassen
    - Pfadberechnung für die Stickreihenfolge
    - Erstellung der Stickdatei mit der Ink/Stitch CLI und pyembroidery

Nächste Schritte: Einen Testausschnitt sticken und mit den Parametern experimentieren.

{{< rawhtml >}}
<a><img src="/news/images/2026-10-30_hackweekend_berlin_osm2stitch.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Oliver: Routing in der Obstbaumkarte

In die [Obstbaumkarte](https://obstbaumkarte.de/) wurde ein Routing integriert. Weitere spezielle Routingprofile folgen.

---

## Mlvln: ÖPNV Karte in QGIS

Experimente in QGIS für eine OSM Public Transport Karte:

{{< rawhtml >}}
<a><img src="/news/images/2026-10-30_hackweekend_berlin_qgis_oepnv.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## Alex: Straßenraumkarte

In diesem Jahr habe ich die Prozessierung der Straßenraumkarte auf einen "modernen" Stand erneuert und viele Verbesserungen im Rendering umgesetzt. Eine Testversion für den [Berliner Innenstadtring](https://strassenraumkarte.osm-berlin.org/?map=release02#18/52.47379/13.44164) ist bereits online, die finale Veröffentlichung samt Blogartikel folgt demnächst.

Auf dem Hackweekend habe ich ein paar Fixes und Verbesserungen umgesetzt, da ich von anderen Teilnehmenden einiges Feedback bekommen habe. Insbesondere habe ich damit begonnen, das Rendering von Straßen und Wegen auf ein neues, konsequent flächenbasiertes System umzustellen. Das vereinfacht die Darstellung von Oberflächenattributen und reduziert Artefakte, zum Beispiel an den Enden und Übergängen von Wegen. Außerdem habe ich eine Überarbeitung des Stylings für Straßen und Wege angestoßen, um Wegeart (Straßen, Zufahrten, Wege) und Oberflächen (einige Varianten von befestigten und unbefestigten Oberflächen) besser unterscheiden zu können. Coming soon...

Nebenbei wie immer über verschiedene OSM Themen von Tagging Fragen bis KI Entwicklung gequatscht.

{{< rawhtml >}}
<a><img src="/news/images/2026-10-30_hackweekend_berlin_strassenraumkarte.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}

---

## cyton: LiDAR Scans puzzlen

Unvollständiges Puzzle aus LiDAR Scans, global ausgerichtet:

{{< rawhtml >}}
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-bottom: 20px;">
<div>
<a><img src="/news/images/2026-10-30_hackweekend_berlin_lidar_1.png" style="width: 100%; height: auto; border: 1px solid #808080; border-radius: 3px;"/></a>
</div>
<div>
<a><img src="/news/images/2026-10-30_hackweekend_berlin_lidar_2.png" style="width: 100%; height: auto; border: 1px solid #808080; border-radius: 3px;"/></a>
</div>
</div>
{{< /rawhtml >}}

- Scaniverse Export: glb, via LocalSend
- Jeweils zwei Dateien in CloudCompare aneinander schieben (Y-Achse beim Drehen beibehalten), die 4×4 Matrix der Operation kopieren und zusammen mit den Dateinamen notieren
- Ein Python Skript liest die relativen Operationen zwischen den Dateipaaren ein, speist sie in ein mit dem open3d Paket kompatibles Modell ein, lässt eine genauere Ausrichtung berechnen und speichert alle in ein globales Koordinatensystem verschobenen Modelle einzeln als obj

Alle Modelle gleichzeitig in CloudCompare anzuzeigen, ist für meinen alten Laptop schon sehr grenzwertig machbar.

---

## Wolfram: BBBike Extract Service und Mapillary Takeout

### BBBike Extract Service

Mit dem [BBBike Extract Service](https://extract.bbbike.org/) lassen sich OpenStreetMap Daten für beliebige, auf einer Karte ausgewählte Gebiete herunterladen. Die Daten stehen in mehr als 20 Formaten zur Verfügung, unter anderem für Garmin Geräte, Smartphone Apps und GIS Software. Während des Hackweekends habe ich an einem neuen responsiven Design gearbeitet, das die Nutzung des Dienstes auf Smartphones und Tablets erleichtert. Außerdem habe ich Spanisch, Arabisch und Chinesisch als weitere Sprachen hinzugefügt. Damit ist der Dienst nun in sieben Sprachen verfügbar.

{{< rawhtml >}}
<a><img src="/news/images/2026-10-30_hackweekend_berlin_bbbike_extract.jpg" width="300" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}
*Der [BBBike Extract Service](https://extract.bbbike.org/?lang=zh) auf dem Smartphone mit chinesischer Benutzeroberfläche*

### Mapillary Takeout

Mit dem Tool [mapillary_takeout](https://github.com/gitouche-sur-osm/mapillary_takeout) kann man die Fotos, die man zu Mapillary hochgeladen hat, als Backup herunterladen.

Leider funktioniert das Tool seit der Umstellung der Mapillary API von v3 auf v4 (2021) nicht mehr. Ich habe das Python Skript an die neue API angepasst und damit mehr als 10.000 Fotos mit voller DSL Bandbreite (30 MByte/s) heruntergeladen.

Die Fotos kommen in Originalgröße, aber verpixelt. GPS Position, Aufnahmezeit, Blickrichtung und Kamera schreibt das Skript wieder als EXIF in die Dateien. Das neue Skript wird in den nächsten Tagen veröffentlicht.

---

## Panoramax Instanz für Berlin und Brandenburg

Wir haben über eine [Panoramax](https://panoramax.fr/) Instanz für Berlin und Brandenburg diskutiert. Panoramax ist eine freie Alternative zu Mapillary und Google Street View.

Dabei ging es um rechtliche Risiken, die benötigte Hardware und darum, dass jemand die Initiative ergreift und es einfach mal macht. Leider hat aktuell niemand Zeit. Wenn du Interesse hast, melde dich einfach auf der Berliner OSM Mailingliste.
