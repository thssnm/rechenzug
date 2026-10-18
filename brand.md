# Rechenzug – Marke

**Name:** Rechenzug (Rechen + Zug: ein Rechenschritt, ein Spielzug, ein Zug nach vorn).
**Claim:** Wischen. Rechnen. Treffen.
**Zeile für Läden und Vorschauen:** Täglich ein neues Rechenrätsel.

## Die Idee des Zeichens

Zwei Kacheln treffen sich: blau ist die **Zahl**, orange der **Operator**. Wo sie sich überlappen,
entsteht das **Ergebnis**, in Grün. Das ist die Spielregel in einem Bild und funktioniert noch bei 16 px.

## Farben

| Rolle | Farbe | Hex | Einsatz |
|---|---|---|---|
| Tinte | Fast Schwarz | `#111318` | Hintergrund, Text auf Hell |
| Fläche | Dunkelgrau | `#1b1e26` | Karten, leere Felder |
| Zahl | Hellblau | `#7ec4ff` | Zahlenkacheln, „zug“ im Logo auf Dunkel |
| Operator | Bernstein | `#f0b64c` | Operatorkacheln |
| Ergebnis | Grün | `#5fd884` | Verschmelzung, Erfolg |
| Blau tief | Mittelblau | `#2a7fd4` | „zug“ im Logo auf **hellem** Grund (Hellblau hat dort zu wenig Kontrast) |
| Text | Fast Weiß | `#f0f1f4` | Text auf Dunkel |
| Text leise | Grau | `#9aa0ad` | Nebentext |

## Schrift

Wortmarke: **Poppins Bold** (SIL Open Font License), als Kurven eingebettet, also nirgends als Schrift
nötig. Im Spiel selbst läuft die System-Schrift des Geräts.
„Rechen“ in Text-/Tintenfarbe, „zug“ in Blau (auf Dunkel `#7ec4ff`, auf Hell `#2a7fd4`).

## Dateien

| Datei | Wofür |
|---|---|
| `logo-horizontal-dark.svg` | Logo für dunklen Grund (Standard) |
| `logo-horizontal-light.svg` | Logo für hellen Grund |
| `logo-mark.svg` | Nur das Zeichen, mit eigenem dunklem Grund (Profilbild, Store) |
| `favicon.svg`, `favicon.ico`, `favicon-32.png` | Browser-Tab (vereinfachtes Zeichen mit größeren Kacheln) |
| `apple-touch-icon.png` | iPhone/iPad Startbildschirm (180 px, ohne Rundung, iOS rundet selbst) |
| `icon-192.png`, `icon-512.png` | Android-Symbole |
| `icon-maskable-512.png` | Android-Symbol, das jede Form (Kreis, Squircle) verträgt |
| `og-image.png` | Vorschaubild beim Teilen eines Links (1200 × 630) |
| `manifest.webmanifest` | Name, Farben und Symbole für „Zum Startbildschirm hinzufügen“ |

## Regeln

- **Schutzraum:** rund um das Zeichen mindestens ein Viertel seiner Breite frei lassen.
- **Mindestgröße:** Logo mit Wortmarke ab 120 px Breite, Zeichen ab 24 px. Darunter das Favicon nehmen.
- Reihenfolge der Kacheln nicht ändern: **Blau liegt oben links, Orange unten rechts**, Grün in der Mitte.
- Nicht dehnen, nicht drehen, keine Farbverläufe, keine anderen Farben für die Kacheln.
- Auf hellem Grund immer die Light-Variante nehmen, nie die Dunkel-Variante mit hellem Text.
