# Backlog

Items to revisit. Add context so future-you remembers why it was deferred.

---

## PFK-1 Allosteric Site Structural Details

**Where it belongs:** Chapter 10, Step 3 regulatory bullet points.

**What needs verification:** (1) Does citrate bind its own allosteric site or does it work through/near the AMP/ATP regulatory site? (2) Does F-2,6-BP bind a site distinct from both the substrate (F-6-P) site and the AMP/ATP regulatory site? Current text says each effector acts through allosteric sites without specifying overlap — confirm against a structural reference (e.g., Schirmer & Evans 1990 or a mammalian PFK-1 crystal structure paper) before publication.

**Why deferred:** Structural details complex and species-dependent; beyond pre-med survey scope but should be accurate.

---

## Glucose Origin and Entry into the Cell

**Where it belongs:** Chapter 10 (Glycolysis), likely at the start of Part I or as a short section before the investment phase begins. Could alternatively go in Chapter 5 (Carbohydrates) if that chapter covers digestion.

**What's needed:** The chapter currently opens with glucose already present in the cell, with no account of how it got there. Students will reasonably ask. At minimum, cover: dietary carbohydrates are digested to monosaccharides in the gut; glucose is absorbed in the small intestine and enters the portal circulation; cells take up glucose via facilitated diffusion through **GLUT transporters** (not active transport in most tissues); different tissues express different GLUT isoforms with different $K_m$ values and regulatory properties (GLUT1 ubiquitous/low $K_m$; GLUT2 liver and β cells/high $K_m$, matches glucokinase; GLUT4 muscle and adipose/insulin-regulated). The GLUT4 story connects directly to insulin signaling from Chapter 8 and is heavily MCAT-tested.

**Why it was deferred:** Chapter 10 was written to focus on the pathway itself; the entry logistics were recognized after the fact as a gap.

---

## Oxidation and Reduction

**RESOLVED (Chapter 9, 2026-05-26):** Full quantitative treatment (reduction potentials, ΔG = −nFΔE°', NADH/FADH₂/NADPH as carriers) placed in Chapter 9 (Thermodynamic Principles II). Chapter 2 still has only a one-line inline definition of redox for disulfide bonds; that is intentional. Forward references in earlier chapters point to Chapter 9.

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

---

## G6PD Deficiency as the Clinical Anchor for NADPH

**Where it belongs:** The pentose phosphate pathway chapter (chapter number TBD), in or immediately after the section explaining what NADPH is used for.

**Why it's great:** G6PD deficiency is the most common human enzyme defect (~400 million people affected), is heavily MCAT-tested, and the mechanism is a perfect illustration of the NADPH story. Without G6PD, the pentose phosphate pathway can't run, NADPH can't be generated, reduced glutathione can't be regenerated, red blood cells can't neutralize oxidative stress, and they lyse. Clinically this presents as hemolytic anemia triggered by oxidative stressors: fava beans, primaquine, dapsone, certain infections. The connection from "NADPH manages oxidative stress" (introduced in Ch. 9) to "here's what happens when that system fails" is exactly the kind of payoff that makes the earlier mechanistic groundwork feel worthwhile.

**Note:** Ch. 9 already introduces NADPH and mentions glutathione reductase as an NADPH-dependent enzyme. G6PD deficiency should be the clinical anchor that cashes that forward reference in.

---

## Alcohol Metabolism, NADH Accumulation, and the NAD+/NADH Ratio

**Where it belongs:** The glycolysis/gluconeogenesis chapter (Chapter 10), in the section on gluconeogenesis or the regulation of glycolysis.

**Why it's great:** Alcohol is oxidized to acetaldehyde by alcohol dehydrogenase and then to acetate by aldehyde dehydrogenase — both reactions reduce NAD+ to NADH. Heavy alcohol consumption floods the liver with NADH, driving the NAD+/NADH ratio way down. The consequences are a direct illustration of the pathway thermodynamics in Ch. 9: low NAD+ stalls gluconeogenesis (which needs NAD+ at the glyceraldehyde-3-phosphate dehydrogenase step), causing hypoglycemia; excess NADH pushes pyruvate toward lactate rather than gluconeogenesis, causing lactic acidosis; and the same NADH shift pushes oxaloacetate toward malate, starving the TCA cycle of its entry substrate. Fasting hypoglycemia in a binge drinker is essentially a real-world demonstration of what happens when you collapse the NAD+/NADH ratio.

**Note:** Ch. 9 already makes the point that NAD+/NADH ratio governs pathway flux. This case study is the payoff for that concept, and should live in whichever chapter covers gluconeogenesis regulation.

---

## Ch. 7: CFTR as a Worked Example of a Regulated Ion Channel

**Where it belongs:** Chapter 7, after the section on ligand-gated ion channels or as part of the pump/channel clinical examples.

**What's needed:** A brief treatment of CFTR (cystic fibrosis transmembrane conductance regulator) as a chloride channel whose opening is regulated by cAMP/PKA-mediated phosphorylation. Key points: CFTR is a chloride channel, not a pump; it opens when PKA phosphorylates its regulatory domain; this is the normal intestinal secretion mechanism; loss-of-function mutations cause cystic fibrosis; gain-of-function (via cholera toxin locking the upstream G protein on) causes the secretory diarrhea of cholera.

**Why it belongs here:** Chapter 8 (Signal Transduction) references CFTR and Chapter 7 in the cholera case, but CFTR is never actually introduced in Chapter 7. The reference is currently a forward promise with no anchor. Adding CFTR to Chapter 7 would let Chapter 8 use it as established context and also gives Chapter 7 a natural clinical hook connecting ion channels to both cystic fibrosis and infectious disease.
