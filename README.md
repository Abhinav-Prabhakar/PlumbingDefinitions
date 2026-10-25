<div align="center">
  <img src="assets/og.png" alt="one·liners — Plumbing, in one line." width="100%" />
</div>

<div align="center">

# one·liners · Plumbing

**Plumbing, in one line.**

A quiet code book you can practise: 206 definitions across 5 subjects — water supply, drain-waste-vent, traps and vents, backflow and fixtures, and the plumbing code — with an adaptive two-way quiz and a memory of what you actually know.

<a href="https://abhinav-prabhakar.github.io/PlumbingDefinitions/">
  <img src="https://img.shields.io/badge/OPEN%20THE%20APP-live-b5653a?style=for-the-badge&logo=githubpages&logoColor=white" alt="Open the live app" />
</a>

<br /><br />

<img src="https://img.shields.io/badge/definitions-206-b5653a?style=flat-square" alt="206 definitions" />
<img src="https://img.shields.io/badge/subjects-5-0e0f11?style=flat-square" alt="5 subjects" />
<img src="https://img.shields.io/badge/PWA-offline--ready-0e0f11?style=flat-square&logo=pwa&logoColor=white" alt="PWA offline ready" />
<img src="https://img.shields.io/badge/backend-none-2a78b8?style=flat-square" alt="No backend" />
<img src="https://img.shields.io/badge/vanilla-HTML%20%C2%B7%20CSS%20%C2%B7%20JS-66727f?style=flat-square" alt="Vanilla HTML CSS JS" />
<img src="https://img.shields.io/badge/deploy-GitHub%20Pages-0e0f11?style=flat-square&logo=github&logoColor=white" alt="GitHub Pages" />

</div>

<p align="center"><sub>Screenshots use sample study data. The app itself starts clean, on your device.</sub></p>

---

## Why this exists

Plumbing exams are full of near-twins: *riser* and *branch*, *trap seal* and *trap arm*, *backflow* and *back-siphonage*. **one·liners** gives each term one line, quizzes it both ways, and puts the twins side by side until they stop blurring.

Warm paper, copper and water-blue, a sturdy grotesk, and a pipe run with a P-trap holding its seal while water flows through. No accounts, no server, no noise.

> **Recognition is not recall.** Recognising *tailpiece* on a diagram is not the same as naming it from its description. So the quiz asks both ways.

---

## Screenshots

<table>
  <tr>
    <td width="50%">
      <img src="assets/screenshot-home-light.png" alt="Home in light mode" width="100%" />
      <p align="center"><sub><strong>Light by default</strong> · today, activity, subject mastery</sub></p>
    </td>
    <td width="50%">
      <img src="assets/screenshot-home-dark.png" alt="Home in dark mode" width="100%" />
      <p align="center"><sub><strong>Dark when you choose it</strong> · remembered across visits</sub></p>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td width="58%">
      <img src="assets/screenshot-subject-light.png" alt="A subject's definitions with per-definition mastery" width="100%" />
      <p align="center"><sub><strong>Every definition has a memory.</strong> Hover a row for its mastery and source.</sub></p>
    </td>
    <td width="42%">
      <img src="assets/screenshot-quiz-dark.png" alt="A two-way quiz in dark mode" width="100%" />
      <p align="center"><sub><strong>Answers explain themselves.</strong> The definition, and what you picked.</sub></p>
    </td>
  </tr>
</table>

<div align="center">
  <img src="assets/screenshot-mobile-subject.png" alt="one·liners on a phone" width="310" />
  <p><sub><strong>320 → 1440px.</strong> The same quiet interface, not a crushed desktop.</sub></p>
</div>

---

## What's inside

**206 one-liners** across **5 subjects**, written for plumbing apprentices and journeyman exam candidates.

- **Core** — Water Supply Systems, Drain-Waste-Vent, Traps and Vents, Backflow and Fixtures, Plumbing Code

| Subject | Definitions | Units |
| --- | ---: | --- |
| **Water Supply Systems** | 42 | Supply basics · Pressure and flow · Pipe materials · Fittings and valves · Water heating |
| **Drain-Waste-Vent** | 42 | Drainage basics · Drain pipe sizing · Waste fittings · Vent systems · Slope and grade |
| **Traps and Vents** | 40 | Trap fundamentals · Trap seals · Venting methods · Vent sizing · Common venting defects |
| **Backflow and Fixtures** | 42 | Cross-connection basics · Backflow devices · Fixture types · Fixture requirements · Water efficiency |
| **Plumbing Code** | 40 | Code framework · Permits and inspection · Materials and joints · Support and protection · Safety and testing |

