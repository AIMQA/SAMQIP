# SAM QIP Hub

The Society for Acute Medicine's quality-improvement hub for acute medicine: the twelve-piece QIP kit, a library of completed projects, where help comes from, and a Learn page with the method in five minutes.

Plain HTML — no build step, no server code, no analytics, no cookies. Everything in this folder is the whole site.

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

RES-04, the QIP Diagram Tool, is not in this bundle — it is the site already at https://aimqa.github.io/SAMQIP/, which stays where it is.

Every link between the pages and to the files is relative, so the whole folder must stay together and file names must not change. Rename a file and its resource row breaks.

## Publish — a `hub` folder inside the existing SAMQIP repository

The Diagram Tool stays exactly where it is, at **https://aimqa.github.io/SAMQIP/**. The hub goes into a folder beside it, so it lives at **https://aimqa.github.io/SAMQIP/hub/** — same repository, nothing moved, no link anywhere goes dead.

1. In the `SAMQIP` repository, create a folder called `hub`.
2. Upload everything in this bundle into that folder — including `.nojekyll`, which some file managers hide.
3. Pages is already on for this repository, so a minute or two after the commit the hub is live at `https://aimqa.github.io/SAMQIP/hub/`. The Learn page is `…/SAMQIP/hub/learn.html` and the checker `…/SAMQIP/hub/SAM_Abstract_Compliance_Checker.html`. Every "Open the QIP Diagram Tool" link points at `https://aimqa.github.io/SAMQIP/`.
4. Optional: add a link to the hub from the Diagram Tool's own page, so people arriving at the tool can find the kit.

Link-preview images, canonical URLs and `og:url` are already absolute for the `/hub/` address. If you would rather give the hub its own repository (for a shorter address), the only change is those six lines in `index.html` and `learn.html`.

## Updating the site

- Edit the HTML directly and re-upload; there is nothing to build.
- To update a kit file, replace it under the same name.
- The library section is the **kit-format shelf of the SAM Improvement Exchange**. To add a completed project, edit that section in `index.html` — copy the worked-example card (`article.entry`), fill it in, and remove the example and the empty-state box once real entries exist. When the shelf passes about ten projects, move it to its own page. Link to it from the Exchange page on the SAM website so the two are one front door.
- The two pages share one stylesheet by copy (`<style>` block in each). If you change the look in one, make the same change in the other.
- Version stamp lives in each page's footer ("Kit version 1.0 · page updated …").

## Contact rule built into the pages

`quality.improvement@acutemedicine.org.uk` is used for three things only: joining the SAM QIP team, submitting a completed project for the library, and reporting a problem with the site (accessibility included). Everything else routes to local and regional teams — the Support section says so. The address is shown in full with a Copy button rather than relying on a mail-app link, because `mailto:` buttons do nothing on machines with no mail app set up.
