# SAM QIP Hub

The Society for Acute Medicine's quality-improvement hub for acute medicine: the twelve-piece QIP kit, a library of completed projects, where help comes from, and a Learn page with the method in five minutes.

Plain HTML — no build step, no server code, no analytics, no cookies. Everything in this folder is the whole site.

## Draft status

**This is a draft awaiting approval by the Society for Acute Medicine.** Every page says so: an amber "DRAFT" bar sits at the top of the hub, the Learn page, the checker and the 404 page (it stays visible as you scroll), the browser-tab titles start with "DRAFT ·", and the footer stamp reads "Draft — awaiting SAM approval".

To remove it once approved, in each of `index.html`, `learn.html`, `SAM_Abstract_Compliance_Checker.html` and `404.html`:
1. delete the `<div class="draft-banner" …>…</div>` block (just inside the header);
2. delete the CSS block that begins `/* ============ Draft banner …` ;
3. remove `DRAFT · ` from the `<title>` and, where present, the `og:title`;
4. in the footer, change "Draft — awaiting SAM approval · Kit version 1.0" to "Kit version 1.0".
That is the whole job — nothing else references the draft state.


## What's here

| File | What it is |
|---|---|
| `index.html` | The hub — kit, library, support map, get involved, about. This is the front page. |
| `learn.html` | Learn QI — five-minute primer, training ladder, ARCP expectations, FAQ, links. |
| `SAM_Abstract_Compliance_Checker.html` | The QI abstract checker (RES-12). Opens in a new tab from the hub. |
| `404.html` | Shown by GitHub Pages for a missing address; points back to the hub. |
| `SAM_QIP_Hub_og.png`, `SAM_QIP_Learn_og.png` | Link-preview images (1200×630) for Teams, WhatsApp, LinkedIn, X. |
| `SAM_QIP_Kit_Start_Here.docx` | RES-01 |
| `SAM_QIP_Roadmap.pptx` | RES-02 |
| `SAM_QIP_Team_Workbook.xlsx` | RES-03 |
| `SAM_SMART_Aim_Statement_Builder.docx` | RES-05 |
| `SAM_PDSA_Cycle_Worksheet.docx` | RES-06 |
| `SAM_Run_Chart_SPC_Worksheet.xlsx` | RES-07 |
| `SAM_QIP_Audit_Data_Template.xlsx` | RES-08 |
| `SAM_SQUIRE_2_0_Reporting_Guide.pptx` | RES-09 |
| `SAM_SQUIRE_2_0_Presentation_Template.pptx` | RES-10 |
| `SAM_ARCP_Evidence_Checklist.pdf` | RES-11 |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. Keep it. |

RES-04, the QIP Diagram Tool, is not in this bundle — it is its own site at https://aimqa.github.io/SAM-QI-diagram-tool/ (repository `SAM-QI-diagram-tool`).

Every link between the pages and to the files is relative, so the whole folder must stay together and file names must not change. Rename a file and its resource row breaks.

## Publish — the root of the SAMQIP repository

The Diagram Tool now has its own repository and address, **https://aimqa.github.io/SAM-QI-diagram-tool/**, so the hub takes over **https://aimqa.github.io/SAMQIP/**. Every "Open the QIP Diagram Tool" link — on the pages, in the Roadmap deck, the Team Workbook and the Start Here document — already points at the tool's new address.

1. In the `SAMQIP` repository, remove the old Diagram Tool files (they live in `SAM-QI-diagram-tool` now).
2. Upload everything in this bundle to the root of `SAMQIP` — including `.nojekyll`, which some file managers hide.
3. Pages is already on for this repository, so a minute or two after the commit the hub is live at `https://aimqa.github.io/SAMQIP/`, the Learn page at `…/SAMQIP/learn.html`, the checker at `…/SAMQIP/SAM_Abstract_Compliance_Checker.html`.
4. Anyone who saved the tool's old address lands on the hub, one click from the tool.

Link-preview images, canonical URLs and `og:url` are already absolute for `https://aimqa.github.io/SAMQIP/`; nothing needs editing after upload.

## Updating the site

- Edit the HTML directly and re-upload; there is nothing to build.
- To update a kit file, replace it under the same name.
- The library section is the **kit-format shelf of the SAM Improvement Exchange**. To add a completed project, edit that section in `index.html` — copy the worked-example card (`article.entry`), fill it in, and remove the example and the empty-state box once real entries exist. When the shelf passes about ten projects, move it to its own page. Link to it from the Exchange page on the SAM website so the two are one front door.
- The two pages share one stylesheet by copy (`<style>` block in each). If you change the look in one, make the same change in the other.
- Version stamp lives in each page's footer ("Kit version 1.0 · page updated …").

## Contact rule built into the pages

`quality.improvement@acutemedicine.org.uk` is used for three things only: joining the SAM QIP team, submitting a completed project for the library, and reporting a problem with the site (accessibility included). Everything else routes to local and regional teams — the Support section says so. The address is shown in full with a Copy button rather than relying on a mail-app link, because `mailto:` buttons do nothing on machines with no mail app set up.