Every definition is one sentence, 8–28 words, and carries a source locator. Hover a
definition's mastery rail to see where it came from. Coverage, gaps and assumptions are
documented in [`data/README.md`](data/README.md).

---

## Two directions of recall

Every round mixes both question types, balanced 5/5. You cannot coast on recognition.

| Prompt | You choose | What it trains |
| --- | --- | --- |
| `Trap seal` | one of four definitions | term → meaning |
| “The short pipe that carries waste from a fixture outlet down to the trap inlet.” | one of four terms | meaning → term |

- **The term is never in the question.** When a definition has to mention its own term, the
  quiz blanks it out, so meaning → term tests meaning.
- **Wrong answers that look right.** Distractors come from each definition's curated
  look-alikes, then from similar wording in the same unit — never four random strangers.
- **Adaptive sampling.** The three weakest definitions are guaranteed a slot; the rest are
  weighted toward low mastery.
- **Keyboard complete.** <kbd>1</kbd>–<kbd>4</kbd> or <kbd>A</kbd>–<kbd>D</kbd> to choose,
  <kbd>Enter</kbd> for next, <kbd>Esc</kbd> to leave, <kbd>r</kbd> to repeat a round.

---

## A memory you can see

Mastery is one confidence score per definition, stored locally: **+30%** for a correct answer,
**−40%** for a miss. Four clean answers reach 100%.

| After | Score | Reads as |
| --- | --- | --- |
| no attempts | 0% | `new` |
| 1 correct | 30% | `learning` |
| 2 correct | 60% | `familiar` |
| 3 correct | 90% | `solid` |
| a miss | −40% | re-learn |

The subject page shows a 2px bar on every definition; cards show a bar profile of the whole
subject; the home page has a daily goal stack and a quiet, monochrome activity trail.

---

## Offline, installable, private

- **Full PWA** — manifest, service worker, maskable icons. Works offline after the first load.
  Install from the browser's own menu (Chrome: the install icon in the address bar; iOS Safari:
  **Share → Add to Home Screen**; macOS Safari: **File → Add to Dock**).
- **No accounts, no analytics, no server.** Progress lives in `localStorage` under
  `oneliners.plumbing-licensing.*` and never leaves the device.
- **Self-hosted type** — Archivo, Inter. No external font requests.
- **Light by default**, dark when you choose it, remembered before first paint.

---

## Sources

