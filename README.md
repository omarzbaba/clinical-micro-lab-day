# Lab Day — A Day in Clinical Microbiology

A **fun, compact, interactive** one-day orientation to the hospital clinical microbiology laboratory, built for medical students on a short rotation. Made for **Alex Kuang** and **Nicholas Barron**.

© 2026 **Omar Z Baba, MD**. All rights reserved. See [LICENSE](LICENSE).

> **Live site:** see the **GitHub Pages** URL in the repository's **About** panel.

---

## What's inside

| Section | What it does |
|---|---|
| **The map** | The seven sub-disciplines — bacteriology, virology, mycology, parasitology, mycobacteriology, serology, molecular — each expandable with specimens, methods, organisms, considerations and timing |
| **The journey** | A clickable 7-step walk from specimen receipt through accessioning, adequacy, direct exam, plating, reading/identification, to susceptibility and reporting |
| **The benches** | Urine, respiratory, blood, stool, wound and sterile-fluid benches — media set up, incubation, what the tech looks for, common isolates, and each bench's classic trap |
| **The toolbox** | 14 test methods filterable by family: Gram stain, media, colony morphology, biochemicals, strip assays, disks, rapid antigen, MALDI-TOF, automated ID/AST, blood culture instruments, disk diffusion, broth microdilution, targeted PCR/GeneXpert, multiplex panels/BioFire |
| **Watch it work** | Six looping CSS/SVG animations: the four Gram stain steps, streaking for isolation, overnight colony growth, a blood culture flagging positive, disk-diffusion zones, and a PCR amplification curve |
| **Through the scope** | 10 real freely-licensed stains, plates and bench results, each credited |
| **Flashcards** | 16 flip cards of the organisms worth recognizing by the end of the day |
| **Which bench?** | A scored specimen-routing game |
| **Checkpoint** | 12 quiz questions with instant feedback and a pearl on each |

Light and dark themes, keyboard accessible, `prefers-reduced-motion` respected.

## Run it locally

One self-contained HTML file plus a local `assets/lab/` image folder. No build step, no external requests.

```bash
python3 -m http.server 8123
```

Then visit `http://localhost:8123`. (Opening `index.html` directly also works.)

## Editing the content

All teaching content lives in a single `const DATA = {…}` object near the top of the `<script>` block: `disciplines`, `workflow`, `benches`, `methods`, `flashcards`, `benchGame` and `quiz`. Add or edit an entry and it renders automatically — the hero counters update themselves. Colour tokens for each discipline and bench are CSS custom properties at the top of `<style>`.

## Images and animations

The six animated explainers are original SVG/CSS by the author. The 10 photographs in `assets/lab/` come from **Wikimedia Commons** under public-domain, CC0, CC BY or CC BY-SA licences and are credited beneath each figure with a link to the original. They were individually vetted against their source metadata — several candidates were rejected for showing the wrong subject (a cell-culture chamber labelled as an incubator, an antimicrobial susceptibility panel labelled as a catalase test, a diagnostic algorithm diagram labelled as an agar plate). All motion respects `prefers-reduced-motion`.

## Accuracy

Content was authored and then independently reviewed by a clinical-microbiology reviewer; 31 findings were identified and resolved before release, including several biosafety corrections. Media, panels, instruments, biosafety requirements and turnaround times **vary between laboratories** — this is an orientation aid, not a standard operating procedure.

---

## Copyright

**© 2026 Omar Z Baba, MD. All rights reserved.**

The curriculum, written content, questions, design system and source code of this dashboard — and their selection and arrangement as a compilation — are the original work of the copyright holder and may not be reproduced, redistributed or adapted without written permission.

Full terms are in [LICENSE](LICENSE). This dashboard is an educational orientation aid, not a clinical protocol, and does not constitute medical advice.
