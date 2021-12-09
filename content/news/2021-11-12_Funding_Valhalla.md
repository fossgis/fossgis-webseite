---
title: "Globaler Valhalla Server online"
date: "2021-11-12T15:00:00+02:00"
author: "Nils Nolde"
---

Zusätzlich zum bereits existierenden und viel genutzten OSRM Server hat der FOSSGIS e.V. nun einen [Förderantrag](https://www.fossgis.de/wiki/Förderanträge/Valhalla-Routingserver) genehmigt für die Bereitstellung einer globalen und freien Server Instanz der FOSS Routing Software [Valhalla](https://github.com/valhalla/valhalla).

Ein interaktiver Router ist auf https://valhalla.openstreetmap.de verfügbar.

## Was ist Valhalla?

Valhalla ist ein ursprüngliches Mapzen Projekt das [2015](https://www.mapzen.com/blog/valhalla-intro/) gestartet wurde: ein C++ Framework für hoch-dynamisches und effizientes Openstreetmap Routing.

Valhalla baut, im Gegensatz zu den meisten vergleichbaren FOSS Lösungen, auf einem gekachelten Graphen auf, der, ähnlich wie Map Vector Tiles, in eine Hierarchie gegliedert ist. Damit wird der RAM Verbrauch beim Betrieb eines Servers relativ gering gehalten, gleichzeitig können alle Bewegungsprofile auf dem gleichen Graphen agieren. Daher kann man Valhalla problemlos auch offline auf Mobilgeräten laufen lassen. Aufgrund der hoch flexiblen Routingalgorithmen und der reichhaltigen Attribution in den Kacheln, lässt sich die Routenfindung mit vielen Einstellungsmöglichkeiten bei jeder Routenanfrage anpassen, u.a.:

- Polygone vermeiden, z.Bsp. bei großen Events oder temporären Baustellen  
- Fahrzeugdimensionen einhalten, z.Bsp. Höhe und Gewicht des Autos/LKWs  
- Höhenmeter vermeiden oder begünstigen für Fahrrad/Fußgänger  
- jede Menge anderer "Costing" Optionen wie Maut/Autobahn/Spielstraßen/Grenzübergänge/Fähren vermeiden/begünstigen  
- multimodales Routing (**noch nicht** verfügbar auf dem FOSSGIS Server)  
- Verkehrseinbindung, live & historisch (**nicht** verfügbar auf dem FOSSGIS Server)  

Eine vollständige Liste aller Optionen findet man in der [Dokumentation](https://github.com/valhalla/valhalla/blob/master/docs/api/turn-by-turn/api-reference.md#automobile-and-bus-costing-options). 

Eine weitere Besonderheit von Valhalla ist, dass die meisten obigen Optionen für **alle Endpunkte** gelten, also kann man sogar eine Matrix berechnen die die Vehikeldimensionen bei der Routenfindung beachtet.

![Valhalla Isochrone Berlin](/news/images/2021_11_12_Valhalla_Isochrone_Berlin.png)
<figure>
  <img
  src="/news/images/2021-11-12_Valhalla_Isochrone_Berlin.png"
  alt="Valhalla Isochrone in Berlin">
  <figcaption>&copy; Data by <a href="https://www.openstreetmap.org/copyright" target="_blank">OpenStreetMap Contributors</a>, &copy; Position base map by <a href="https://carto.com" target="_blank">Carto</a></figcaption>
</figure>

## Wie nutzt man Valhalla?

Ein interaktiver Router ist auf https://valhalla.openstreetmap.de verfügbar. 

Die HTTP Schnittstelle ist erreichbar auf https://valhalla1.openstreetmap.de (beachte die **1**). Die folgenden Endpunkte sind freigeschaltet (Links führen zur entsprechenden Dokumentation):

- [`/route`](https://github.com/valhalla/valhalla/blob/master/docs/api/turn-by-turn/api-reference.md): Eine Route mit bis zu 20 Wegpunkten berechnen  
- [`/sources_to_targets`](https://github.com/valhalla/valhalla/blob/master/docs/api/matrix/api-reference.md): Eine Matrix mit bis zu 50 OD Paare  
- [`/isochrone`](https://github.com/valhalla/valhalla/blob/master/docs/api/isochrone/api-reference.md): Bis zu 100 Minuten/150 Kilometer Isochronen & Isodistanzen  
- [`/optimized_route`](https://github.com/valhalla/valhalla/blob/master/docs/api/optimized/api-reference.md): Lösung des Traveling Salesman Problem  
- [`/trace_route`, `/trace_attributes`](https://github.com/valhalla/valhalla/blob/master/docs/api/map-matching/api-reference.md): Map-matching und -tracing  
- [`/status`](https://github.com/valhalla/valhalla/blob/master/docs/api/status/api-reference.md): Healthcheck und Zeitstempel des Graphen  
- (sehr bald): `/expansion`, wie `/isochrone` aber mit einzelnen Straßengeometrien statt Polygonen  

Es gibt auch eine Reihe unterstützender FOSS für Valhalla um den Einstieg zu erleichtern:

- [Valhalla JS Demos](https://github.com/valhalla/demos)  
- [QGIS Plugin](plugins.qgis.org/plugins/valhalla/)  
- [Valhalla Web App](https://github.com/gis-ops/valhalla-app)  

Es gelten die aktuellen [Nutzungsbedingungen](https://fossgis.de/arbeitsgruppen/osm-server/nutzungsbedingungen/) der FOSSGIS e.V. Dienste.

## Vergleich Valhalla & OSRM

Man könnte annehmen dass es sich bei beiden um Konkurrenten handelt. Tatsächlich erfüllen sie recht unterschiedliche Aufgaben in ihrem derzeitigen Entwicklungsstadium und ergänzen sich funktional hervorragend: während OSRM sich über riesige Matrizen in Rekordzeit freut, ist Valhalla feinfühliger und kann auch sehr spezielle Routingoptionen wunderbar umsetzen.

Ein paar zusätzliche Vergleiche:

- OSRM erfordert eine riesige Menge RAM für den Graphen, während Valhalla auf einem alten Smartphone (theoretisch) den ganzen Planeten laufen lassen kann  
- Valhalla benötigt relativ viel zusätzlichen RAM für individuelle Anfragen, während OSRM wenig extra RAM braucht für selbst sehr große Anfragen  
- Die Matrix API (und in geringerem Maße auch die Routing API) ist Größenordnungen schneller bei OSRM, Valhalla ist dafür vielseitiger einsetzbar (funktional und Hardware)  
