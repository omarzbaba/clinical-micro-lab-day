# Lab Day — A Day in Clinical Microbiology

A **fun, compact, interactive** one-day orientation to the hospital clinical microbiology laboratory, built for medical students on a short rotation. Made for **Alex Kuang** and **Nicholas Barron**.

© 2026 **Omar Z Baba, MD**. All rights reserved. See [LICENSE](LICENSE).

> **Live site:** see the **GitHub Pages** URL in the repository's **About** panel.

---

## What's inside

## How it is organised

Lab Day is a **slide deck**, not a dashboard. One idea per screen, advanced with a
single Next button (or the arrow keys). There are exactly four controls on screen at
any time: Contents, the theme toggle, Back and Next. 141 slides across 15 chapters,
with a Contents overlay to jump between them and shareable per-slide URLs (`#s42`).

`Welcome · Specialties · Biosafety · The journey · The benches · How we test ·
Algorithms · Watch · Through the scope · The report · Flashcards · Which bench? ·
Quiz · Glossary · Recap`

Everything that used to be shown at once — ten chapter tabs, three segmented
controls, two accordions, filter chips and a pip strip — is gone. Each biosafety
level, each bench, each test method, each report stage, each flashcard and each quiz
question now has a screen of its own. The glossary stays a single searchable slide
because that is what a dictionary is for.

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
