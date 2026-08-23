# Café & Konditorei Schlosser — Website-Demo

Eine vollständig responsive Design- und Konzeptdemo für das **Café & Konditorei
Schlosser** in Speyer (seit 1954). Modernes, spielerisches Webdesign, das die
traditionelle, familiäre Identität des Cafés bewahrt.

> **Hinweis:** Dies ist eine unabhängige Demo-Website zu Präsentationszwecken,
> kein offizieller Web-Auftritt. Es werden keine echten Fotografien der Marke
> verwendet — stattdessen eine eigens gestaltete, illustrative Bildsprache
> (SVG) in den Markenfarben. Für eine finale Umsetzung sollten diese Flächen
> durch professionelle Food-Fotografie des Cafés ersetzt werden.

## Inhalte & Quellen

Alle Fakten (Adresse, Öffnungszeiten, Telefonnummer, Historie, Speisen,
Preise der kleinen Gerichte, Services) stammen aus öffentlich zugänglichen
Informationen zu `cafe-schlosser.de` und wurden **nicht erfunden**:

- Adresse: Maximilianstraße 10, 67346 Speyer (ca. 200 m vom Dom)
- Öffnungszeiten: Dienstag–Sonntag 9–18 Uhr, Montag Ruhetag
- Telefon: 06232 74101
- Gegründet 1954/1955 durch Konditormeister Reinhold und Maria Schlosser,
  heute in dritter Generation familiengeführt
- Frühstück (klein/groß/nach Wunsch), hausgemachte Kuchen & Torten,
  Kaffee- & Teespezialitäten, Mittagstisch mit Suppen/Salaten/Flammkuchen
  (inkl. realer Preise), Eisbecher mit italienischem Eis der Eismanufaktur
  Englert, Schlosser's Bubblewaffel, Winterkreationen (Spekulatius, Wiener
  Mandel, Belgische Schokolade), Services (Reservierung, Gutscheine, WLAN,
  Hunde erlaubt, Kinderstühle)

Wo die Originalseite keine spezifischen Produktnamen oder Preise nennt (z. B.
einzelne Torten), wurden bewusst nur allgemeine, nicht erfundene
Kategoriebeschreibungen verwendet.

## Struktur

```
├── index.html          # gesamte Seite (semantisches HTML5, eine Seite)
├── css/style.css        # Design-System, Layout, Animationen
├── js/main.js           # Mobile Navigation, Sticky Header, Scroll-Reveal
├── assets/favicon.svg   # Favicon im Markenlook
└── README.md
```

Kein Build-Prozess nötig — reines HTML/CSS/JS. Einfach `index.html` im
Browser öffnen oder per statischem Hosting (GitHub Pages, Netlify, Vercel …)
bereitstellen.

## Design-System

Die Farbpalette orientiert sich an der klassischen Bordeaux/Gold/Creme-Optik
traditioneller deutscher Café-Konditoreien, passend zur Markenidentität:

| Rolle | Farbe |
|---|---|
| Primär (Burgund) | `#7A2131` |
| Akzent (Gold) | `#C69749` |
| Hintergrund (Creme) | `#FBF4E8` |
| Text (Espresso) | `#3A2A20` |

Typografie: **Fraunces** (Headlines, warm & editorial) + **Work Sans**
(Fließtext, klar & modern), via Google Fonts.

## Struktur der Seite

1. Hero — „Genuss seit 1954 – mitten in Speyer."
2. Genusswelt — spielerische Kategorie-Navigation
3. Frühstück
4. Kuchen & Torten (visuelles Flaggschiff)
5. Kleine Gerichte / Mittagstisch (mit echten Preisen)
6. Eis & Waffeln (verspielt, Bubblewaffel im Fokus)
7. Kaffee & Tee
8. Tradition seit 1954
9. Service (Reservierung, Gutscheine, WLAN, Hunde, Kinderstühle)
10. Besuch uns (Adresse, Öffnungszeiten, Kontakt, CTA)

## Technisch

- Semantisches HTML5, ARIA-Labels, `skip-link`, Tastaturbedienbarkeit
- Vollständig responsive (Desktop → Mobile), mobile Navigation als Overlay
- Sanfte Scroll-Reveal-Animationen via `IntersectionObserver`
  (mit `prefers-reduced-motion`-Fallback)
- Keine externen Abhängigkeiten außer Google Fonts
