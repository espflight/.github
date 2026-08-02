<div align="center">

<p>
  <a href="https://github.com/espflight/.github/blob/main/profile/README.md">English</a> ·
  <strong>Deutsch</strong> ·
  <a href="https://github.com/espflight/.github/blob/main/profile/README.fa.md">فارسی</a>
</p>

# ESPFlight

### Open-Source-Flugsteuerungsökosystem für leichte ESP-basierte DIY-Quadrocopter

**Bauen. Lernen. Fliegen. Verbessern.**

<br>

<a href="https://espflight.com">
  <img alt="ESPFlight-Website" src="https://img.shields.io/badge/Website-espflight.com-0284C7?style=for-the-badge&logo=googlechrome&logoColor=white">
</a>
<a href="https://github.com/espflight?tab=repositories">
  <img alt="ESPFlight-Repositories" src="https://img.shields.io/badge/Repositories-Ansehen-181717?style=for-the-badge&logo=github&logoColor=white">
</a>
<a href="mailto:info@espflight.com">
  <img alt="ESPFlight kontaktieren" src="https://img.shields.io/badge/Kontakt-E--Mail-0F766E?style=for-the-badge&logo=gmail&logoColor=white">
</a>

<br><br>

<img alt="Projektstatus" src="https://img.shields.io/badge/Status-Vorbereitung_der_Veröffentlichung-F59E0B?style=flat-square">
<img alt="Referenzplattform" src="https://img.shields.io/badge/Referenzplattform-ESP8266-00979D?style=flat-square&logo=espressif&logoColor=white">
<img alt="Mobile Plattform" src="https://img.shields.io/badge/Mobile_App-Android-3DDC84?style=flat-square&logo=android&logoColor=white">

<br><br>

**Firmware · Android-Steuerung · Dokumentation · Referenzaufbau**

</div>

---

## Über ESPFlight

**ESPFlight** ist ein Open-Source-Ökosystem zum Bauen, Steuern, Testen und Verstehen leichter DIY-Quadrocopter auf Basis von ESP-Mikrocontrollern.

Das Projekt verbindet Flugsteuerungsfirmware, eine speziell entwickelte Android-Anwendung, praxisorientierte Dokumentation und einen getesteten Referenzaufbau. Dadurch soll der Einstieg in die Entwicklung eigener Flugsteuerungssysteme erleichtert werden.

ESPFlight richtet sich an Maker, Studierende, Lehrkräfte, Embedded-Entwickler und Drohnenbegeisterte, die verstehen möchten, wie ein Flugsteuerungssystem funktioniert und mit kostengünstiger Hardware experimentieren wollen.

---

## Das Ökosystem

### 🚁 ESPFlight Firmware

Die zentrale Flugsteuerungsfirmware verarbeitet die Steuerbefehle des Piloten und sorgt für einen stabilen Flug.

Aktuelle Entwicklungsbereiche:

* Verarbeitung von IMU-Daten
* Schätzung der Fluglage
* PID-Stabilisierung
* Motormischung und Motorausgabe
* Verarbeitung der Steuereingaben
* Verwaltung des Flugzustands
* Scharf- und Unscharfschaltlogik
* Failsafe bei Kommunikationsverlust
* Überwachung der Batteriespannung
* Reaktion auf niedrige Spannung
* Modulare Flugsteuerungsarchitektur

### 📱 ESPFlight Lite

Eine schlanke Android-Anwendung, die speziell für unterstützte ESPFlight-Quadrocopter entwickelt wird.

Zu ihren wichtigsten Funktionen gehören:

* Touchbasierte Flugsteuerung
* WLAN-Kommunikation
* Überwachung des Verbindungsstatus
* Wesentliche Flugtelemetrie
* Batterie- und Signalinformationen
* Anzeige der Flugzeit
* PID-Konfiguration
* Für das Querformat optimierte Steuerung
* Benutzeroberfläche auf Englisch und Persisch

ESPFlight Lite konzentriert sich auf die wesentlichen Werkzeuge zur Konfiguration, Steuerung und Überwachung eines unterstützten Fluggeräts.

### 📚 Dokumentation

Die ESPFlight-Dokumentation wird praktische Anleitungen für folgende Bereiche bereitstellen:

* Aufbau des Referenz-Quadrocopters
* Verkabelung der elektronischen Komponenten
* Installation der Firmware
* Konfiguration der Flugsteuerung
* Kalibrierung der IMU
* Sicheres Testen der Motoren
* Verständnis von Arming und Failsafe
* Abstimmung der PID-Werte
* Fehlerbehebung bei häufigen Problemen
* Verständnis der Quellcodearchitektur

### 🔧 Referenzaufbau

ESPFlight wird eine bekannte und funktionsfähige Hardwarekonfiguration dokumentieren, die auf dem während der Entwicklung und der Flugtests eingesetzten Quadrocopter basiert.

Der Referenzaufbau soll Folgendes bereitstellen:

* Getestete Komponentenauswahl
* Schalt- und Verkabelungspläne
* Motor- und Propellerkonfiguration
* Hinweise zum Stromversorgungssystem
* Montageanleitungen
* Firmwarekonfiguration
* Sicherheitsprüfungen vor dem Flug
* Verfahren für die ersten Flugtests

---

## Projektstatus

> [!IMPORTANT]
> ESPFlight befindet sich in aktiver Entwicklung und wird derzeit auf die erste öffentliche Veröffentlichung vorbereitet.

Eine funktionsfähige Entwicklungsversion der Firmware wurde bereits unter realen Bedingungen auf dem aktuellen ESP8266-basierten Referenz-Quadrocopter getestet.

