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

RES-04, the QIP Diagram Tool, is a separate site (https://aimqa.github.io/SAMQIP/) and is linked, not copied.

Every link between the pages and to the files is relative, so the whole folder must stay together and file names must not change. Rename a file and its resource row breaks.

## Publish on GitHub Pages

1. Create a repository (public, or private on a plan that allows Pages), e.g. `SAMQIPHub`.
2. Upload everything in this folder to the root of the repository — including `.nojekyll`, which some file managers hide.
3. In the repository: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. After a minute or two the site is live at `https://<account>.github.io/<repository>/`.
   The hub is that address; the Learn page is `…/learn.html`; the checker is `…/SAM_Abstract_Compliance_Checker.html`.

### One edit once you know the address

Link previews need an absolute image URL. In `index.html` and `learn.html` change the two `og:image` and two `twitter:image` values from `./SAM_QIP_Hub_og.png` / `./SAM_QIP_Learn_og.png` to the full address, e.g. `https://<account>.github.io/<repository>/SAM_QIP_Hub_og.png`. Nothing else depends on the address.

## Updating the site

- Edit the HTML directly and re-upload; there is nothing to build.
- To update a kit file, replace it under the same name.
- To add a completed project to the library, edit the "Completed projects from SAM members" section in `index.html` — the empty-state box comes out and a project card goes in. When the library passes about ten projects, move it to its own page.
- The two pages share one stylesheet by copy (`<style>` block in each). If you change the look in one, make the same change in the other.
- Version stamp lives in each page's footer ("Kit version 1.0 · page updated …").

## Contact rule built into the pages

`quality.improvement@acutemedicine.org.uk` is used for three things only: joining the SAM QIP team, submitting a completed project for the library, and reporting a problem with the site (accessibility included). Everything else routes to local and regional teams — the Support section says so.
