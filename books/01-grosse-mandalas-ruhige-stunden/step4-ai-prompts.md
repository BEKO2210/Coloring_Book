# Step 4 — AI Art Prompts (ChatGPT-Image)

**Buch:** Große Mandalas für ruhige Stunden
**Tool:** ChatGPT-Image (GPT-4o Image / Sora-Image)
**Status:** 🟡 Test-Phase — 3 Pilot-Prompts zur Stil-Freigabe

---

## 🎨 ChatGPT-Image Prompt-Strategie

**Was bei ChatGPT-Image anders ist als bei Midjourney/Leonardo:**

| Aspekt | ChatGPT-Image Besonderheit |
|---|---|
| Negative Prompts | ❌ Funktionieren **nicht** als separates Feld — stattdessen `"Do NOT include..."` im Hauptprompt |
| Aspect Ratio | Als Text angeben: `"portrait orientation, 8.5 × 11 inch ratio"` |
| Stil-Anweisungen | Reagiert sehr gut auf **konkrete Stil-Referenzen** wie `"adult coloring book line art"` |
| Sprache | Deutsch + Englisch beide möglich — **Englisch produziert konsistentere Line-Art** |
| Detail-Kontrolle | `"bold outlines only, 2pt line weight, no shading, no gradients"` wirkt zuverlässig |
| Ausgabekanal | Druckbar nur mit `"pure white background, high contrast, black ink only"` |

### Master-Style-Block (wird in ALLE 30 Prompts kopiert)

```
STYLE REQUIREMENTS (mandatory, do not deviate):
- Adult coloring book line art style
- Pure black ink on pure white background — no gray, no color, no shading
- Bold, confident outlines, uniform line weight approximately 2pt
- Large open fields inside the design (minimum 8mm gaps between lines) suitable for seniors
  with limited fine motor control
- Perfectly centered composition, portrait orientation, 8.5 × 11 inch aspect ratio (letter size)
- Clean printable artwork with generous white margin (0.5 inch) on all sides
- High contrast, crisp clean lines — no sketchy strokes, no hatching, no stippling
- Symmetrical mandala structure, mathematically balanced
- Do NOT include: text, letters, numbers, signatures, watermarks, faces, people,
  shading, gradients, color, photorealism, 3D rendering, gray tones
```

---

## 🧪 Pilot-Prompt 1 — EASY (Difficulty 1)

**Zu Seite:** #1 — Sonnen-Mandala
**Ziel:** Sofort-Erfolgserlebnis, großflächig, auch für müde Tage

### Prompt (in ChatGPT-Image einfügen)

```
Create a coloring book page for seniors: a large, simple SUN MANDALA.

DESIGN:
- Central circle containing a smiling stylized sun face made of SIMPLE GEOMETRIC SHAPES
  (NO human face features — just round eyes as circles and a gentle curved smile line)
- 8 large, wide sun rays radiating outward, each ray is a broad triangle or flame shape
- Between the rays: 8 small decorative flower shapes (5-petal daisies)
- Outer circle border with a simple wave pattern
- Everything highly symmetrical (8-fold radial symmetry)
- Mandala fills about 80% of the page, centered

STYLE REQUIREMENTS (mandatory, do not deviate):
- Adult coloring book line art style
- Pure black ink on pure white background — no gray, no color, no shading
- Bold, confident outlines, uniform line weight approximately 2pt
- Large open fields inside the design (minimum 8mm gaps between lines) suitable for seniors
  with limited fine motor control
- Perfectly centered composition, portrait orientation, 8.5 × 11 inch aspect ratio (letter size)
- Clean printable artwork with generous white margin (0.5 inch) on all sides
- High contrast, crisp clean lines — no sketchy strokes, no hatching, no stippling
- Symmetrical mandala structure, mathematically balanced
- Do NOT include: text, letters, numbers, signatures, watermarks, detailed faces, people,
  shading, gradients, color, photorealism, 3D rendering, gray tones
```

### Aspect Ratio / Tweaks
- **In ChatGPT:** nach Ausgabe bei Bedarf sagen: *"Make the lines thicker and the open spaces larger."*
- **Falls zu detailliert:** *"Simplify — remove small decorative elements, keep only the main shapes."*

---

## 🧪 Pilot-Prompt 2 — MEDIUM (Difficulty 2)

**Zu Seite:** #9 — Tulpen-Kranz
**Ziel:** Kernsortiment-Qualität, florale Varianz testen

### Prompt

