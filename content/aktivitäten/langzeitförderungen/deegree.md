---
title: "Deegree"
---

[**deegree**](https://www.deegree.org) ist eine Open-Source-Software für Geodateninfrastrukturen und das Geodaten-Web. **deegree** bietet Komponenten für das Geodatenmanagement an, einschließlich Datenzugriff, Visualisierung, Ermittlung und Sicherheit. Offene Standards stehen im Mittelpunkt von **deegree**.

Die **deegree**-Software basiert auf den Standards des Open Geospatial Consortium (OGC) und des ISO Technical Committee 211. Sie umfasst die Referenzimplementierung des OGC Web Map Service (WMS), einen vollständig kompatiblen Web Feature Service (WFS) sowie Pakete für Catalogue Service (CSW), Web Coverage Service (WCS), Web Processing Service (WPS) und Web Map Tile Service (WMTS). Seit 2000 wird *deegree* von lat/lon entwickelt, mit der starken Absicht, es zu einem Community-getriebenen Projekt zu machen. Ein wichtiger Schritt in diese Richtung war die Akzeptanz als OSGeo-Projekt im Jahr 2010. Heute wird *deegree* von mehreren Organisationen und Einzelpersonen mit einer großen Anwenderbasis auf der ganzen Welt aufrechterhalten.

## Kernfunktionen 
### Web Feature Services (WFS): Liefert Vektordaten aus Geodaten

* Implementiert die WFS-Standards 1.0.0, 1.1.0 und 2.0.0 (OGC-Referenzimplementierung)
* Unterstützt KVP-, XML- und SOAP-Anforderungen
* GML `2/3.0/3.1/3.2` als Ausgabe/Eingabe
* Erweiterte Unterstützung für Filterausdrücke basierend auf XPath 1.0
* Unterstützt zahlreiche Backends wie PostGIS, Oracle Spatial, MS SQL Server, Shapefiles oder GML-Instanzdokumente

### Web Map Services (WMS): Liefert Karten aus, die aus Geodaten gerendert wurden

* Implementiert die WMS-Standards 1.1.1 und 1.3.0 (OGC-Referenzimplementierung)
* Umfassende Unterstützung für die Styling-Sprachen SLD/SE-Versionen 1.0.0 und 1.1.0
* Unterstützt zahlreiche Backends wie PostGIS-, Oracle Spatial-, Shapefiles- oder GML-Instanzdokumente
* Rasterformate wie PNG oder GeoTIFF

### Web Map Tile Services (WMTS): Liefert vorgerenderte Kartenkacheln aus

* Implementiert den grundlegenden WMTS-Standard 1.0.0 (OGC-Referenzimplementierung)
* Unterstützt verschiedene Backends wie GeoTIFF, Remote-WMS oder Rasterpyramiden und Kacheln 

### Catalogue Services for the Web (CSW): Führt Suchen nach Geodatensätzen und -diensten durch

* Implementiert den CSW-Standard 2.0.2
* Vollständig transaktional
* Unterstützt KVP-, XML- und SOAP-Anforderungen
* ISO-Metadaten-Anwendungsprofil 1.0.0
* Behandelt alle definierten abfragbaren Eigenschaften (sowohl für Dublin Core als auch für das ISO-Profil)

### Web Processing Services (WPS): Führt Geodatenprozesse aus

* Implementiert den WPS-Standard 1.0.0
* Unterstützt KVP-, XML- und SOAP-Anforderungen

### OGC GML 2.12, 3.0.1, 3.1.1 und 3.2.1

* OGC-zertifizierte Referenzimplementierung für 3.2.1

## Implementierte Standards

* Catalogue Service for the Web (CSW) 
* Filter Encoding (FE) 
* Geographic-Markup-Language(GML) 
* Open Geospatial Consortium (OGC) 
* Styled Layer Descriptor (SLD) 
* Web Coverage Service (WCS) 
* Web Feature Service (WFS)
* Web Feature Service - Gazetteer Service (WFS-G) 
* Web Feature Service - Transactional (WFS-T) 
* Web Map Service (WMS) 
* Web Map Tile Service (WMTS) 
* Web Processing Service (WPS)

## Technische Daten

* Plattformen: Linux/Unix, Mac OS, Windows
* API-Schnittstellen: WFS, WMS, WMTS, CSW, WPS, WCS, REST-API
* Sprachen: Java, XML
* Datenbanken: PostgreSQL/PostGIS, Oracle Locator, MS SQLServer
* Server: Apache Tomcat, WildFly, Jetty, GlassFish

## Lizenz

* GNU Lesser General Public License, Version 2.1 (LGPL 2.1)
