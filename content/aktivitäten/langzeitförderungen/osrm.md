---
title: "OpenStreetMap Routing Server (OSRM)"
---

Der Routing Server verarbeitet OpenStreetMap Daten mit
[OSRM](https://github.com/Project-OSRM/) für die Navigation und Routensuche. Unterstützt werden Auto-, Fahrrad- und Fussgängerprofile. Über die Seite
[routing.openstreetmap.de](https://routing.openstreetmap.de) kann man
direkt Routen planen und exportieren. Die
[API](https://github.com/Project-OSRM/osrm-backend/blob/master/docs/http.md)
ist offen und kann auch von anderen Projekten genutzt werden. Sie bietet
zum Beispiel auch eine Approximation für die Reihenfolge, in der eine
Liste von Orten am besten angefahren werden kann (bekannt als travelling
salesman Problem).

Der FOSSGIS Routing Server wird auch von der
[openstreetmap.org](https://openstreetmap.org) Webseite eingebunden.
Zugang zu solch verarbeiteten Daten ist wichtig für die Beitragenden
Mapper, als Feedback für ihre Arbeit und zum Finden von Fehlern.
[Weitere Informationen zur Infrastruktur und genutzter
Software](http://map.project-osrm.org/about.html)