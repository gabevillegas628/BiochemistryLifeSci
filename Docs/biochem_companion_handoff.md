# Biochemistry Course Companion — Project Handoff

## What This Is

A free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Written by the course instructor. Not trying to replace Stryer encyclopedically — trying to replace the *need* to buy Stryer for this specific course.

**The problem it solves:** Students currently pay ~$100+ for a Stryer 10th ed. digital rental that expires at semester end and bundles Achieve access they no longer need. The rental covers far more than the course uses. This resource covers exactly what the course covers, in the voice and framing the course uses, for free.

**The audience:** Pre-med undergraduates in a one-semester biochemistry survey. MCAT downstream. They need mechanistic reasoning, not encyclopedic coverage.

**The pedagogical philosophy:** Clinical reasoning first. Every chapter asks "what breaks and why does it matter" before "here is the pathway." Mechanisms over memorization. The goal is students who can reason through a novel clinical scenario, not students who can reproduce a pathway from memory.

---

## What This Is Not

- A comprehensive two-semester biochemistry reference
- A competitor to Stryer/Lehninger in depth or breadth
- A traditional textbook written for every possible audience
- A document that needs to be complete before it's useful

---

## Authoring Stack

- **Format:** Markdown (.md files)
- **Math/equations:** MathJax inline syntax (dollar sign delimiters) — renders on LibreTexts, GitHub Pages, MkDocs, and most modern static site generators without modification
- **Editor:** VS Code
- **Version control:** Git (start a repo immediately, even if it's just local for now)
- **Publishing target:** TBD — LibreTexts is the likely home (free hosting, textbook-appropriate navigation, MathJax native support, openly licensed). GitHub Pages with MkDocs is an alternative if more control is needed. Decision doesn't need to be made before writing starts — Markdown is portable.

### MathJax Quick Reference

Inline fraction: `$\frac{numerator}{denominator}$`

Display equation (centered, larger):
```
$$\Delta G = \Delta G^{\circ'} + RT\ln\frac{[\text{products}]}{[\text{reactants}]}$$
```

Greek letters: `$\Delta$` `$\alpha$` `$\beta$` `$\mu$` `$K_m$` `$k_{cat}$`

Subscripts/superscripts: `$CO_2$` `$ATP^{4-}$`

---

## Chapter Structure Template

Each chapter follows this rough structure. Not rigid — let the content dictate — but use this as a starting scaffold:

```
# Chapter N: [Topic]

## The Big Picture
Why does this matter clinically? What's the one thing a physician needs to 
understand about this topic? Start here before any mechanism.

## The Mechanism
Explained the way you'd explain it in lecture. Not a list of steps — a 
narrative of why each step happens. If a student understands the logic, 
they can reconstruct the pathway. If they memorize the pathway, they 
understand nothing.

## When It Breaks
The diseases, deficiencies, poisons, and clinical presentations that emerge 
from pathway dysfunction. This is where the clinical cases live. Each one 
should illuminate the mechanism, not just illustrate that the topic is 
"relevant to medicine."

## The MCAT Angle
What does this actually look like when tested? Not a list of facts — a 
description of the reasoning pattern the MCAT tests repeatedly on this topic.

## Worked Problems
2-3 problems that require mechanistic reasoning, not recall. Show the 
reasoning process, not just the answer.

## Opener Questions
The clinical reasoning questions used at the start of class sessions. 
(These double as study questions for students reading independently.)
```

---

## Chapter List (Maps to Course Syllabus)

Ordered by syllabus sequence, not traditional textbook order. Write in this order — students need Ch 1 in week 1, not Ch 15.

| # | Topic | Stryer Ch | Status |
|---|-------|-----------|--------|
| 1 | Thermodynamic Principles & Why We Exist | 1 | **START HERE** |
| 2 | Protein Composition & Structure | 2 | Not started |
| 3 | Molecular Binding & Hemoglobin | 3 | Not started |
| 4 | Enzyme Kinetics | 5 | Not started |
| 5 | Carbohydrates | 11 | Not started |
| 6 | Lipids & Biological Membranes | 12 | Not started |
| 7 | Membrane Channels & Pumps | 13 | Not started |
| 8 | Signal Transduction | 14 | Not started |
| 9 | Thermodynamic Principles II | 15 | Not started |
| 10 | Glycolysis | 16 | Not started |
| 11 | The Krebs Cycle | 17 | Not started |
| 12 | Electron Transport Chain & Oxidative Phosphorylation | 18 | Not started |
| 13 | Pentose Phosphate Pathway | 20 | Not started |
| 14 | Glycogen Metabolism | 21 | Not started |
| 15 | β-Oxidation | 22 | Not started |
| 16 | Protein Metabolism | 23 | Not started |
| 17 | Nucleotide & Amino Acid Biosynthesis | 25/26 | Not started |
| 18 | DNA & RNA Synthesis | 28/29 | Not started |
| 19 | RNA & Protein Synthesis | 29/30 | Not started |

---

## Chapter 1 — Starting Point

**Topic:** Thermodynamic Principles & Why We Exist

**The core framing (write from this):**

The standard "entropy means disorder" explanation immediately creates a paradox — cells are extraordinarily ordered, so how do they exist without violating the second law? Most textbooks handwave about open systems and energy input without actually satisfying the question.

The better framing: organisms are local entropy-decreasing machines that only get away with it by accelerating entropy increase elsewhere — in the sun, in the heat they dissipate, in the CO2 they exhale. The universe's entropy budget still increases; we take a temporary loan against it to maintain our ordered state. The loan must be repaid constantly, which is why we have to eat.

This reframes metabolism before a single pathway is introduced. Every catabolic reaction, every ATP hydrolysis, every electron tumbling down the ETC is loan repayment. The organism is the thermodynamic loophole. The pathways are the mechanism of the loophole.

**Key concepts to cover:**
- Entropy as universal tendency, not local tendency — the distinction that makes life possible
- Enthalpy, entropy, Gibbs free energy — ΔG as the actual decision-maker for whether reactions proceed
- Standard free energy (ΔG°') vs actual free energy (ΔG) — why the cell's ATP/ADP ratio matters enormously
- Coupled reactions — how cells use favorable reactions to drive unfavorable ones
- Why ATP is the energy currency (not because it has "high energy bonds" — that framing is wrong and misleading)

**Clinical hook:**
Dinitrophenol (DNP) — a weight loss drug used in the 1930s that uncouples the proton gradient from ATP synthesis. Patients lost weight rapidly because they were burning fuel without capturing the energy as ATP, dissipating it as heat instead. Some died of hyperthermia. Still used illegally today. Explains thermodynamic uncoupling before the ETC chapter introduces the proton gradient formally — plant the seed here.

**Opener questions drafted:**
1. "A reaction has a negative ΔG but proceeds extremely slowly at room temperature. What's missing and why doesn't thermodynamic favorability guarantee it happens?"
2. "Cells maintain the ATP/ADP ratio far above equilibrium. Why does this matter for the actual ΔG of ATP hydrolysis inside a cell compared to the standard ΔG°'?"

---

## File Structure

```
biochem-companion/
├── README.md              ← project overview, licensing, how to contribute
├── 01-thermodynamics.md   ← START HERE
├── 02-protein-structure.md
├── 03-hemoglobin.md
├── ...
├── figures/               ← placeholder for figures when they exist
└── assets/                ← anything else
```

---

## Licensing

Publish under Creative Commons CC BY-NC-SA 4.0 — same license as LibreTexts content. Free to use, adapt, and share with attribution, non-commercially, under the same license. This is the right license for an OER that you want students and other educators to use freely without opening commercial exploitation.

---

## Notes on Voice

This is not a textbook written for every possible biochemistry course. It is written for one course, one audience, one pedagogical philosophy. That specificity is the point.

Write the way you explain things in lecture and in conversation — not the way Stryer explains things. If a sentence sounds like it belongs in a reference manual, rewrite it. If a paragraph doesn't answer "why does this matter" somewhere, it's missing something.

The clinical cases are not appendices or "real world connections" boxed off at the end of chapters. They are the spine of the explanation. The mechanism exists to explain the disease. The disease exists to make the mechanism matter.

---

## Context

This project emerged from a longer conversation about:
- AI detection in student essays (apostrophe forensics, docx metadata analysis)
- Course redesign toward clinical reasoning and MCAT alignment
- The Pulse classroom response platform (separate project — see `classroom_response_tool_handoff.md`)
- The observation that students pay ~$100 for a digital rental they use 40% of

The textbook is the last piece of a coherent system: Pulse handles real-time engagement, the exam redesign handles assessment, and this handles the content layer. All three serve the same goal — students who reason like clinicians, not students who memorized Anki decks.

The instructor describes his career as "a series of accidentally fortunate stumbles." This project is no exception.
