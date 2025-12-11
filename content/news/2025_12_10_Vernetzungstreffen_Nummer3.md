---
title: "Vernetzungstreffen"
date: "2025-12-10"
author: "Katja Haferkorn"
images:   
- https://www.fossgis.de/mediawiki/images/b/b9/FOSSGIS-Logo_Slogan.png
language: de-de
categories:
- FOSSGIS
- openstreetmap
- Arbeitstreffen
---

Am 10. Dezember hat das Online-Vernetzungstreffen der FOSSGIS-Community stattgefunden. Mehr als 20 Teilnehmende nutzten die Gelegenheit, sich Wissen und Informationen zum Thema "KI in der Geodatenanalyse: Chancen und Herausforderungen" zu holen und sich auszutauschen und zu vernetzen. 

Die Idee des Vernetzungstreffens, welches sich an Geoinformatiker:innen, FOSSGIS-Konferenz-Teilnehmende, Mitglieder und Interessierte in und an der FOSSGIS-Community richtet, ist, das gegenseitige Kennenlernen sowie Austausch zu Anliegen oder Themen, hier können sich Kontaktpunkte und Anknüpfungspunkte finden.

### KI in der Geodatenanalyse: Chancen und Herausforderungen

Hendrik Wagenseil, Geograf, arbeitet beim BKG in der [Arbeitsgruppe](https://www.bkg.bund.de/DE/Forschung/Projekte/KI-Vorhaben/KI-Vorhaben_cont.html) KI- Analyse von Fernerkundungsdaten. Nach ein paar Basics nimmt uns Hendrik mit in die Fragestellungen und Abläufe und erklärt anhand von Anwendungsfällen den Einsatz von KI beim BKG, beleuchtet Nutzen, Erwartung an KI, sowie auch die Herausforderungen. Als nützlich erweist sich die Ressourceneffizienz bei Prozessen, die viel manuelles Arbeiten erfordern, aber auch bei Änderungen in Daten kann KI unterstützen sowie es auch bei der Erschließung der Datenvielfalt von Lidardaten nützlich sein kann. 
Wenn ein Prozess operativ in den Einsatz kommt, ist die Schnelligkeit von Nutzen, weil damit viel händische Arbeit weg fällt.

{{< rawhtml >}}
<a><img src="/news/images/2025-12-10_Vernetzungstreffen_KI-Geodatenanalyse_KI-Nutzen.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
_Nutzen von Geo-KI_


Noch ist das nicht soweit, die Verfahren befinden sich in verschiedenen Entwicklungsstadien und sind auf dem Weg zum Abschluss. Durch iteratives Arbeiten lassen sich die Prozesse Stück für Stück in den operativer Einsatz überführen.
Es gibt Schnittstellen zu definieren, den Umgang mit Unsicherheiten zu üben und der Ressourcenhungrigkeit der Techologie gerecht zu werden.

Um mit der Schnelligkeit der aktuellen Entwicklung mitzuhalten, braucht es agiles und exploratives Arbeiten, hier machen es die Hürden einer Behörde einhergehend mit starken 
Sicherheitseinschränkungen und dazugehöriger Bürokratie, z.B. DSGVO nicht leicht. 

Der Anwendungsfall _Baustellenerkennung_ war beispielgebend für die Ausführungen im Vortrag und die Darstellung der "KI-Pipeline".


{{< rawhtml >}}
<a><img src="/news/images/2025-12-10_Vernetzungstreffen_KI-Geodatenanalyse_KI-Pipeline.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
_Pipeline Geo-KI_

### Q&A

Die Teilnehmenden bringen diverse Hintergründe mit, beschäftigen sich mit OSS-Software, Open Data oder OSM im Job in der öffentlichen Verwaltung oder Privatwortschaft und haben verschiedenste Fragestellungen zum Thema.

* **Frage:** Wenn das Erkennungs-Modell auf einem anderen Modell aufbaut, kann man ihm auch "Vorkenntnisse" wieder abtrainieren? Z.B. Wenn viele Baustellen in den USA im Trainingsdatensatz waren und diese bestimmte Merkmale (z.B. Fahrzeuge) aufweisen die für die Baustellenerkennung hier irrelevant  bzw. irreführend sind?    
**Antwort:** Architektur + Gewichte + Beispiele + Training mit False Positives macht das Modell genauer.

* **Frage:** Wie sieht es mit FOSS aus? Werden die Modelle open Source gestellt?    
**Antwort:** BKG hat die exotische Rolle in Bereich Datenharmonisierung, d.h. die Aufgabe ist es von den Ländern übergebene DOP-Daten zu vereinheitlichen und bereitzustellen. Grundlage ist eine Verwaltungsvereinbarung, die Daten gehören nicht dem BKG, deshalb können Labels nicht Open Source gestellt werden. Beispiel Daten zum Digitalen Zwilling gehören dem BKG, Veröffentlichung ist angedacht/geplant, da es sicherheitsrelevante Details enthält, gibt es dazu noch Diskussionen.     
Hier spielt auch das Thema Lizenzen rein, Sentinel-Daten sind frei verfügbar, Privatanbieter bieten kommerzielle Produkte, die teilweise detailreicher sind, eine Veröffentlichung ist deshalb nicht möglich bzw. unbezahlbar.
Die zugrunde liegenden rechtlichen Regelungen geben verchiedenen Aussagen, das
Haushaltsrecht regelt anders, als die Open Data Verordnung.   
Deshalb ist es noch offen, ob Code ververöffentlicht werden kann.   
Hinweis aus der Teilnehmerschaft: Falk Zscheiles [Vortrag auf der FOSSGIS 2025](https://media.ccc.de/v/fossgis2025-58056-text-und-data-mining-in-der-openstreetmap-datenbank-aus-rechtlicher-sicht ) sagt, dass das Modell veröffentlicht werden dürfte. 

* **Frage:** Gibt es Erfahrungen mit Digitalisierung von gescannten analogen Beabauungsplänen etc.?    
**Antwort:** Liegenschaftskataster ist Ländersache. Niedersachsen hat ein fortgeschrittenes Modell um einzelne Gebäude auf Luftbildern zu erkennen, hier sind Fernerkundungsdaten die Grundlage, keine B-Pläne.

* **Frage:** Hat das BKG Erfahrungen zum Georeferenzieren mit KI?    
**Antwort:** nein

* **Frage:** Headline: ["Erstmals alle Gebäude der Welt als 3DModell verfügbar"](https://www.tum.de/aktuelles/alle-meldungen/pressemitteilungen/details/erstmals-alle-gebaeude-der-welt-als-3d-modell-verfuegbar) - Ki oder Hexerei?    
**Antwort:** Mitteilung bezieht sich auf LOD1-Daten

Auch auf der FOSSGIS 2026 wird KI ein Thema sein, das Programm ist auf der Konferenzomepage verfügbar: https://fossgis-konferenz.de/2026/programm/.

### FOSS4G 2025
Im nächsten Themenpunkt berichtete Mirko ein paar Highlights von der [FOSS4G 2025 in Auckland](https://2025.foss4g.org/), das ist die internationale FOSS-Konferenz im Geobereich an der ca. 500 Teilnehmende dabei waren. Das Thema Nachhaltigkeit wurde in vielen Facetten diskutiert, sowohl ökologisch als auch planerisch. Beiträge aus dem deutschsprachigen Raum wurden in diesem Jahr vermisst. 

### News aus dem Verein
Die FOSSGIS 2026 findet vom (24.)25.-28.03.2026 in Göttingen statt.
- das Programm ist veröffentlicht: https://fossgis-konferenz.de/2026/programm/
- Neu: lange Workshops am Dienstag, den 24.03.2026 
- Anmeldung ab Januar 2026: https://fossgis-konferenz.de/2026/anmeldung/
- Sponsoren sind willkommen: https://fossgis-konferenz.de/2026/#Sponsoring
- Helfer:innen sind willkommen: https://fossgis-konferenz.de/2026/helfen/

Der FOSSGIS e.V. hat im Oktober einen Vereinsworkshop zur Weiterentwicklung mit 32 Mitgliedern veranstaltet, der Fokus lag auf verschiedenen Entwicklungsfeldern, wie Neumitglieder - Mitarbeit, bestehende Mitglieder - Unterstützung zur Mitarbeit, Nachwuchssicherung für Gremien, Welche Handlungsfelder sollten gestärkt werden?    
Ein Ergebnis u.a. ist, das [Vernetzungstreffen](https://www.fossgis.de/wiki/Termine/Vernetzungstreffen) auszubauen, um die Vernetzung der Mitglieder untereinander zu verstärken.    
Ein Bericht zum Vereinsworkshop ist im [Newsblog](https://fossgis.de/news/2025_10_13_fossgis-vereinsworkshop_jubilaeum/) veröffentlicht.     
Die ersten Ideen zum Buddysystem wurden geschildert, ein Treffen zum Weiterdenken am Buddysystem ist für den [22.01.2026](https://fossgis.de/aktivit%C3%A4ten/termine/) um 15 Uhr vorgesehen.    
Um an der Vision und Mission des Vereins zu arbeiten, gründet sich derzeit die [AG Grundsatz](https://www.fossgis.de/wiki/AG-Grundsatz), erste Infos sind im Wiki aufgeschrieben, das nächste Treffen findet am [19.01.2026](https://fossgis.de/aktivit%C3%A4ten/termine/) um 18 Uhr statt.

Der Vorstand des FOSSGIS-Vereins braucht neue Mitstreitende, eine komissarische Mitarbeit ist derzeit möglich, die nächste Vorstandswahl findet im Rahmen der Mitgliederversammlung im März statt. Fragen können an Katja oder jemand aus dem Vorstand gerichtet werden.

Zu guter Letzt gab es einen Aufruf zum Mitmachen an Aktivitäten des Vereins, beispielsweise bei der Unterstützung des FOSSGIS-Standes auf Veranstaltungen, wie re.publica 2026, Deutscher Kartographie Kongress (DKK) oder beim Open Source Park der OSBA auf der Smart Country Convention (SCCON), Maker Faire hannover, FrOSCon, Kielux oder KonGeoS. Bei Interesse und Fragen gerne an Katja wenden.

Die Aktivitäten des Vereins sind im FOSSGIS-Vereins-Kalender zu finden: [https://fossgis.de/aktivitäten/termine](https://fossgis.de/aktivit%C3%A4ten/termine/).

### Abschluss und Feedback

Zum Abschluss wurden in der Feedbackrunde das breite Themenspektrum als kurzweilig, ansprechend und abwechslungsreich benannt sowie die Kombination aus thematischen Informationen und Vernetzung den Verein erlebbar machen. Die Vorstellungs- und Vernetzungsrunde als interaktiver Teil der Veranstaltung wurde positiv bewertet, verbunden mit dem Wunsch nach mehr Zeit für Austausch dieser Art verbunden mit inspirierenden Fragen.

Das nächste Vernetzungstreffen ist für den **15.04.2026 um 18 Uhr** geplant, die Vorbereitungsgruppe wird die entstandenen Ideen aufgreifen und freut sich auf das nächste Treffen.


{{< rawhtml >}}
<a><img src="/news/images/2025-12-10_Screenshot-Vernetzungstreffen.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
_Screenshot Vernetzungstreffen 10.12.2025_
