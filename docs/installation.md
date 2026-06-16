# Installation

Diese Anleitung richtet sich an Anwender und Kunden-IT.

## Voraussetzungen

- Windows 10 oder neuer.
- Java/JRE, damit die KoSIT-XRechnung-Prüfung ausgeführt werden kann.
- Microsoft ODBC Driver 17 oder 18 for SQL Server.
- Netzwerkzugriff auf den EHFleet/FLEETFUHRPARK-IM-SQL-Server.
- Servername, Datenbankname, Benutzername und Passwort für die EHFleet-Datenbank.

## Download

1. Release `latest` öffnen: [Aktuelle Testversion](https://github.com/harzmann/fleet-erechnung-hybridviewer-docs/releases/tag/latest)
2. ZIP-Datei herunterladen und in einen lokalen Programmordner entpacken.
3. Optional die `.sha256`-Datei herunterladen und die Prüfsumme vergleichen.

```powershell
Get-FileHash -Algorithm SHA256 ".\FleetXRechnungHybridViewer_0.1.0_<commit>.zip"
```

## Manuelle Installation

1. ZIP-Datei entpacken.
2. `FleetXRechnungHybridViewer.exe` starten.
3. Bei Windows-SmartScreen die Ausführung der internen Testversion bestätigen.
4. Menü `Einstellungen -> EHFleet-DB Einstellungen...` öffnen.
5. SQL-Server, Datenbank, Benutzer und Passwort eintragen.
6. Verbindung testen und speichern.

## Update

1. Anwendung schließen.
2. Neue ZIP-Datei herunterladen und entpacken.
3. Vorhandene EXE ersetzen oder einen neuen Programmordner verwenden.
4. Anwendung starten und Verbindungstest durchführen.

Lokale Einstellungen und verschlüsselte Passwortdateien bleiben auf dem jeweiligen Client. Bei einem neuen Programmordner müssen die Datenbankeinstellungen gegebenenfalls erneut gesetzt werden.

## Funktionstest

- Hybrid-PDF öffnen und prüfen, ob PDF und strukturierte Rechnungsdaten angezeigt werden.
- XML-Datei direkt öffnen.
- `EHFleet -> XRechnung prüfen...` ausführen und den Validierungsreport anzeigen.
- `EHFleet -> Stammdaten -> Lieferanten...`, `Fahrzeuge...` und `Kategorien...` öffnen.
- XRechnung-Ansicht öffnen, Positionen zuordnen und Speichern testen.
- Druck- und Exportfunktionen stichprobenartig prüfen.

## Rollback

Falls ein Rollback notwendig ist:

1. Anwendung schließen.
2. Vorherige ZIP-Version aus einem gesicherten Release oder Backup entpacken.
3. EXE ersetzen oder den alten Programmordner wieder verwenden.
4. Datenbankverbindung und XRechnung-Funktionstest erneut prüfen.
