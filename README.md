## Fix 7.1 – Kategorien
Kategorien werden jetzt zuverlässig in IndexedDB gespeichert, nach dem Anlegen sofort in der Galerie angezeigt und unmittelbar in allen Kategorie-Auswahllisten verfügbar.

# Meine Ausgaben – lokale Finanz-App

Eine mobile-first Progressive Web App zur lokalen Erfassung und Analyse von Einnahmen und Ausgaben. Keine Serverdatenbank, keine Registrierung und keine feste Kategorie-Liste.

## Funktionen

- Kalender mit anklickbaren Tagen und Mehrfach-Eingabe
- Einnahmen und Ausgaben
- frei anlegbare Kategorien
- automatisch gelernte Händler und Zahlungsarten
- Suche, Zeitraum-, Kategorie- und Händlerfilter
- Monats-, Jahres-, Händler-, Kategorie- und Wochentagsanalysen
- automatische Erkenntnisse zu Trends und Ausgabemustern
- Budgets pro eigener Kategorie
- wiederkehrende Buchungen
- JSON-Vollbackup und Import für Gerätewechsel
- CSV-Export
- IndexedDB für lokale Daten
- Offline-PWA für GitHub Pages

## GitHub Pages

1. Inhalt dieses Ordners in ein GitHub-Repository hochladen.
2. GitHub → Settings → Pages öffnen.
3. Als Quelle `Deploy from a branch` auswählen.
4. Branch `main` und Ordner `/ (root)` auswählen.
5. Nach dem Deployment die angezeigte GitHub-Pages-Adresse öffnen.
6. Auf Android/Chrome bzw. iPhone/Safari kann die Seite anschließend zum Startbildschirm hinzugefügt werden.

Die App verwendet ausschließlich relative Pfade und benötigt keinen Build-Schritt.

## Datenschutz und Datenhaltung

Die Buchungen werden im Browser im IndexedDB-Speicher des jeweiligen Geräts gespeichert. GitHub Pages hostet nur die statischen App-Dateien. Die App überträgt deine Buchungen nicht an einen eigenen Server.

**Wichtig beim Gerätewechsel:** Vor dem Wechsel unter `Einstellungen → JSON-Backup exportieren` ein Backup erstellen und auf dem neuen Gerät über `JSON-Backup importieren` einspielen.

## Projektstruktur

- `index.html` – komplette App
- `manifest.webmanifest` – PWA-Metadaten
- `sw.js` – Offline-Service-Worker
- `icon.svg` – App-Icon
- `README.md` – diese Anleitung

## Hinweis

Das Projekt ist als persönliche lokale Ausgaben-App gedacht. Backups solltest du selbst sicher aufbewahren.
