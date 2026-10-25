# Dino Horizon – Chrome Dino-inspirierter Offline Runner

Ein vollständig lokales Paket des Chromium T-Rex Runner (Chromium 98.0.4758.55).
Keine Installation, kein Server und keine Internetverbindung sind nötig. Die
Spielansicht verwendet durchgehend Chromiums 2×-Sprite-Atlas und eine 2×-Canvas-
Auflösung. Das bewahrt alle originalen Animationsabläufe bei einer deutlich
ruhigeren Darstellung. Ein farbiger Wüstenhintergrund ergänzt die Spielszene.

> Hinweis: Dino Horizon ist ein inoffizielles, eigenständiges Fan-Projekt und
> ist nicht mit Google oder Chrome verbunden bzw. von ihnen unterstützt.

## Starten

- macOS: `start.command` doppelklicken (beim ersten Mal ggf. Rechtsklick → Öffnen).
- Jedes Betriebssystem: `index.html` in einem modernen Browser öffnen.

Steuerung: Leertaste / ↑ / Antippen springt, ↓ duckt sich, Enter startet nach
einem Absturz erneut.

Die ursprüngliche Chromium-Spielquellen liegen unverändert in `offline.js` und
`offline-sprite-definitions.js`. Der Browser-Wrapper in `index.html` stellt nur
die lokale Startseite und das Sprite-Sheet bereit. Sounds sind im Paket als Originaldateien enthalten, aber
absichtlich nicht aktiviert: Chromium bettet sie in seiner Fehlerseite als
Daten-URLs ein; das Deaktivieren macht den Start direkt per `file://` in jedem
Browser robust.

## Lizenz

Die eigenen Wrapper- und Design-Dateien sind unter MIT lizenziert. Übernommene
Chromium-Spielbestandteile bleiben BSD-3-Clause-lizenziert. Alle Hinweise stehen
vollständig in `LICENSE`.
