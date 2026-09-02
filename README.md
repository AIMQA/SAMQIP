# SAM QIP Diagram Tool

A single self-contained HTML file for building the diagrams a Quality Improvement Project (QIP) needs, in the style used by the Society for Acute Medicine (SAM). No install, no server, no account required — open the file in a browser and start typing.

## What it's for

Acute medicine QIPs tend to need the same handful of diagrams, in the same order:

1. **Pitch** — the five-sentence pitch (problem, number, aim, why it matters, the ask) for putting a QIP idea in front of a supervisor.
2. **2×2 Ideas** — plot candidate change ideas by impact vs. ease of delivery, to pick what to test first.
3. **Process Map** — what actually happens on the ward today, including decision points and their "otherwise" branches.
4. **5 Whys** — dig from the problem down to a root cause.
5. **Fishbone** — spread out every candidate cause across People / Process / Equipment / Environment / Policies / Patient factors before narrowing in.
6. **Driver Diagram** — aim → primary drivers → secondary drivers → change ideas, ready to test in a PDSA cycle.

Each tab is a separate diagram; a **page** bundles all six together as one project (e.g. one page per QIP, or one per PDSA cycle).

## Using it

- **Load example** fills every tab with a worked VTE-assessment example — a quick way to see how a finished set of diagrams should look.
- **Click any box and type.** Selecting a box shows shape/branch controls in the bar under the hint text.
- **+ New page** starts another project without losing the current one; pages are listed along the top and can be renamed or deleted.
- **Undo / Redo** (or Ctrl+Z / Ctrl+Y) covers every change, including Load example and Clear.
- **Show guidance** (top of the diagram area) toggles inline explanations for what belongs in each part of the diagram — worth leaving on the first few times through.

## Saving, sharing, exporting

- **It saves itself** — everything autosaves to the browser's local storage as you go, so closing the tab is safe.
- **Save file / Open…** downloads or reloads a portable `.json` copy of all your pages — the way to move a project between computers or keep an offline backup.
- **Share link** sends a snapshot to a colleague; **Collaborate** starts a live room so more than one person can edit the same page at once.
- **Sign in with Google** keeps named projects following you across devices — a popup, nothing emailed. See `COLLABORATION_SETUP.md` if it isn't working.
- **Download PNG** exports the current diagram only (not the toolbar or guidance panels) as a landscape image — the format made for dropping straight into slides or a workbook.
- **Print / PDF** produces a one-page landscape PDF of the current diagram.
- **Download PPTX** builds a full PowerPoint deck — one slide per diagram type (Pitch, 2×2, Process Map, 5 Whys, Fishbone, Driver Diagram), for every page in the project, each slide with a SAM-branded header. Useful for a full QIP project handover deck.

## Notes on this version

- Diagram shapes, borders and connector lines render in **black** (not the SAM green) so exports read cleanly in black-and-white print and in slide decks with their own colour scheme. The app's own header/toolbar keep the SAM green branding, since that part never appears in an export.
- A process map decision can branch into an **"otherwise" path** (click a decision box → **+ Add "No" step**). With more than one branching decision on the same map, each branch now routes through its own lane and uses one of six distinct dash styles, so multiple branches stay easy to tell apart.

## Files

- `SAM_QIP_Diagram_Tool.html` — the tool itself. Open it directly in a browser; everything (styles, logic, examples) is in this one file.
