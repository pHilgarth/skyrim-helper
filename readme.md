# Skyrim Hearthfire Building Helper

Ein einfaches, webbasiertes Hilfstool für *The Elder Scrolls V: Skyrim - Hearthfire*. Es hilft Spielern dabei, den Überblick über benötigte Baumaterialien für verschiedene Bauprojekte und Räume zu behalten.

## Features

- **Projekt-Auswahl via Dropdown:** Sobald ein Bauprojekt oder ein Raum ausgewählt wird, wird er direkt zur Bautabelle hinzugefügt.
- **Mengenanpassung & Entfernen:** Anzahl der Bauprojekte anpassen oder nicht mehr benötigte Projekte per Klick entfernen.
- **Automatische Berechnung:** Summiert alle benötigten Baumaterialien (wie Holz, Bruchstein, Schloss, Scharnier etc.) aus der Datenbasis auf.
- **Interaktive Fortschrittsanzeige:** Eingabe bereits gesammelter Materialien inklusive visueller Fortschrittsleiste.

---

## Voraussetzungen & Installation

Da das Tool Daten dynamisch aus einer Textdatei (`hearthfire.txt`) lädt, greifen bei modernen Browsern Sicherheitsbeschränkungen (CORS / Same-Origin-Policy), wenn die `index.html` bzw. `hearthfire.html` direkt als lokale Datei (`file://...`) geöffnet wird.

**Für die Nutzung ist daher ein lokaler Webserver erforderlich.**

### Option 1: VS Code (Live Server Extension) – *Empfohlen*
1. Repository klonen oder als ZIP herunterladen.
2. Den Ordner in **Visual Studio Code** öffnen.
3. Die Extension **Live Server** (von Ritwick Dey) installieren.
4. Unten rechts auf **"Go Live"** klicken oder Rechtsklick auf `hearthfire.html` $\rightarrow$ **Open with Live Server**.

### Option 2: Python (ohne zusätzliche Tools)
Falls Python installiert ist, im Projektordner folgendes Terminal / PowerShell öffnen:

```bash
# Python 3
python -m http.server 8000