```
Create a coloring book page for seniors: a TULIP WREATH MANDALA.

DESIGN:
- 6 large stylized tulips arranged in a perfect circle, each tulip pointing OUTWARD,
  stems pointing toward the center
- Tulips are simple cup-shaped flowers with 3 visible petals each, large and easy to color
- Between each tulip pair: a single leaf shape (long, gently curved)
- Central circle: a small rosette made of 6 small dots / round shapes — simple
- Outer border: a thin plain circle frame
- 6-fold radial symmetry, mandala fills 75% of page

STYLE REQUIREMENTS (mandatory, do not deviate):
- Adult coloring book line art style
- Pure black ink on pure white background — no gray, no color, no shading
- Bold, confident outlines, uniform line weight approximately 2pt
- Large open fields inside the design (minimum 8mm gaps between lines) suitable for seniors
  with limited fine motor control
- Perfectly centered composition, portrait orientation, 8.5 × 11 inch aspect ratio (letter size)
- Clean printable artwork with generous white margin (0.5 inch) on all sides
- High contrast, crisp clean lines — no sketchy strokes, no hatching, no stippling
- Symmetrical mandala structure, mathematically balanced
- Do NOT include: text, letters, numbers, signatures, watermarks, faces, people,
  shading, gradients, color, photorealism, 3D rendering, gray tones
```

### Tweaks
- Falls Tulpen zu realistisch: *"Make the tulips more stylized — flat, simple shapes only, like a child's drawing but with clean geometry."*
- Falls zu viele kleine Elemente: *"Remove all small dots and decorative filler — keep only the 6 tulips, 6 leaves, and the central rosette."*

---

## 🧪 Pilot-Prompt 3 — PREMIUM (Difficulty 4)

**Zu Seite:** #29 — Feier-Mandala (Buch-Höhepunkt)
**Ziel:** Premium-Wow-Seite, aber trotzdem senior-tauglich (keine winzigen Details)

### Prompt

```
Create a coloring book page for seniors: a LARGE CELEBRATION MANDALA combining floral and
geometric elements.

DESIGN (from center outward, 5 concentric rings):
Ring 1 (center): an 8-petal rosette, medium-size
Ring 2: 12 small teardrop shapes arranged in a circle
Ring 3: 12 larger stylized flowers (lily-shape, 3 petals each) alternating with 12 simple leaves
Ring 4: a band of 24 soft wave shapes (like gentle scallops)
Ring 5 (outer): 12 large fan-shaped sun-ray petals, wide and open
- 12-fold radial symmetry, perfectly balanced
- Mandala fills 85% of the page
- Every section has LARGE open interior spaces — NO fine hatching, NO tiny dots,
  NO complex filigree

STYLE REQUIREMENTS (mandatory, do not deviate):
- Adult coloring book line art style
- Pure black ink on pure white background — no gray, no color, no shading
- Bold, confident outlines, uniform line weight approximately 2pt
- Large open fields inside the design (minimum 8mm gaps between lines) suitable for seniors
  with limited fine motor control — IMPORTANT: keep fields large even in this complex design
- Perfectly centered composition, portrait orientation, 8.5 × 11 inch aspect ratio (letter size)
- Clean printable artwork with generous white margin (0.5 inch) on all sides
- High contrast, crisp clean lines — no sketchy strokes, no hatching, no stippling
- Symmetrical mandala structure, mathematically balanced
- Do NOT include: text, letters, numbers, signatures, watermarks, faces, people,
  shading, gradients, color, photorealism, 3D rendering, gray tones
```

### Tweaks
- Falls Innenfelder zu klein werden: *"Simplify — reduce to 4 rings only, make all shapes 30% larger."*
- Falls zu symmetrisch-langweilig: *"Add gentle variation in the petal sizes of ring 3 while keeping 12-fold symmetry."*

---

## 🔍 Quality-Check nach Generierung (vor Batch-Freigabe)

Pro Pilot-Bild prüfen:

- [ ] Linienstärke gleichmäßig dick (~2pt), keine dünnen Haarlinien?
- [ ] Alle Innenfelder mindestens 8 mm breit (Fingertest mit Daumen)?
- [ ] Hintergrund rein weiß, keine Grauschatten?
- [ ] Kein Text, keine Zahlen, keine Wasserzeichen?
- [ ] Motiv zentriert, Portrait-Format, Rand frei?
- [ ] Symmetrie sauber (nicht verzerrt / schief)?
- [ ] Kein realistisches Gesicht / keine Person?
- [ ] Druckbar auf 8,5 × 11 inch ohne Zuschnitt wichtiger Elemente?

---

## 🚀 Nach Stil-Freigabe: Batch-Plan

Sobald du die 3 Pilot-Bilder freigibst, erstelle ich:

1. **Prompts #2–8, #10–28** (Evergreen-Kernseiten) — Difficulty 1–3
2. **Prompt #30** (Ausklang-Spirale) — Premium-Partner zu #29
3. **Bonus-Prompts:** How-to-Color-Anleitung, Color-Test-Page, Titel-Seite (für Step 5 vorbereitet)

**Geschätzter Umfang des Final-Dokuments:** ~30 Prompts × ~250 Wörter + Tweaks = ca. 8.000 Wörter.

---

## 📋 Lessons-Learned-Feld (wird nach Freigabe gefüllt)

| Pilot | Generiert? | Qualität | Nötige Anpassung am Master-Style |
|---|---|---|---|
| #1 Sonnen-Mandala (Easy) | ⏳ | — | — |
| #9 Tulpen-Kranz (Medium) | ⏳ | — | — |
| #29 Feier-Mandala (Premium) | ⏳ | — | — |
