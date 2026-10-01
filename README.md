# Rettenbach Schneiradar

Live-Prognose, wann am Rettenbachferner in Sölden die Schneekanonen starten können:
Rettenbach Talstation (~2'680 m) und Schwarze Schneide Mittelstation (~3'000 m).

- Statische Seite (`index.html`), lädt die Wetterdaten beim Öffnen live von [Open-Meteo](https://open-meteo.com)
- 10 Tage stündlich: ECMWF, ICON, GFS (Feuchtkugeltemperatur mit Luftdruck der Höhe)
- 30 Tage: Beschneiungs-Chance aus ECMWF- und GFS-Ensemble (an Hauptmodelle angeglichen)
- Messkorrektur mit den Wetterstationen der Panomax-Webcams (Cam 196 Rettenbach, Cam 216 Schwarze Schneid)
- Startgrenze TechnoAlpin-Propellermaschinen: ca. −2,5 °C Feuchtkugel

## Idee für ein Folgeprojekt: Heiz-Prognose

Dasselbe Prinzip (Prognose → Schwelle → Zeitleiste «wann ist es so weit?») für die Heizung im eigenen Haus,
mit eigener Seite (mobile-first) und eigenem Repo. Statt «Feuchtkugel ≤ −2,5 °C → Kanone läuft» z.B.
«Tagesmittel unter Heizgrenze → heizen nötig».

Benötigte Angaben, bevor es losgeht:

- **Standort:** Ort/Höhe für die Wetterdaten
- **Heizung:** Art (Wärmepumpe, Pellets, Öl, Gas, Holz), Heizgrenze, Trägheit des Hauses (Fussbodenheizung/Radiatoren, Bauweise)
- **Heizautomatik:** Marke/Modell, ob App oder Schnittstelle zum Auslesen (Innen-/Vorlauftemperatur)
- **Ziel:** nur «wann heizen?» oder auch Verbrauch/Kosten
- **Optional:** Photovoltaik, um Sonne und Heizzeiten abzustimmen

## Mögliche Verbesserungen Schneiradar

- Feineres Modell für die ersten 2 Tage (z.B. ICON-D2, ~2 km)
- Messkorrektur getrennt für Tag und Nacht
- Klimatologie (Messwerte der letzten Jahre) für den 30-Tage-Kalender
- Genaue Höhe der Mittelstation und der Webcam-Sensoren nachtragen