| Source | Publisher | License |
| --- | --- | --- |
| [ASSE International Plumbing Dictionary, 6th Edition](https://asse-plumbing.org/) | ASSE International | free public PDF; copyright ASSE International |
| [40 CFR 141.2 - National Primary Drinking Water Regulations definitions](https://www.ecfr.gov/current/title-40/chapter-I/subchapter-D/part-141/subpart-A/section-141.2) | US Environmental Protection Agency (eCFR) | US Government work (public domain) |
| [International Plumbing Code 2021 (Chapters 1-10)](https://up.codes/viewer/texas/ipc-2021) | International Code Council (ICC) | proprietary model code; free read-only access, no redistribution |
| [29 CFR 1910.146 - Permit-Required Confined Spaces](https://www.osha.gov/laws-regs/regulations/standardnumber/1910/1910.146) | US Occupational Safety and Health Administration | US Government work (public domain) |
| [29 CFR 1926 Subpart P - Excavations](https://www.osha.gov/laws-regs/regulations/standardnumber/1926/1926SubpartP) | US Occupational Safety and Health Administration | US Government work (public domain) |
| [Cross-Connection Control Manual (EPA 816-R-03-002)](https://www.epa.gov/sites/default/files/2015-09/documents/epa816r03002_0.pdf) | US Environmental Protection Agency, Office of Water | US Government work (public domain) |
| [WaterSense product criteria (toilets, faucets, showerheads, urinals)](https://www.epa.gov/watersense/watersense-products) | US Environmental Protection Agency, WaterSense | US Government work (public domain) |
| [Uniform Plumbing Code 2024 (IAPMO/ANSI UPC 1-2024)](https://epubs.iapmo.org/2024/UPC/) | International Association of Plumbing and Mechanical Officials (IAPMO) | proprietary model code; free read-only edition |

Definitions are paraphrased one-liners, not excerpts. Raw source material is not redistributed.

> [!IMPORTANT]
> Educational vocabulary only; not plumbing advice or code compliance guidance.

---

## Run it locally

```bash
# A server is required: the app fetches its data.
python3 -m http.server 8000
# → http://localhost:8000/
```

No build step, no dependencies. `index.html` is the whole app.

```text
.
├── index.html             # the entire app
├── manifest.webmanifest   # PWA manifest
├── sw.js                  # offline app shell + data cache
├── data/
│   ├── curriculum.json    # sections and subjects the app loads
│   ├── sources.json       # where every definition comes from
│   ├── collection.json    # scope, audience, assumptions
│   ├── README.md          # coverage report
│   └── subjects/*.json    # one file per subject
└── assets/                # icons, social card, screenshots, fonts
```

---

## The one·liners family

Same instrument, different vocabularies. Each has its own look, data and progress.

| Collection | Repository |
| --- | --- |
| [Electronics, in one line.](https://abhinav-prabhakar.github.io/ECEDefinitions/) | [`Abhinav-Prabhakar/ECEDefinitions`](https://github.com/Abhinav-Prabhakar/ECEDefinitions) |
| [Anatomy and physiology, in one line.](https://abhinav-prabhakar.github.io/AnatomyDefinitions/) | [`Abhinav-Prabhakar/AnatomyDefinitions`](https://github.com/Abhinav-Prabhakar/AnatomyDefinitions) |
| [Electricity, in one line.](https://abhinav-prabhakar.github.io/ElectricalCodeDefinitions/) | [`Abhinav-Prabhakar/ElectricalCodeDefinitions`](https://github.com/Abhinav-Prabhakar/ElectricalCodeDefinitions) |
| [HVAC, in one line.](https://abhinav-prabhakar.github.io/HVACDefinitions/) | [`Abhinav-Prabhakar/HVACDefinitions`](https://github.com/Abhinav-Prabhakar/HVACDefinitions) |
| [Medicine, in one line.](https://abhinav-prabhakar.github.io/MedicalTerminologyDefinitions/) | [`Abhinav-Prabhakar/MedicalTerminologyDefinitions`](https://github.com/Abhinav-Prabhakar/MedicalTerminologyDefinitions) |
| [Nursing, in one line.](https://abhinav-prabhakar.github.io/NursingDefinitions/) | [`Abhinav-Prabhakar/NursingDefinitions`](https://github.com/Abhinav-Prabhakar/NursingDefinitions) |
| [Pharmacology, in one line.](https://abhinav-prabhakar.github.io/PharmacologyDefinitions/) | [`Abhinav-Prabhakar/PharmacologyDefinitions`](https://github.com/Abhinav-Prabhakar/PharmacologyDefinitions) |
| **[Plumbing, in one line.](https://abhinav-prabhakar.github.io/PlumbingDefinitions/)** | [`Abhinav-Prabhakar/PlumbingDefinitions`](https://github.com/Abhinav-Prabhakar/PlumbingDefinitions) |
| [Software, in one line.](https://abhinav-prabhakar.github.io/SoftwareInterviewDefinitions/) | [`Abhinav-Prabhakar/SoftwareInterviewDefinitions`](https://github.com/Abhinav-Prabhakar/SoftwareInterviewDefinitions) |
| [The law, in one line.](https://abhinav-prabhakar.github.io/LegalDefinitions/) | [`Abhinav-Prabhakar/LegalDefinitions`](https://github.com/Abhinav-Prabhakar/LegalDefinitions) |

### Credits

Definitions are paraphrased from the public references listed above; code sections are cited, not reproduced. Built on the [one·liners](https://github.com/Abhinav-Prabhakar/ECEDefinitions) engine. Fonts: Archivo, Inter (SIL Open Font License 1.1).

<div align="center">
  <sub>If this helps you pass your plumbing exam, star the repo. Keep the seal, vent the stack.</sub>
</div>
