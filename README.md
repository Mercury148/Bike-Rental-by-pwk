# Bike-Rental-by-pedalwerk
Userinterface for renting eBikes, keeping track of current rentals, needed repairs

## Fahrradverleih

Oberfläche für einen Riese & Müller Fahrradverleih: Inventar mit Filtern und eine anonyme Kundenkartei.

## Funktionen

- **Inventar:** Karten mit Bild, Modellname, Rahmengröße, passenden Körpergrößen, Drehmoment (Nm), Akku (Wh) und Schaltung. Filter nach Suche, Bauart, Körpergröße, Schaltung und Status (verfügbar, verliehen, Werkstatt). Räder anlegen, bearbeiten und löschen.
- **Kundenkartei:** „Neuer Kunde“ erzeugt eine zufällige Nummer aus einem Buchstaben, einem Minus und fünf Ziffern (z. B. `K-48213`). I und O werden nicht verwendet, damit sie nicht mit 1 und 0 verwechselt werden. Klarnamen werden nicht gespeichert, nur optional Körpergröße und eine Notiz.
- **Farben & Bilder:** Jede Farbe wird einmal mit Bild angelegt. Räder in dieser Farbe zeigen das Bild automatisch, ein eigenes Foto pro Rad ist optional.
- **Verleih:** Räder an eine Kundennummer verleihen und zurückbuchen, mit Hinweis, ob die Körpergröße zum Rahmen passt.

## Betrieb

Die App ist eine einzelne Datei (`index.html`) ohne Build-Schritt.

- **In Claude veröffentlicht:** Inventar und Kartei liegen in einer gemeinsamen Datenbank, Fotos können hochgeladen werden.
- **Direkt im Browser oder über GitHub Pages:** Die App läuft im lokalen Modus. Daten werden nur im `localStorage` des jeweiligen Browsers gespeichert, der Foto-Upload ist ausgeblendet. Zum Start sind drei Beispielräder enthalten.

Die Beispieldaten sind Richtwerte und sollten durch den echten Bestand ersetzt werden.