# Änderungen

Build-Metadaten werden nach jedem automatischen App-Build auf der Startseite aktualisiert.

# ChangeLog

## 2026-06-16 - 0.1.0

### Anwendung
- Hybrid-PDF-Viewer für XRechnung/EN16931 mit paralleler PDF-, XML- und strukturierter Datenansicht.
- Direkter Import von Hybrid-PDFs und XML-Dateien inklusive Drag & Drop.
- Extraktion eingebetteter XML-Rechnungen aus Hybrid-PDFs mit `pikepdf`.
- KoSIT-Validator-Integration mit HTML-Reportanzeige.
- Druck- und Exportfunktionen für PDF, XML und strukturierte Rechnungsansicht.

### EHFleet-Integration
- SQL-Server-Anbindung über `pyodbc` mit lokal speicherbaren Verbindungseinstellungen.
- Stammdaten-Dialoge für Lieferanten, Fahrzeuge und Kategorien.
- XRechnung-Fachansicht für Fremdrechnungskopf, Headerdaten und Positionen.
- Zuordnung von Rechnungspositionen zu Kategorien und Fahrzeugen.
- Heuristische ML-/Matching-Unterstützung für Lieferanten- und Positionszuordnungen.
- Persistenzlogik für Fremdrechnungen, Positionen, Steuerdaten und Dokumentdaten.

### Betrieb und Deployment
- PyInstaller-Spec für den Windows-EXE-Build mit App-Icon.
- Validator-Ressourcen werden in den EXE-Build aufgenommen; Reports und temporäre Dateien liegen im EXE-Betrieb in einem beschreibbaren lokalen App-Verzeichnis.
- Öffentliches MkDocs-Dokumentationsportal mit Download, Installation, Handbuch und Changelog.
