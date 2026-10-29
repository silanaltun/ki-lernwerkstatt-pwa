# KI-Lernwerkstatt

Eine Progressive Web App zum Lernen und Ausprobieren an der Schnittstelle von Betriebswirtschaft und künstlicher Intelligenz.

**App öffnen:** [silanaltun.github.io/ki-lernwerkstatt-pwa](https://silanaltun.github.io/ki-lernwerkstatt-pwa/)

## Das steckt drin

- **Karteikarten:** Zehn vorbefüllte Fragen zu KI und BWL sowie die Möglichkeit, eigene Karten hinzuzufügen und den Lernstand zu markieren.
- **ROI- und Token-Kostenrechner:** Zwei Modellszenarien anhand veränderbarer Annahmen vergleichen, monatliche Ersparnis, ROI und Amortisationsdauer schätzen. Die voreingestellten Preise sind Beispiele und keine aktuellen Anbieterpreise.
- **Notizen und Backup:** Notizen, Karten, Lernstand und Rechnerwerte bleiben lokal im Browser. Sie können als JSON exportiert und auf einem anderen Gerät importiert werden.
- **Offline und installierbar:** Nach dem ersten vollständigen Laden über HTTPS kann die App dank Service Worker auch ohne Internetverbindung verwendet werden. Browserdaten können beim Löschen des Browserspeichers verloren gehen; ein regelmäßiger Export dient als Backup.

## Installation

Die App zunächst über den Link oben online öffnen. Auf **iPhone oder iPad** in Safari auf **Teilen → Zum Home-Bildschirm** tippen. Auf **Android** im Browsermenü **App installieren** oder **Zum Startbildschirm hinzufügen** wählen. Auf Desktop-Systemen kann ein unterstützter Browser eine Installationsoption in der Adressleiste oder im Menü anbieten.

## Lokal starten

Einen lokalen Webserver im Projektordner starten, zum Beispiel mit `python -m http.server 8000`, und anschließend `http://localhost:8000/` öffnen. Für den Service Worker ist HTTPS oder localhost nötig; ein direkter `file://`-Aufruf bietet die Offline-Installation nicht.

Die App verwendet HTML, CSS und JavaScript ohne externe Bibliotheken oder Tracker. `manifest.webmanifest` beschreibt die Installation und `sw.js` speichert die App-Dateien für die Offline-Nutzung. Die Icons basieren auf dem Avatar der Autorin.
