# Rechenzug

Mathematisches Schiebe-Puzzle. Wische über das Feld, Zahl trifft Operator, es wird gerechnet.
Eine einzige Datei, kein Build-Schritt, keine Abhängigkeiten, kein Tracking.

## Modi

- **Lernen**: vier geführte Mini-Rätsel für Einsteiger (Wischen, Rechnen, Reihenfolge, Teilen).
- **Daily**: ein Rätsel pro Tag, gleich für alle, Schwierigkeit Schwer.
- **Endlos**: neues Rätsel per Knopf, Stufen Leicht / Mittel / Schwer / Master / Overkill.

Beim ersten Start öffnet sich die Anleitung automatisch, danach über den „?“-Knopf.

## Ergebnis teilen (Daily)

Nach dem Lösen zeigt das Daily eine Ergebniskarte: Zugzahl, Urteil und ein Feld pro Zug
(grün = gerechnet, grau = nur geschoben, gelb = rückgängig, rot = zurückgesetzt).
„Teilen“ öffnet das Share-Sheet des Geräts, „Kopieren“ legt den Text in die Zwischenablage.
Bei sehr langen Läufen zeigt die Karte die letzten 32 Felder, davor steht „… +N“ für die ausgeblendeten.
Die Richtungen der Züge stehen bewusst nicht im Text, damit der Lösungsweg kein Spoiler ist.
Das Ergebnis wird lokal gespeichert und ist nach einem Neuladen wieder da.

## Marke

Name, Claim, Farben, Logo-Regeln: siehe `brand.md`. Das Spiel bringt Favicon und Logo selbst mit (eingebettet),
die übrigen Dateien (Startbildschirm-Symbole, Vorschaubild, Manifest) liegen daneben.

## Dateien für den Upload

Alle Dateien liegen flach im Hauptordner, damit man sie am Handy gemeinsam auswählen kann:

`index.html`, `manifest.webmanifest`, `favicon.ico`, `favicon.svg`, `favicon-32.png`, `apple-touch-icon.png`,
`icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `og-image.png`
(optional zum Aufbewahren: `logo-mark.svg`, `logo-horizontal-dark.svg`, `logo-horizontal-light.svg`, `brand.md`, `README.md`).

Das Spiel läuft auch nur mit `index.html`, dann fehlen Startbildschirm-Symbol und Vorschaubild.

**Eine Zeile anpassen:** in `index.html` steht bei `og:image` die Adresse
`https://thssnm.github.io/rechenzug/og-image.png`. Sie muss zur echten Adresse passen
(`https://<benutzer>.github.io/<repo>/og-image.png`), sonst zeigt die Linkvorschau kein Bild.

## Deploy auf GitHub Pages

1. Repo anlegen, `index.html` in den Root hochladen.
2. Im Repo: Settings → Pages → Branch: `main` / `(root)` → Save.
3. URL nach kurzer Zeit unter `https://<username>.github.io/<reponame>/`.

## Bekannte offene Punkte

- Quadrat-Kombinationen können große Zahlen erzeugen, Kachel-Schrift skaliert noch nicht mit der Ziffernanzahl.
- Overkill braucht beim Generieren auf dem Handy teilweise über eine Sekunde.
- Endlos-Rätsel werden nicht gespeichert (Reload = neues Rätsel).
