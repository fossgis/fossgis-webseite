---
title: "CRA, openCode, ZenDiS"
date: "2025-12-09"
author: "Jochen Topf, Katja Haferkorn"
images:
language: de-de
categories:
- FOSSGIS
- openstreetmap
- Arbeitstreffen
---

### Cyber Resilience Act und die openCode-Plattform des ZenDiS

Am 09.12.2025 hat der FOSSGIS e.V. einen Informationstermin zum Cyber Resilience Act (CRA) und zur Platform openCode.de organisiert. [Julian Schauder](https://schauder.info/
) vom [ZenDiS](https://www.zendis.de/) stellte uns [openCode.de](https://opencode.de/) vor. Angesprochen waren Firmen und Institutionen, die Lösungen auf Basis von Open Source Software anbieten. 
25 Teilnehmende waren dabei, zahlreiche Fragen konnten beantwortet werden.


### ZenDiS und openCode

Das ZenDiS (Zentrum für Digitale Souveränität der Öffentlichen Verwaltung) wurde 2022 gegründet und ist seit 2024 operativ tätig. Seine Aufgabe ist die Unterstützung der öffentlichen Verwaltungen in Deutschland bei der Ablösung von digitalen Abhängigkeiten. Dafür bietet das ZendiS derzeit die Produkte OpenDesk als Arbeitsplatzsoftware und openCode als Kollaborationsplattform für die Nutzung in öffentlichen Institutionen an. Alle Software ist Open Source und kommt damit der Forderung "public money, public code" nach.

openCode ist im Kern eine öffentliche Gitlab-Instanz, sie bietet zahlreiche Repositories mit Tools, Infrastruktur und Anwendungen für die öffentliche Verwaltung. Beispielsweise wird derzeit das Konsultationsverfahren zum Deutschlandstack über openCode durchgeführt. Repositories mit Code können nur für Open-Source-Software eingerichtet werden, proprietärer Code ist nicht erlaubt. Und es braucht die Zustimmung mindestens einer Verwaltung aus Deutschland, um sicherzustellen, dass auch Interesse von der Verwaltung aus besteht.


{{< rawhtml >}}
<a href="https://files.fossgis.de/Koordinierungsstelle/Workshop/2025-12-09_Folien_CRA-OpenCode-Onlinetermin.pdf"><img src="/news/images/2025-12-09_CRA-openCode-ZenDis_Fole9.png" width="800" style="border: 1px solid #808080; border-radius: 3px;"/></a>
{{< /rawhtml >}}       
_Folie aus der Präsentation zeigt Sicherheitsarchitektur von openCode_

Über ein reines Code-Repository hinaus bietet openCode viele Funktionen für ein gesundes Ökosystem.
Der Code wird von automatisierten Tools analysiert. Dabei wird eine SBOM (Software Bill of Materials) erstellt, die angibt, welche Bibliotheken und andere Software als Grundlage für ein Projekt dienen. Außerdem wird der Code auf mögliche Probleme untersucht ("linting"). Über die Software DevGard werden diese Informationen mit CVEs (Beschreibungen sicherheitskritischer Fehler) zusammengeführt. Aus all diesen Daten kann dann automatisiert eine grobe Aussagen darüber getroffen werden, wie gut eine Software gewartet ist oder wie schnell auf Sicherheitsprobleme reagiert wird. Das wird dann "plakativ" in sogenannten Bades dargestellt. Ziel ist es (potentiellen) Nutzenden Entscheidungshilfen zu geben, welche Software sie nutzen sollen.

### Cyber Resilience Act

Das wichtigste Thema der Veranstaltung war der Cyber Resilience Act (CRA), der 2026 in Kraft treten wird. Der Vortrag ging auf die Anforderungen an Software bzw. die Prozesse rund um die Erstellung und Wartung sicherer Software ein. Die Funktionen von openCode bzw. der dort eingbauten Module wurden vorgestellt, jeweils mit Referenz auf die gesetzlichen Vorgaben, deren Lösung mit openCode angestrebt wird. ZenDiS schafft damit eine Referenzimplementierung, die zeigt, wie der CRA praktisch umgesetzt werden kann und steht dafür auch im engen Austausch mit dem BSI (Bundesamt für Sicherheit in der Informationstechnik), das in Deutschland als Regulierer für die Durchsetzung des CRA zuständig ist.

Wir danken dem ZenDiS und insbesondere dem Vortragenden Julian Schauder für ihre Arbeit und den interessanten Vortrag und Fragerunde danach.

Die vorgestellten Folien sind [hier](https://files.fossgis.de/Koordinierungsstelle/Workshop/2025-12-09_Folien_CRA-OpenCode-Onlinetermin.pdf) zu finden.

Wer weiter an dem Thema interessiert ist: Auf der kommenden FOSSGIS-Konferenz wird es auch einen Vortrag zu dem Thema [Sichere Softwarelieferketten mit openCode](https://pretalx.com/fossgis2026/talk/YCJCXQ/) und eine Expert:innen-Fragestunde zum Thema [OpenCode.de: Softwarequalität erkennen - Badges](https://pretalx.com/fossgis2026/talk/M8RAVF/) geben. Die Arbeitsgruppe CRA des FOSSGIS e.V. trifft sich regelmäßig, Infos zur Arbeitsgruppe dazu sind im [Wiki](https://www.fossgis.de/wiki/Arbeitsgruppe_CRA) zu finden.
