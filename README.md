# OrigoVero Digital Product Passport: Tess van Zalinge scarf

A mobile passport for the Tess van Zalinge Amsterdam Fashion Week Scarf, Cotton Sateen, Patchwork, 68 x 68 cm (SCT-TVZ-COTS-D1-68-001), built from the Figma prototype `Scarf / SCT-TVZ-COTS-D1-68-001` and the same static HTML, CSS and JavaScript as the battery and wine passports. Open `index.html` through any static server.

Content comes only from the product page on origovero.com. The scarf photo is loaded from the client's site.

## What is different from the other passports

| Part | Scarf |
|---|---|
| Key fact | 100% Cotton (main material) |
| Order | Details, Journey, Impact, Story and care (what it is and where it comes from before how to wash it) |
| Journey | Five steps: China (country level), then the Netherlands and three steps in Amsterdam. The Netherlands step is plotted at Amsterdam because the page names no city. The camera never zooms closer than country level on China (`data-zoom`) |
| Details | Size, batch, fabric, print, format, "Item: 1 of 6 in this batch" (the batch page lists six items, this is item 001), ecodesign, link to all batches of the model |
| Impact | Recycled content 0%, cotton 100%, where the fabric and the scarf were made |
| Story | The same module skeleton as the other two products, with a highlight band (wash temperature): one paragraph from the studio, then the care as notes (wash, bleach, dry, iron) plus the note about the studio's own care label |
| Not on this page | No actions block, no tasting or cold chain, no external support or shop links |

## Open questions for the client

- "Nº 1 of 6" is read as the item number inside batch 2026-08 (the batch page lists six items). Is it also a limited edition, i.e. will no more be made?
- Which city or mill the fabric came from in China and where in the Netherlands it was printed.
- Dates for the steps that have none (raw material, quality check); the page says "to be confirmed" only for printing.
- "Print: Patchwork" is read from the product name.
- The care text is shortened into a list; the reasons given in the original (sateen shows shine, sun fades prints) are dropped.
- Coordinates are hand-entered; the map uses OpenStreetMap tiles (not for heavy production traffic) and Leaflet from unpkg.

## Behaviour and checks

Scrollspy tabs, animated accordions, map with one point per step and a camera that follows the product, Replay, full screen step viewer, language sheet. Checked with Playwright at 390 px: no console errors, no horizontal scroll.

## Feedback and reviews

The report form also takes feedback: the reason "Share feedback" goes to the brand privately, in the same place on all three passports. Public reviews are not shown. Questions for the client: are public ratings wanted at all (the EU passport content is an authoritative record from the operator, and reviews are not part of it), how would a review be tied to the item (scanning the item's own QR proves possession), and where would they be aggregated (the "All batches of this model" page looks like the natural place).
