# Ruchenstein: Brand-Paket

**Name:** Ruchenstein (im Logo in Grossbuchstaben, im Text normal geschrieben)
**Slogan:** Websites mit Fundament.
**Was ich mache:** Websites und Logos für kleine Firmen in Zürich. Zum Fixpreis, in rund zehn Tagen live.
**Wer:** André Ruchenstein, allein. Auf der Website und in Posts immer in der Ich-Form.

## Warum dieser Auftritt

- **Zielgruppe:** kleine Firmen in Zürich (Läden, Cafés, Praxen, Handwerk, Gründer). Sie wollen schnell online, einen klaren Preis und eine echte Person als Ansprechpartner. Deshalb: Deutsch, Ich-Form, feste Preise, keine erfundenen Zahlen.
- **Name:** dein eigener Nachname. Er ist einmalig, wirkt seriös und zeigt, dass hinter der Arbeit ein Mensch steht.
- **Logo:** RUCHEN / STEIN in zwei Zeilen. Der schwarze Block ist der Stein: Er füllt die Lücke nach STEIN, und das Wort wird zu einem vollen Rechteck. Das ist das Fundament aus dem Slogan.
- **Stil:** Schweizer Plakatstil. Riesige schmale Schrift, Schwarz und Weiss, viel Fläche. Bewusst keine Verläufe, kein Glanz, keine kursive Zierschrift.

### Bevor du die Firma gründest

1. **Firmenname:** auf [zefix.ch](https://www.zefix.ch) nach „Ruchenstein“ suchen. Als Einzelfirma muss dein Nachname sowieso im Namen stehen, das passt also.
2. **Domain:** zum Beispiel bei hostpoint.ch nach `ruchenstein.ch` suchen. Ist sie vergeben, sind `andreruchenstein.ch` oder `ruchenstein.studio` gute Alternativen. Ich konnte das von hier aus nicht prüfen.
3. **Social Handles:** `@ruchenstein` auf Instagram, LinkedIn und Behance reservieren, bevor du postest.

## Logo-Dateien (`logo/`)

| Datei | Wofür |
|---|---|
| `ruchenstein.svg` / `-white.svg` | Hauptlogo, zweizeilig, auf hellem / dunklem Grund |
| `ruchenstein-zeile.svg` / `-white.svg` | Einzeilig, für sehr flache Stellen (E-Mail-Signatur, Rechnung) |
| `icon-ink.svg`, `icon-white.svg` | Quadratisch, Basis für Profilbilder |
| `favicon.svg` | Browser-Tab (R mit Stein) |

Regeln: Logo nie verzerren, nur Schwarz oder Weiss, rundherum mindestens so viel Abstand lassen, wie der Stein hoch ist. Der Stein bleibt immer bündig mit dem N darüber.

## Farben

| Name | Hex | Einsatz |
|---|---|---|
| Ink | `#111110` | Text, Logo, dunkle Flächen, Buttons |
| Weiss | `#FFFFFF` | Hauptfläche |
| Stein | `#E4E0D8` | Ruhige Zweitfläche (Kontakt, Angebote) |
| Stein hell | `#F1EFEA` | Kleine Flächen, Karten |

Keine zusätzliche Akzentfarbe. Hervorgehoben wird mit Grösse und Schwarz, nicht mit Farbe.

## Schrift (gratis, Google Fonts)

- **Archivo Extra Condensed Black** (font-stretch 62.5 %, Stärke 900), GROSSBUCHSTABEN, für Titel und Preise
- **Archivo** normal für Fliesstext
- Gestaltungsmittel: Ein Titel darf mit einem schwarzen Block enden, der die Zeile füllt (wie im Logo). Pro Seite oder Bild höchstens einmal.

## Social-Media-Paket (`social/`)

| Datei | Plattform | Grösse |
|---|---|---|
| `avatar-ink.png` (Haupt), `avatar-white.png`, `avatar-stone.png` | Profilbild überall | 1080 × 1080 |
| `linkedin-banner.jpg` | LinkedIn, persönliches Profil (links frei für dein Foto) | 1584 × 396 |
| `linkedin-company.jpg` | LinkedIn-Unternehmensseite | 1128 × 191 |
| `behance-banner.jpg` | Behance | 3200 × 410 |
| `x-header.jpg` | X / Twitter | 1500 × 500 |
| `youtube-banner.jpg` | YouTube (Inhalt im sicheren Bereich) | 2560 × 1440 |
| `ig-01-hallo.jpg`, `ig-02-arbeit.jpg`, `ig-03-angebot.jpg` | Die ersten 3 Posts für Instagram und LinkedIn | 1080 × 1350 |
| `story-cover.jpg` | Instagram-Story / TikTok-Cover | 1080 × 1920 |
| `card-front.png`, `card-back.png` | Visitenkarte (85 × 55 mm) | 1004 × 650 |

`brand-board.jpg` ist die Übersicht für Präsentationen und Behance.

## Texte für die Profile (zum Kopieren)

**LinkedIn: Headline**
> Websites und Logos für kleine Firmen in Zürich. Fixpreis, in rund zehn Tagen live.

**LinkedIn: Info**
> Ich bin André Ruchenstein und baue Websites und Logos für kleine Firmen in Zürich. Du sprichst von der ersten Nachricht bis zum Livegang mit mir. Für Code und Bilder nutze ich KI und sage das offen, dadurch bin ich schneller und günstiger. Was auf deine Website kommt, entscheide ich selbst.

**Instagram: Bio** (max. 150 Zeichen)
> Websites mit Fundament.
> Websites und Logos für kleine Firmen in Zürich.
> Fixpreis, in rund 10 Tagen live.

**Behance: Über mich**
> Websites und Logos für kleine Firmen in Zürich.

## E-Mail-Signatur

```html
<table cellpadding="0" cellspacing="0" style="font-family:Arial,sans-serif;font-size:13px;color:#111110">
  <tr><td style="padding-bottom:4px"><strong>André Ruchenstein</strong></td></tr>
  <tr><td style="padding-bottom:10px;color:#5c5a55">Websites und Logos, Zürich</td></tr>
  <tr><td><a href="https://deinedomain.ch" style="color:#111110">deinedomain.ch</a></td></tr>
</table>
```

## Website (`ruchenstein/index.html`)

Aufgebaut wie die Website eines Designers, nicht wie eine Verkaufsseite: oben ein paar Sätze in normaler Schrift, dann deine Arbeiten mit grossen Bildern, Über mich, wie du arbeitest mit den Preisen als einfache Liste, und Kontakt per E-Mail. Kein Formular, keine Preistabelle, keine riesigen Slogan-Titel.

**Noch zu ersetzen oder zu ergänzen, bevor sie live geht:**
- `hallo@deinedomain.ch` (Website, Posts, Visitenkarte) → deine echte Adresse, auf Wunsch auch Telefon
- Ein Foto von dir und ein paar echte Sätze über dich für „Über mich“
- AML Revisions als zweites Projekt, sobald dein Vater einverstanden ist
- Impressum und Datenschutz (in der Schweiz Pflicht), sobald du Firmenname und Adresse hast
- Die Preise sind Vorschläge für den Start. Passe sie an, wie du dich wohlfühlst.