Die aktuelle Arbeit konzentriert sich auf die Überprüfung flugkritischer Programmteile, die Fertigstellung des Failsafe-Systems, die Vereinfachung der Projektstruktur, die Verbesserung der Dokumentation und die Vorbereitung von ESPFlight Lite auf die öffentliche Firmwareveröffentlichung.

### Aktueller Fortschritt

* [x] Funktionsfähige Flugsteuerungsfirmware
* [x] Erfolgreiche Flugtests unter realen Bedingungen
* [x] ESPFlight Lite Android-Steuerung
* [ ] Überprüfung des Failsafe bei Kommunikationsverlust abschließen
* [ ] Verhalten bei niedriger Batteriespannung vollständig überprüfen
* [ ] Firmware-Quellcode bereinigen und organisieren
* [ ] Installations- und Konfigurationsanleitungen erstellen
* [ ] Referenz-Quadrocopter dokumentieren
* [ ] Erste öffentliche Version veröffentlichen

Ein öffentliches Veröffentlichungsdatum wurde noch nicht bekannt gegeben.

---

## Geplante Repositories

| Repository           | Zweck                                     |     Status     |
| :------------------- | :---------------------------------------- | :------------: |
| `espflight-firmware` | Zentrale Flugsteuerungsfirmware           | In Entwicklung |
| `espflight-lite`     | Schlanke Android-Steuerungsanwendung      | In Entwicklung |
| `espflight-docs`     | Dokumentation und Bauanleitungen          |     Geplant    |
| `espflight-hardware` | Referenzaufbau und Verkabelungsunterlagen |     Geplant    |
| `espflight-examples` | Lern- und Entwicklungsbeispiele           |     Geplant    |

Die Namen und die Organisation der Repositories können sich vor der Veröffentlichung noch ändern.

---

## Projektgrundsätze

### Testen vor der Einstufung als stabil

Flugkritisches Verhalten sollte auf realer Hardware getestet werden, bevor es als stabil bezeichnet wird.

### Sicherheit als Grundanforderung

Arming, Motorausgabe, Kommunikationsverlust, Batteriespannung und Failsafe-Verhalten sind grundlegende Bestandteile des Systems.

### Verständlicher Quellcode

Der Quellcode soll übersichtlich genug bleiben, damit Entwickler nachvollziehen können, wie die Flugsteuerung funktioniert.

### Modulare Entwicklung

Firmware, Anwendungen, Dokumentation und Hardwareunterlagen sollen getrennt organisiert bleiben, aber als zusammenhängende Projekte funktionieren.

### Erschwingliche und zugängliche Hardware

ESPFlight soll weiterhin für leichte DIY-Projekte mit allgemein verfügbaren Komponenten geeignet sein.

### Ehrlicher Projektstatus

Experimentelle, unvollständige, getestete und stabile Funktionen sollen stets eindeutig gekennzeichnet werden.

---

## Zielgruppe

ESPFlight wird entwickelt für:

* DIY-Drohnenbauer
* Elektronikbegeisterte
* Studierende und Lehrkräfte
* Embedded-System-Entwickler
* Android-Entwickler
* Maker, die Flugsteuerungskonzepte kennenlernen möchten
* Entwickler, die mit ESP-Mikrocontrollern experimentieren

Grundkenntnisse in Elektronik, Löten, Mikrocontrollern und Embedded-Programmierung werden empfohlen.

---

## Mitwirken

ESPFlight wird derzeit auf eine öffentliche Zusammenarbeit vorbereitet.

Richtlinien für Beiträge, Codierungsstandards, Issue-Vorlagen und Testanforderungen werden zusammen mit den jeweiligen Repositories veröffentlicht.

Zukünftige Beiträge können folgende Bereiche umfassen:

* Firmwareentwicklung
* Android-Entwicklung
* Fehlerberichte
* Dokumentation
* Übersetzungen
* Hardwaretests
* Sicherheitsprüfungen
* Beispielprojekte

> [!NOTE]
> Flugkritische Änderungen sollten eindeutig als experimentell gekennzeichnet werden, bis ihr Verhalten durch kontrollierte Tests validiert wurde.

---

## Sicherheitshinweis

> [!WARNING]
> ESPFlight ist experimentelle Software. Quadrocopter können bei falscher Montage, Konfiguration, Veränderung oder Bedienung Verletzungen, Sachschäden, Batteriebrände oder Kontrollverlust verursachen.

Vor dem Testen:

* Bei Tests auf der Werkbank alle Propeller entfernen
* Das Fluggerät vor Motortests sicher befestigen
* Motorreihenfolge und Drehrichtung überprüfen
* Geeignete Akkus und Leistungskomponenten verwenden
* Arming- und Failsafe-Verhalten ohne Propeller testen
* Personen und Tiere vom Testbereich fernhalten
* Erste Flüge in einem großen und freien Bereich durchführen
* Geltende Luftfahrt- und Sicherheitsvorschriften beachten

Die Nutzung von ESPFlight erfolgt vollständig auf eigene Gefahr.

---

<div align="center">

## ESPFlight

**Ein zugänglicher Einstieg in die Entwicklung eigener Flugsteuerungssysteme.**

<br>

<a href="https://espflight.com">
  <img alt="ESPFlight besuchen" src="https://img.shields.io/badge/Besuchen-espflight.com-0284C7?style=for-the-badge&logo=googlechrome&logoColor=white">
</a>

<br><br>

<sub>ESPFlight befindet sich in aktiver Entwicklung.</sub>

</div>
