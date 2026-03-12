# Haweya Abdillahi — Campagnesite

Campagnesite voor Haweya Abdillahi, kandidaat #3 PvdA Amsterdam, gemeenteraadsverkiezingen 18 maart 2026.

- **GitHub**: https://github.com/wouterzaalberg/haweya-abdillahi
- **Kandidaat**: Haweya Abdillahi, #3 op de lijst
- **Partij**: PvdA Amsterdam
- **Verkiezing**: 18 maart 2026

## Huisstijl

### Kleuren
- **PvdA Rood**: `#e12b1a`
- **Rood donker**: `#b82215`
- **Creme**: `#faf5f0`
- **Near-black**: `#0d0d0d`
- **Warm grijs**: `#3a3632`
- **Lichtgrijs**: `#e8e4df`

### Typografie

| Toepassing | Font | Bestand |
|---|---|---|
| Titels / naam | PvdA Compressed | `1. Titel - PVDA-Compressed.otf` |
| Ondertitels / labels | TitlingGothic FB Normal Bold | `2. Ondertitel - TitlingGothicFBNormal-Bold.otf` |
| Broodtekst | TitlingGothic FB Normal Regular | `3. Tekst - TitlingGothicFBNormal-Regular.otf` |
| Serif accenten / quotes | Crimson Pro | Google Fonts |
| Mono labels | Space Mono | Google Fonts |

Fonts worden via `@font-face` geladen (OTF bestanden in root).

### Logo's
- `1. PvdA Amsterdam logo wit.png` - Wit logo met tekst (voor hero)
- `5. PvdA logo roos rood.png` - Rode roos (voor overig gebruik)

## Pagina structuur (index.html)

### 1. Hero
- **Achtergrond**: `hero.jpg` - Haweya in rood pak, stedelijke setting
- **Donkere gradient**: Links-naar-rechts op desktop, onder-naar-boven op mobiel
- **PvdA logo wit**: Linksboven, uitgelijnd met naam
- **"18 Maart 2026"**: Rechtsboven
- **Naam**: "HAWEYA ABDILLAHI #3" in PvdA Compressed, groot (tot 9rem)
  - "#3" in PvdA-rood met punch-animatie
- **Achternaam**: Gewoon wit (geen outline)
- **Tagline**: "Kandidaat Gemeenteraadslid. Lijst 1, plek 3 — PvdA Amsterdam."
- **Grote "3"**: Achtergrond-element (wit, 6% opacity)
- **Animatie**: Tekst schuift van links naar binnen, #3 verschijnt met bounce
- **Content**: Links gepositioneerd met margin-left, max-width 55%
- **Scroll hint**: Rechtsonder met verticale tekst + geanimeerde lijn

### 2. Video
- Witte achtergrond, max-width 1100px
- YouTube embed (youtube-nocookie.com) van "Stem Haweya": `_OpwKY1MGw4`
- Clean embed: geen annotaties, geen gerelateerde video's, neutrale controls
- Scroll-reveal animatie
- Label "Bekijk de video" in rood mono-font

### 3. Intro / Over
- Twee-koloms grid: donkere achtergrond links (bio), creme rechts (stats)
- Stats: Lijst 1 plek 3, Nationale Politie, Voormalige positie Gemeente Amsterdam, 18 Maart 2026
- "03" als groot achtergrondgetal (3% opacity)

### 4. Waarom kandidaat?
- Witte achtergrond, gecentreerde tekst (max 700px)
- Verticale lijn boven de sectie
- Crimson Pro serif, lichter gewicht

### 5. Prioriteiten
- Vier kaarten in 2x2 grid: Smartphonevrij opgroeien & digitalisering, Een stad waar iedereen meedoet, Betaalbaar Amsterdam, Aandacht voor vrouwen
- Hover: kaart wordt zwart met witte tekst, nummer wordt rood
- Verticale lijn boven de sectie

### 6. Quote
- Zwarte achtergrond, groot openingsaanhalingsteken
- Crimson Pro italic quote
- Attributie in rood

### 7. CTA (Stem)
- Rode achtergrond, "STEM" als groot achtergrondwoord
- "Haweya" in outline tekst
- Oproep-tekst: "Op 18 maart kiezen we..." + "Stem Lijst 1, plek 3"
- Witte CTA-button naar PvdA Amsterdam

### 8. Footer
- Zwart, naam + partij + social links (LinkedIn, PvdA)
- Verkiezingsdatum rechts

## Animaties
- **Hero**: slideInLeft (tekst van links), numberPunch (#3 bounce), fadeIn (top bar, scroll hint)
- **Scroll reveal**: `.reveal` class met translateY + opacity, IntersectionObserver (15% threshold)
- **Thema cards**: Gestaggerd reveal (150ms per kaart)
- **Scroll lijn**: Pulserende lijn-animatie
- **Grain overlay**: Subtiel noise-filter over hele pagina (2.5% opacity)

## Responsive
- **> 768px**: Volledige layout
- **< 768px**: Hero full-width, intro 1 kolom, gradient van onder naar boven, scroll hint verborgen

## Bestandsstructuur

```
/
├── CLAUDE.md
├── index.html
├── hero.jpg
├── portret.jpg
├── 1. PvdA Amsterdam logo wit.png
├── 5. PvdA logo roos rood.png
├── 1. Titel - PVDA-Compressed.otf
├── 2. Ondertitel - TitlingGothicFBNormal-Bold.otf
└── 3. Tekst - TitlingGothicFBNormal-Regular.otf
```
