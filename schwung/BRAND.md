# schwung: Brand-Paket

**Name:** schwung (immer klein geschrieben)
**Claim:** Brands in motion.
**Was wir sind:** Kleines Design-Studio in Zürich. Websites, Logos und Launch-Inhalte für kleine Marken, vom ersten Gespräch bis zur fertigen Website in etwa zehn Tagen.

## Warum "schwung"

- *Schwung* heisst Elan, Bewegung, Antrieb. Genau das soll eine Website einer Marke geben.
- Das Logo ist eine **Rampe (Quarterpipe) mit einer Kugel** am höchsten Punkt: der Moment, in dem etwas abhebt.
- Kurz, deutsch mit Charakter, international merkbar (wie "Bauhaus" oder "Zeitgeist").

Vor der Wahl geprüft, aber schon vergeben: *Firn Studio* (Agentur in Chur), *Zunder* (Studio in Linz), *Hapta* (zu nah an "Haptic Studio"), *Oktav* (zu nah an "Octav Design").

### Bevor du die Firma gründest (wichtig)

Ich konnte von hier aus nur im Web suchen, nicht in den offiziellen Registern. Prüfe deshalb selbst:

1. **Firmenname:** [zefix.ch](https://www.zefix.ch) → nach "schwung" suchen.
2. **Marke:** [swissreg.ch](https://www.swissreg.ch) (Schweiz) und [euipo.europa.eu](https://euipo.europa.eu) (EU) → Klasse 42 (Webdesign) und 35 (Werbung).
3. **Domain:** `schwung.ch` und `schwung.design` sind vergeben (sie haben schon eine Website). `schwungstudio.ch`, `schwung-studio.ch` und `schwung.studio` waren beim Test nicht belegt. Das ist ein gutes Zeichen, aber kein Beweis: vor dem Kauf beim Anbieter (z. B. hostpoint.ch) prüfen. Empfehlung: **schwungstudio.ch** (Schweizer Endung, ohne Bindestrich), E-Mail dann z. B. `andre@schwungstudio.ch`.
4. **Social Handles:** `@schwung.studio` auf Instagram, TikTok, LinkedIn und Behance reservieren, bevor du postest.

Ist der Name besetzt, hier meine Ersatz-Namen: **Hochform**, **Aufwind**, **Kinetik Studio**.

## Logo-Dateien (`brand/logo/`)

| Datei | Wofür |
|---|---|
| `schwung-logo.svg` / `-white.svg` | Hauptlogo (Zeichen + Schrift) auf hellem / dunklem Grund |
| `schwung-mark.svg` / `-white.svg` | Nur das Zeichen |
| `schwung-wordmark.svg` / `-white.svg` | Nur der Schriftzug |
| `schwung-icon-black.svg`, `-blue.svg` | App-Icon / Profilbild-Basis |
| `favicon.svg` | Browser-Tab |

Regeln: Logo nie verzerren, nicht umfärben (ausser Schwarz/Weiss), immer Abstand in der Grösse der Kugel lassen.

## Farben

| Name | Hex | Einsatz |
|---|---|---|
| Ink | `#0D0D0C` | Hauptfläche, Text |
| Paper | `#F2EFE9` | Helle Flächen (statt Weiss) |
| Schwung Blue | `#2346FF` | Die eine Signalfarbe: Buttons, Kugel, Akzente. Sparsam! |
| Blue Light | `#6F86FF` | Nur für das Akzentwort auf dunklem Grund (besser lesbar) |
| Stone | `#E4DFD5` | Ruhige Zweitfläche |

## Schrift (gratis, Google Fonts)

- **Archivo**, Condensed (font-stretch 62 %), Stärke 900, GROSSBUCHSTABEN → Headlines
- **Instrument Serif Italic** → genau ein Akzentwort pro Headline ("Brands in *motion*")
- **Archivo** normal → Fliesstext

## Social-Media-Paket (`brand/social/`)

| Datei | Plattform | Grösse |
|---|---|---|
| `avatar-black.png` (Haupt), `avatar-blue.png`, `avatar-paper.png` | Profilbild überall | 1080 × 1080 |
| `linkedin-banner.jpg` | LinkedIn, dein persönliches Profil | 1584 × 396 |
| `linkedin-company.jpg` | LinkedIn-Unternehmensseite | 1128 × 191 |
| `behance-banner.jpg` | Behance | 3200 × 410 |
| `x-header.jpg` | X / Twitter | 1500 × 500 |
| `youtube-banner.jpg` | YouTube | 2560 × 1440 |
| `ig-01-hello.jpg`, `ig-02-work.jpg`, `ig-03-offer.jpg` | Die ersten 3 Instagram-/LinkedIn-Posts | 1080 × 1350 |
| `story-cover.jpg` | Instagram-Story / TikTok-Cover | 1080 × 1920 |
| `card-front.png`, `card-back.png` | Visitenkarte (85 × 55 mm) | 1004 × 650 |

`brand-board.jpg` ist die Übersicht für Präsentationen und Behance.

## Texte für die Profile (zum Kopieren)

**LinkedIn: Headline**
> Founder of schwung, a design studio in Zürich. Brands in motion.

**LinkedIn: Info / Unternehmensseite**
> schwung is a small design studio in Zürich. We make websites, logos and launch content for small brands, usually from first call to live site in about ten days. We use AI for code and images and say so openly; every design decision is made by a person.

**Instagram / TikTok: Bio** (max. 150 Zeichen)
> Brands in motion.
> Design studio in Zürich.
> Logo and website in about 10 days.

**Behance: Über mich**
> schwung is a small design studio in Zürich. Websites, logos and launch content for small brands.

**Name überall gleich:** `schwung`, Handle `@schwung.studio`

## E-Mail-Signatur

```html
<table cellpadding="0" cellspacing="0" style="font-family:Arial,sans-serif;font-size:13px;color:#0d0d0c">
  <tr><td style="padding-bottom:6px"><strong>André Ruchenstein</strong>, Founder</td></tr>
  <tr><td style="padding-bottom:10px;color:#6f6a62">schwung, Zürich</td></tr>
  <tr><td><a href="https://yourdomain.ch" style="color:#2346ff;text-decoration:none">yourdomain.ch</a></td></tr>
</table>
```

## Website (`schwung/index.html`)

Eine Seite mit: Startbereich, SOLUM als Fallstudie, Leistungen, Ablauf in 10 Tagen, Preise, Fragen (inkl. ehrlicher Antwort zu KI), Kontaktformular. Das Formular öffnet das E-Mail-Programm des Besuchers mit der fertigen Nachricht, funktioniert also auch ohne Server.

**Noch zu ersetzen, bevor sie live geht:**
- `hello@yourdomain.ch` (auf Website, Visitenkarte und Signatur) → deine echte E-Mail, sobald die Domain steht
- Impressum und Datenschutz (in der Schweiz Pflicht) fehlen noch. Sobald du Firmenname und Adresse hast, baue ich die Seiten und verlinke sie im Footer. Social-Links kommen dazu, sobald die Profile existieren.
- Die Preise sind Vorschläge für den Start. Passe sie an, wie du dich wohlfühlst.
- Im ZIP für Netlify ist SOLUM schon enthalten (`/solum/`), der Link der Fallstudie funktioniert dort.
