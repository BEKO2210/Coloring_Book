# Pipeline State — KDP Coloring Book Workflow

> **Zweck:** Persistenter Status-Tracker aller Bücher in der Produktions-Pipeline.
> **Owner:** Belkis (BEKO2210)
> **Letzte Aktualisierung:** 2026-04-18

---

## 🌍 Globale Projekt-Setup

| Key | Wert |
|---|---|
| `{MARKET}` | amazon.de (DE) |
| `{LANGUAGE}` | DE |
| `{BOOKTYPE}` | Coloring Book |
| `{NICHE}` | Mandalas für Senioren (Beschäftigung, Entspannung, Demenz-geeignet) |
| **AI-Image-Tool (primär)** | **ChatGPT-Image (GPT-4o Image / Sora-Image)** |
| Niche Opportunity-Score | 9,5 / 10 |
| Gewählt in | Step 1 |
| **Ziel-Scope** | **Alle 20 Produktideen aus Step 2 werden veröffentlicht** |

---

## 📚 Buch-Pipeline — Alle 20 Bücher der Nische

### Cluster A — Evergreen (Kernsortiment)

| Slot | Thema (`{THEME}`) | Cluster | Status | Step | Ordner |
|---|---|---|---|---|---|
| **Buch 1** | Große Mandalas für ruhige Stunden | Evergreen | 🟡 In Arbeit | Step 4 | `books/01-grosse-mandalas-ruhige-stunden/` |
| **Buch 2** | Blumen-Mandalas für Senioren (Gartenblumen) | Evergreen | ⏳ Queue | — | `books/02-blumen-mandalas/` |
| **Buch 3** | Tiere fürs Herz — Mandalas mit Haustieren | Evergreen | ⏳ Queue | — | `books/03-tiere-fuers-herz/` |
| **Buch 4** | Schrebergarten & Gartenfreude | Evergreen | ⏳ Queue | — | `books/04-schrebergarten/` |
| **Buch 5** | Handarbeits-Mandalas (Stricken, Nähen, Häkeln) | Evergreen | ⏳ Queue | — | `books/05-handarbeit/` |
| **Buch 6** | Musik erinnert — Mandalas zu Volksliedern | Evergreen | ⏳ Queue | — | `books/06-volkslieder/` |
| **Buch 7** | Alpen, Nordsee, Schwarzwald — Reise-Mandalas | Evergreen | ⏳ Queue | — | `books/07-reise-dach/` |
| **Buch 8** | Küche von damals — Vintage Haushalt | Evergreen | ⏳ Queue | — | `books/08-vintage-kueche/` |
| **Buch 9** | XL-Mandalas — Extra groß, extra einfach | Evergreen | ⏳ Queue | — | `books/09-xl-mandalas/` |
| **Buch 10** | Zahlen-Mandalas — Malen nach Zahlen | Evergreen | ⏳ Queue | — | `books/10-malen-nach-zahlen/` |

### Cluster B — Seasonal

| Slot | Thema (`{THEME}`) | Cluster | Status | Step | Ordner |
|---|---|---|---|---|---|
| **Buch 11** | Advents-Mandalas — 24 Motive | Seasonal (Q4) | ⏳ Queue | — | `books/11-advent/` |
| **Buch 12** | Weihnachten im Herzen — Klassische Mandalas | Seasonal (Q4) | ⏳ Queue | — | `books/12-weihnachten/` |
| **Buch 13** | Frühlingserwachen — Oster- & Maiblumen | Seasonal (Q1/Q2) | ⏳ Queue | — | `books/13-fruehling/` |
| **Buch 14** | Sommer-Mandalas — Sonnenblumen & Kornfelder | Seasonal (Q2/Q3) | ⏳ Queue | — | `books/14-sommer/` |
| **Buch 15** | Goldener Herbst — Erntedank-Mandalas | Seasonal (Q3/Q4) | ⏳ Queue | — | `books/15-herbst/` |

### Cluster C — Trend / Differenzierung

| Slot | Thema (`{THEME}`) | Cluster | Status | Step | Ordner |
|---|---|---|---|---|---|
| **Buch 16** | Unsere Woche — 7 Mandalas für jeden Tag | Trend | ⏳ Queue | — | `books/16-unsere-woche/` |
| **Buch 17** | Gemeinsam malen — Oma & Enkel | Trend | ⏳ Queue | — | `books/17-oma-enkel/` |
| **Buch 18** | Sprichwort-Mandalas — Weisheiten aus der Kindheit | Trend | ⏳ Queue | — | `books/18-sprichwoerter/` |
| **Buch 19** | Mandalas für zittrige Hände | Trend | ⏳ Queue | — | `books/19-zittrige-haende/` |
| **Buch 20** | Beschäftigungs-Band XXL — 100 Mandalas (Premium/B2B) | Trend | ⏳ Queue | — | `books/20-xxl-100/` |

