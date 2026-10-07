# schwung: Brand-Paket

**Name:** schwung (immer klein geschrieben)
**Claim:** Brands in motion.
**Was wir sind:** Design-Studio aus Zürich für Websites, Markenauftritte und Launch-Pakete. Mit KI schnell, mit Geschmack gut.

## Warum "schwung"

- *Schwung* heisst Elan, Bewegung, Antrieb. Genau das soll eine Website einer Marke geben.
- Das Logo ist eine **Rampe (Quarterpipe) mit einer Kugel** am höchsten Punkt: der Moment, in dem etwas abhebt.
- Kurz, deutsch mit Charakter, international merkbar (wie "Bauhaus" oder "Zeitgeist").

Vor der Wahl geprüft, aber schon vergeben: *Firn Studio* (Agentur in Chur), *Zunder* (Studio in Linz), *Hapta* (zu nah an "Haptic Studio"), *Oktav* (zu nah an "Octav Design").

### Bevor du die Firma gründest (wichtig)

Ich konnte von hier aus nur im Web suchen, nicht in den offiziellen Registern. Prüfe deshalb selbst:

1. **Firmenname:** [zefix.ch](https://www.zefix.ch) → nach "schwung" suchen.
2. **Marke:** [swissreg.ch](https://www.swissreg.ch) (Schweiz) und [euipo.europa.eu](https://euipo.europa.eu) (EU) → Klasse 42 (Webdesign) und 35 (Werbung).
3. **Domain:** z. B. bei hostpoint.ch: `schwung.ch` ist vermutlich vergeben. Gute Alternativen: `schwung.studio`, `schwungstudio.ch`, `studio-schwung.ch`.
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
| Schwung Blue | `#3D2BFF` | Die eine Signalfarbe: Buttons, Kugel, Akzente. Sparsam! |
| Blue Soft | `#8F84FF` | Akzentwort auf dunklem Grund |
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
> Founder @ schwung · Brands in motion · Design studio, Zürich

**LinkedIn: Info / Unternehmensseite**
> schwung is a design studio in Zürich. We build premium websites, brand looks and launch kits for ambitious small brands. AI helps us move fast; people with taste make it right. From idea to live in about ten days.

**Instagram / TikTok: Bio** (max. 150 Zeichen)
> Brands in motion ⚪︎
> Design studio · Zürich
> Brand + website in 10 days ↓

**Behance: Über mich**
> schwung: a Zürich design studio that puts brands in motion. Web design, brand looks, motion and AI product imagery.

**Name überall gleich:** `schwung` · Handle `@schwung.studio`

## E-Mail-Signatur

```html
<table cellpadding="0" cellspacing="0" style="font-family:Arial,sans-serif;font-size:13px;color:#0d0d0c">
  <tr><td style="padding-bottom:6px"><strong>Your Name</strong> · Founder</td></tr>
  <tr><td style="padding-bottom:10px;color:#6f6a62">schwung · Brands in motion · Zürich</td></tr>
  <tr><td><a href="https://yourdomain.ch" style="color:#3d2bff;text-decoration:none">yourdomain.ch</a></td></tr>
</table>
```

## Website (`schwung/index.html`)

Eine Seite mit: Hero, Arbeiten (SOLUM als Fallstudie), Leistungen, Ablauf in 10 Tagen, Preise, FAQ (inkl. ehrlicher Antwort zu KI), Kontaktformular.

**Noch zu ersetzen, bevor sie live geht:**
- `hello@yourdomain.ch` → deine echte E-Mail
- Social-Links im Footer (`href="#"`) → deine Profile
- Impressum und Datenschutz (in der Schweiz Pflicht) → eigene Seiten
- Das Formular braucht einen Dienst zum Versenden, z. B. **Netlify Forms** (gratis): im `<form>` `name="contact" data-netlify="true"` ergänzen
- Die Preise sind Vorschläge für den Start. Passe sie an, wie du dich wohlfühlst.
- Der Link zur SOLUM-Fallstudie zeigt auf `../solum/index.html`. Auf Netlify den richtigen Link eintragen.
