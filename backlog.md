# Backlog

Items to revisit. Add context so future-you remembers why it was deferred.

---

## Oxidation and Reduction

**Where it belongs:** Unclear. A brief definitional section (loss/gain of electrons, OIL RIG, one biological example like NAD+/NADH) could go in Chapter 1 alongside acid-base chemistry as part of the chemical toolkit. Disulfide bond context in Chapter 2 needs at minimum a one-line definition. Full quantitative treatment (reduction potentials, ΔG of electron transfer) belongs with metabolism, before the ETC chapter.

**Decision needed:** Add a short redox section to Chapter 1, or handle it inline in Chapter 2 with a forward reference to metabolism?

---

## Peptide Bond: Formation and Resonance Diagrams

**Where it belongs:** Chapter 2, peptide bond section (currently after the amino acids section).

**What's needed:** Two visual/diagrammatic additions:
1. Peptide bond formation: the condensation reaction showing two amino acids combining with loss of water. Currently described in prose only.
2. Resonance structures of the peptide bond: showing electron delocalization from the nitrogen lone pair into the carbonyl, explaining the partial double-bond character and planarity. Critical for students to understand WHY rotation is restricted.

**Challenge:** MathJax can render reaction arrows and simple structural formulas but full bond-line structural drawings are difficult without a figure. Options: (a) use a MathJax array to approximate structural layout, (b) defer until a figures directory exists, (c) find a clean ASCII/Unicode approximation. Decide when tackling Chapter 2 revision.

---

## Ch. 3: Binding Site Geometry, Specificity, and $K_d$

**Where it belongs:** Chapter 3, The Chemistry of Binding section, after the $K_d$ derivation and before or within the Oxygen as a Binding Problem section.

**What's needed:** An explicit treatment of how the physical geometry and chemical complementarity of the binding site determine both specificity (which ligands bind at all) and $K_d$ (how tightly they bind). Currently the chapter goes straight from the math of $K_d$ to oxygen delivery without connecting the number back to the molecular architecture that produces it. Key points to cover: shape complementarity restricts which ligands can access the site; the number, type, and geometry of non-covalent contacts (H-bonds, van der Waals, hydrophobic, electrostatic) set the enthalpy of binding; the burial of hydrophobic surface drives the entropic component; together these determine $\Delta G_{binding}$ and thus $K_d = e^{\Delta G / RT}$. Could use heme pocket geometry as the worked example since it is already in the chapter: the distal histidine geometry is what discriminates O$_2$ from CO, making it a perfect illustration of how a few angstroms of geometry difference produces a meaningful $K_d$ difference.

**Challenge:** Needs to stay concise so it does not break the flow into the Myoglobin section. May work best as a bridge subsection between $K_d$ math and the oxygen biology.

---

## "The MCAT Angle" Section: Keep or Cut?

**Affects:** All chapters (Ch. 1 through Ch. 5 drafted so far).

**The tension:** The section exists because MCAT alignment is effectively the point of the course, but explicitly labeling it as "The MCAT Angle" feels like teaching to the test, which conflicts with the book's pedagogical philosophy. Renaming options ("How to Think About This", "Reasoning Through Novel Problems") either sound patronizing or still feel like test-prep rebranding.

**Decision needed:** Either cut the section entirely and trust that the worked problems and clinical cases cover the reasoning patterns, or find a framing that is honest about the purpose without being reductive. Revisit all drafted chapters when a decision is made.

---

## Phi/Psi Angles and Ramachandran Plot

**Where it belongs:** Chapter 2, peptide bond section, immediately after the discussion of phi ($\phi$) and psi ($\psi$) angles and their role in restricting backbone geometry.

**What's needed:**
1. A diagram showing a backbone segment with the phi and psi angles labeled at the alpha-carbon, making clear which bond each angle describes.
2. A Ramachandran plot showing the allowed (alpha-helix, beta-sheet) and disallowed regions of phi/psi space. Ideally shaded to show favored vs. allowed vs. disallowed regions, with the helix and sheet regions labeled.

**Why it matters:** The Ramachandran plot is the single best visual proof that secondary structures are not arbitrary. Students who see it understand immediately why only a few backbone geometries exist in real proteins. Hard to convey in prose alone.

**Challenge:** Both require real figures. MathJax cannot approximate a 2D scatter/contour plot. This is a strong candidate for the figures directory once one is established.
