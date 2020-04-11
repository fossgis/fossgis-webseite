---
title: "4. erfolgreiches FOSSGIS Hacking Event im Linuxhotel in Essen"
date: "2015-12-03T10:42:34+00:00"
author: "Astrid Emde"
aliases:
  - "/node/268"

---

<div id="cke_pastebin">
	Vom 20.11.-22.11.2015 trafen sich zum dritten Mal in diesem Jahr (und zum vierten Mal seit &nbsp;<a href="https://www.fossgis.de/wiki/FOSSGIS_Hacking_Event_2013">November 2013</a>) OSM- und geodatenbegeisterte Menschen zum FOSSGIS-Hackingevent im Linuxhotel. Zu den 16 Teilnehmerinnen und Teilnehmern, die aus Deutschland und den Niederlanden anreisten, gesellte sich am Samstag noch ein Tagesgast. Es wurde wieder intensiv an einer Vielzahl von Open-Source-Projekten gearbeitet. Außerdem wurden wichtige Vorarbeiten für zwei bedeutende Konferenzen der Open-Source-Geodaten-Community geleistet, die 2016 stattfinden: die Fossgis-Konferenz 2016 in Salzburg und die FOSS4G2016 in Bonn.</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	<strong>FOSSGIS-Konferenz</strong></div>
<div id="cke_pastebin">
	Die <a href="https://www.fossgis-konferenz.de/2016/">&nbsp;FOSSGIS 2016</a> findet vom 04.06.-06.06.2016 in Salzburg statt. Während des Hacking-Weekends wurde auch die Planung der FOSSGIS-Konferenzen 2016 und 2017 vorangebracht. Neben organisatorischen Planungen rund um die nächste Konferenz in Salzburg wurde das Einreichungssystem für die Vorträge aktualisiert. Hierbei wird nun eine leicht angepasste Version des &quot;frab - conference management system&quot; eingesetzt. Die [https://www.fossgis-konferenz.de/2016/ Konferenzwebsite] bekommt neue Informationen. Für die Konferenzdarstellung gibt es jetzt die Skyline der Festung Hohensalzburg als [https://www.fossgis.de/wiki/Konferenz_2016/Artwork#Skyline_Salzburg &nbsp;wunderschönes Artwork]. Am Tag vor der Konferenz wird ein OSM-Hacktag (&quot;T-1&quot;) stattfinden. Ideen und Planungen können [[Konferenz 2016/Programm/OSM-Sonntag | hier]] bzw. [https://wiki.openstreetmap.org/wiki/FOSSGIS_2016/Hackday_t-1 hier] eingetragen werden.</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	Zudem wurde der Call for Location für die <a href="https://www.fossgis-konferenz.de/2017/">FOSSGIS-Konferenz 2017 </a>vorbereitet und veröffentlicht.</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	<strong>FOSS4G2016</strong></div>
<div id="cke_pastebin">
	Mit der <a href="http://www.foss4g2016.org">FOSS4G2016</a>&nbsp;findet die bedeutendste internationale Konferenz für Open-Source-Geoinformationssysteme vom 24.8.-26.8.2016 in Bonn statt. An diesem Wochenende wurde wichtige Vorarbeit geleistet:</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	* die Homepage [http://www.foss4g2016.org/ &nbsp;www.foss4g2016.org] wurde komplett überarbeitet</div>
<div id="cke_pastebin">
	* das [https://svn.osgeo.org/osgeo/foss4g/2016/marketing/poster/foss4g2016-poster.pdf Konferenzposter] wurde gestaltet und es wurden weitere Ideen entwickelt (Facebookseite für die Konferenz, Selfiewettbewerb,...).</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	(über den aktuellen Planungsstand zur FOSS4G2016 kann man sich [https://wiki.osgeo.org/wiki/FOSS4G_2016_Meeting_minutes hier] informieren)</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	<strong>OSM- und Open-Source-Communityprojekte</strong></div>
<div id="cke_pastebin">
	* [http://www.openrailwaymap.de/ Openrailwaymap]: Entwicklung eines JOSM-Templates zum [http://lists.openrailwaymap.org/archives/openrailwaymap/2015-November/000372.html Mapping von Straßenbahnsignalen]</div>
<div id="cke_pastebin">
	* [http://blog.openstreetmap.de/ OSM-Wochennotizen]: Verbesserung des Redaktionssystems [https://github.com/TheFive/osmbc OSMBC], Erstellung einer Roadmap, Beschreibung weiterer Funktionen, Planungen zur Einbindung internationaler Teams (ES, CZ, PT, ID, TR, RV)</div>
<div id="cke_pastebin">
	* für [http://imposm.org/ Imposm3] wurden die Tests verbessert; sie laufen jetzt performanter und sind umfangreicher</div>
<div id="cke_pastebin">
	* bei [http://libosmscout.sourceforge.net/ Libosmscout] wurde die Performance verbessert (Daten werden nun intern in einer Tile-basierenden Datenstruktur gecached). Die Style-Sheet Syntax erlaubt seit kurzen &quot;Conditionals&quot;. Während es Wochenendes wurde mittels alternativer Definition der Farben und Deaktivieren einiger Darstellungselemente ein Prototyp für einen Nachmodus (weniger Elemente, abgedeckte Farben) realisiert. Das Routing behandelt nun Restriktionen wie &quot;Anlieger frei&quot; besser. Noch mehr Details bzgl. der Arbeiten am Wochenende gibt in der Projekt-eigenen Mailingliste</div>
<div id="cke_pastebin">
	* [http://www.openlayers.org OpenLayers3]-Hacking: Weiterarbeit an einer interaktiven &Uuml;berlappungsprüfung von Polygonen und Programmierung eines Beispiels zur Eventverarbeitung von geclusterten Vektordaten in einer OpenLayers3-Karte</div>
<div id="cke_pastebin">
	* im Rahmen des [https://github.com/terrestris/BasiGX BasiGX]-Projektes wurde an einer leicht zu verstehenden Freitextsuche in der OSM-Datenbank gearbeitet</div>
<div id="cke_pastebin">
	* am Sonntag wurde das Projekt &quot;In Search of Former Jewish Business Sites in Europe&quot; (Arbeitstitel: FJS - Former Jewish Stores) vorgestellt, das die Lage von Geschäften jüdischer Inhaber zeigt, die während der NS-Zeit zwangsarisiert oder geschlossen wurden</div>
<div id="cke_pastebin">
	* ebenfalls am Sonntag wurde die [http://refugeeswelcomemap.de/ Refugees Welcome Map] vorgestellt, die Helfer und Flüchtlinge über die Infrastruktur für Flüchtlings-Hilfe und -Integration informieren möchte und noch Unterstützer braucht</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	Vielen Dank an das Linuxhotel für die Beherbergung und Bewirtung.</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	Vielen Dank an den FOSSGIS e.V., der das Hacking Event finanziell unterstützt.</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	Vielen Dank an Alex für den leckeren Beaujolais.</div>
<div id="cke_pastebin">
	&nbsp;</div>
<div id="cke_pastebin">
	Vielen Dank an das Orga-Team für die umfangreiche Vor- und Nachbereitung sowie die reibungslose Durchführung des Hacking Events.</div>
