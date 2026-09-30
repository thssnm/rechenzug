# Rechenzug

Mathematisches Schiebe-Puzzle. Zahl trifft Operator, sie verschmelzen zur berechneten Zahl.
Daily-Modus (ein Rätsel pro Tag, gleich für alle) und Endlos-Modus (neues Rätsel per Knopf).

Eine einzige Datei, kein Build-Schritt, keine Abhängigkeiten, kein Tracking.

## Deploy auf GitHub Pages

1. Repo anlegen, `index.html` in den Root hochladen.
2. Im Repo: Settings → Pages → Branch: `main` / `(root)` → Save.
3. URL nach kurzer Zeit unter `https://<username>.github.io/<reponame>/`.

## Bekannte offene Punkte

- Generator kann bei Quadrat-Kombinationen große Zahlen erzeugen (z. B. 25² = 625) — Tile-Schrift skaliert noch nicht mit der Ziffernanzahl.
- Kein Undo, nur Reset auf Rätselstart.
- Keine Persistenz für Endlos-Rätsel (Reload = neues Rätsel).
