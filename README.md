# Rettenbach Schneiradar

Live-Prognose, wann am Rettenbachferner in Sölden die Schneekanonen starten können:
Rettenbach Talstation (~2'680 m) und Schwarze Schneide Mittelstation (~3'000 m).

- Statische Seite (`index.html`), lädt die Wetterdaten beim Öffnen live von [Open-Meteo](https://open-meteo.com)
- 10 Tage stündlich: ECMWF, ICON, GFS (Feuchtkugeltemperatur mit Luftdruck der Höhe)
- 30 Tage: Beschneiungs-Chance aus ECMWF- und GFS-Ensemble (an Hauptmodelle angeglichen)
- Messkorrektur mit den Wetterstationen der Panomax-Webcams (Cam 196 Rettenbach, Cam 216 Schwarze Schneid)
- Startgrenze TechnoAlpin-Propellermaschinen: ca. −2,5 °C Feuchtkugel