### Empfohlene Launch-Reihenfolge
1. **Buch 1** (Flagship, breitester Appeal) →
2. **Buch 9** (einfachste Produktion, schnelle 2. Royalty) →
3. **Buch 2** (starker Evergreen, floral) →
4. **Buch 11** (Advents-Band, Q4-Push wenn Saison passt) →
5. **Buch 19** (Premium-Preis durch USP) →
6. Rest rollierend alle 2–3 Wochen

→ So entsteht früh Cross-Selling-Masse + ein Q4-Peak ist mitgenommen.

---

## 📖 BUCH 1 — Große Mandalas für ruhige Stunden

### State-Variablen

| Key | Wert | Gesetzt in Step |
|---|---|---|
| `{NICHE}` | Mandalas für Senioren | 1 |
| `{THEME}` | Große Mandalas für ruhige Stunden — 50 klassische, großflächige Mandalas mit dicken Linien; entspannter Einstiegsband | 2 |
| `{AUDIENCE}` | Seniors 70+ (inkl. Menschen mit leichter Demenz); Käufer meist Angehörige 45–70 | 3 (vorläufig gesetzt) |
| `{PAGE_CONCEPT}`-Liste | _(wird in Step 3 gefüllt)_ | 3 |
| `{BOOK_TITLE}` | _(offen)_ | 5 |
| `{PRICE_EUR}` | Ziel-Range 9,99–13,99 € (Premium-Option bis 14,99 €) | 1 / 7 |
| KDP Royalty-Schätzung | ≈ 4,20 € bei 11,99 € VK, 60% Royalty, ~120 S. s/w | 1 |

### Step-Fortschritt Buch 1

- [x] Step 1 — Niche Research (Niche gewählt: Mandalas für Senioren)
- [x] Step 2 — Product Ideas (20 Konzepte generiert; `{THEME}` = Nr. 1 gewählt)
- [x] Step 3 — 30 Page Concepts ✅ (`step3-page-concepts.md`)
- [x] Step 4 — AI Art Prompts (ChatGPT-Image, 30 + 3 Bonus) ✅ (`step4-ai-prompts.md`)
- [ ] User-Produktion — 33 Bilder generieren (8 Sessions geplant) — 🟡 läuft parallel
- [x] Step 5 — Book Structure + Titel ✅ (`step5-book-structure.md`)
  - Titel: **„Große Mandalas für ruhige Stunden"**
  - Subtitle: *Das Mandala-Malbuch für Senioren mit extra großen Motiven — auch für Menschen mit Demenz geeignet*
  - Format: 8,5×11", 68 Seiten, matte paperback
  - Preis: Launch 9,99 € → Regulär 11,99 €
- [x] Step 6 — KDP Listing ✅ (`step6-kdp-listing.md`)
- [ ] Step 7 — Scaling Strategy / 20-Bücher-Launchplan

---

## 📖 BUCH 2 — Blumen-Mandalas für Senioren (geplant)

### State-Variablen (vorläufig)

| Key | Wert |
|---|---|
| `{NICHE}` | Mandalas für Senioren (übernommen von Buch 1) |
| `{THEME}` | Blumen-Mandalas aus vertrauten Gartenblumen (Rose, Sonnenblume, Dahlie, Flieder) |
| `{AUDIENCE}` | Seniors 70+, gartenaffin; Käufer Angehörige |

### Übergabepunkt
**Buch 2 startet, sobald Buch 1 komplett ist** (alle 7 Steps abgeschlossen + KDP-Listing ready).

---

## 🗂️ Ordnerstruktur

```
Coloring_Book/
├── CLAUDE.md                          ← Pipeline-Definition (7 Steps)
├── pipeline-state.md                  ← DIESE DATEI (Status-Tracker)
└── books/
    ├── 01-grosse-mandalas-ruhige-stunden/
    │   ├── step3-page-concepts.md     ← 30 Seitenkonzepte (WIP)
    │   ├── step4-ai-prompts.md        ← AI-Art-Prompts (pending)
    │   ├── step5-book-structure.md    ← Buchaufbau + Titel (pending)
    │   ├── step6-kdp-listing.md       ← Amazon-Listing (pending)
    │   └── step7-scaling.md           ← 10er-Serien-Strategie (pending)
    └── 02-blumen-mandalas/            ← wird bei Start Buch 2 angelegt
```

---

## 🔁 Resume-Anleitung

Zum Wiedereinstieg in einer neuen Session einfach sagen:

```
> resume
```

Claude liest dann diese Datei, zeigt den aktuellen State und schlägt den nächsten Step vor.
