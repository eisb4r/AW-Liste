AW-AUFTRÄGE – WEB-APP FÜR IPHONE UND MAC

Dateien:
- index.html: die App
- manifest.webmanifest: Installationsdaten
- sw.js: Offline-Cache
- icon-192.png / icon-512.png: App-Symbole

FUNKTIONEN
Tag, Woche, Monat und Tagesübersicht; Aufträge anlegen, bearbeiten und löschen;
rotes Ausrufezeichen zum Markieren; markierte Aufträge stehen oben; AW-Summen;
Monatsübersicht über den Druckdialog als PDF speichern.

DATEN UND OFFLINE
Die Aufträge werden in localStorage im jeweiligen Browser gespeichert.
iPhone und Mac sind getrennt; es gibt keine Synchronisierung oder Cloud-Sicherung.
Die App muss einmal vollständig über eine HTTPS-Adresse geöffnet werden, damit
der Service Worker die App-Dateien zwischenspeichern kann. Danach funktioniert
die App in der Regel auch ohne Internet. Die erste Installation benötigt Internet.

EINRICHTUNG (BEISPIEL GITHUB PAGES)
1. GitHub-Konto öffnen/erstellen: https://github.com
2. Neues Repository erstellen, z.B. aw-auftraege.
3. Diese fünf App-Dateien ins Hauptverzeichnis (root) hochladen.
4. Repository Settings > Pages öffnen.
5. Bei Build and deployment als Quelle „Deploy from a branch“ wählen,
   Branch „main“ und Ordner „/(root)“, dann Save.
6. Warten, bis GitHub Pages eine HTTPS-Adresse anzeigt. Diese Adresse öffnen.

IPHONE
1. HTTPS-Adresse in Safari öffnen und vollständig laden lassen.
2. Safari: Teilen > Zum Home-Bildschirm > Hinzufügen.
3. Die App einmal online starten, damit der Offline-Cache eingerichtet wird.

MAC
1. Dieselbe HTTPS-Adresse in Safari oder einem anderen aktuellen Browser öffnen.
2. Als Lesezeichen sichern. Je nach Browser kann die Web-App auch installiert werden.

PDF
„Monatsübersicht als PDF“ öffnet den Druckdialog. Am Mac „PDF“ > „Als PDF sichern“.
Am iPhone im Druck-/Teilen-Dialog die PDF-Vorschau öffnen und sichern.

WICHTIGE HINWEISE
- Das ist ein Web-Neuaufbau anhand der im Gespräch genannten Funktionen, keine
  automatische Konvertierung des SwiftUI-Quellcodes.
- Bestehende Daten der Xcode-App werden nicht importiert.
- Browserdaten löschen kann die lokal gespeicherten Aufträge entfernen.
- Nicht die Auftragsdaten in GitHub hochladen: sie bleiben lokal im Browser.
