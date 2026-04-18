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
| Niche Opportunity-Score | 9,5 / 10 |
| Gewählt in | Step 1 |

---

## 📚 Buch-Pipeline (Reihenfolge)

| Slot | Thema (`{THEME}`) | Status | Step erreicht | Ordner |
|---|---|---|---|---|
| **Buch 1** | Große Mandalas für ruhige Stunden (50 klassische Mandalas, dicke Linien) | 🟡 In Arbeit | Step 3 | `books/01-grosse-mandalas-ruhige-stunden/` |
| **Buch 2** | Blumen-Mandalas für Senioren (Gartenblumen: Rose, Sonnenblume, Dahlie, Flieder) | ⏳ Geplant | — | `books/02-blumen-mandalas/` |
| **Buch 3** | _(später, nach Buch 2)_ | ⏳ Offen | — | — |

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
- [ ] Step 3 — 30 Page Concepts
- [ ] Step 4 — AI Art Prompts (pro Seite)
- [ ] Step 5 — Book Structure + Titel
- [ ] Step 6 — KDP Listing
- [ ] Step 7 — Scaling Strategy (10er-Serie)

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
