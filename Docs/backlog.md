# Backlog

Items to revisit. Add context so future-you remembers why it was deferred.

---

## PFK-1 Allosteric Site Structural Details

**Where it belongs:** Chapter 10, Step 3 regulatory bullet points.

**What needs verification:** (1) Does citrate bind its own allosteric site or does it work through/near the AMP/ATP regulatory site? (2) Does F-2,6-BP bind a site distinct from both the substrate (F-6-P) site and the AMP/ATP regulatory site? Current text says each effector acts through allosteric sites without specifying overlap — confirm against a structural reference (e.g., Schirmer & Evans 1990 or a mammalian PFK-1 crystal structure paper) before publication.

**Why deferred:** Structural details complex and species-dependent; beyond pre-med survey scope but should be accurate.

---

## Glucose Origin and Entry into the Cell

**RESOLVED (Chapter 10, 2026-05-31):** Full treatment added as "From Fork to Cell: Getting Glucose In" between The Big Picture and The Logic of Glycolysis sections. Covers starch/sucrose/lactose/glycogen digestion, SGLT1/GLUT5 intestinal absorption, portal circulation, and GLUT1/2/3/4 isoform properties including GLUT4 insulin-regulated translocation and type 2 diabetes connection.

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

**RESOLVED (Chapter 2, 2026-09-06):** Added as two subsections opening Secondary Structure, ahead of The Alpha Helix: "The Ramachandran Plot: What the Backbone Can Actually Do" and "Glycine and Proline: The Two Exceptions". Uses Ramachandran_Generic2.jpg (general case, alpha and beta basins labeled) plus the separate Gly and Pro plots, which make the steric argument visually: no $C_\beta$ opens the whole map for Gly, the pyrrolidine ring collapses Pro to a vertical stripe at $\phi \approx -60°$.

Placed at secondary structure rather than the peptide bond section as originally proposed. The peptide bond section sits under The Amino Acids and is followed by ~110 lines of side chain catalogue, which would have separated the plot from the helix and sheet that give it meaning. The angle definitions stay at the peptide bond section with a forward reference; only the plot moved.

Two accuracy fixes came out of the Pro plot, which shows a well-populated cluster at helical $\phi/\psi$: the claim that proline "cannot" adopt helical angles was wrong and has been corrected in the Alpha Helix section. Proline's $\phi \approx -60°$ is the helical value; it disrupts helices because it has no backbone N-H and its ring clashes with the preceding residue. Ramachandran GN et al. 1963 added as reference 5 (later refs renumbered).

**Still open:** the backlog also asked for a labeled backbone diagram showing which bond each angle describes, to sit next to the definitions at the peptide bond section. Not yet made. Ramachandran_Generic.jpg (the schematic with 3-10, polyproline II, and L-alpha regions labeled) is on disk but unused; it is a candidate if the minor regions ever need naming.

---

## G6PD Deficiency as the Clinical Anchor for NADPH

**Where it belongs:** The pentose phosphate pathway chapter (chapter number TBD), in or immediately after the section explaining what NADPH is used for.

**Why it's great:** G6PD deficiency is the most common human enzyme defect (~400 million people affected), is heavily MCAT-tested, and the mechanism is a perfect illustration of the NADPH story. Without G6PD, the pentose phosphate pathway can't run, NADPH can't be generated, reduced glutathione can't be regenerated, red blood cells can't neutralize oxidative stress, and they lyse. Clinically this presents as hemolytic anemia triggered by oxidative stressors: fava beans, primaquine, dapsone, certain infections. The connection from "NADPH manages oxidative stress" (introduced in Ch. 9) to "here's what happens when that system fails" is exactly the kind of payoff that makes the earlier mechanistic groundwork feel worthwhile.

**Note:** Ch. 9 already introduces NADPH and mentions glutathione reductase as an NADPH-dependent enzyme. G6PD deficiency should be the clinical anchor that cashes that forward reference in.

---

## Alcohol Metabolism, NADH Accumulation, and the NAD+/NADH Ratio

**RESOLVED (Chapter 10, 2026-05-31; Chapter 11, 2026-05-31):** Full treatment added to Chapter 10 as "Alcohol, NAD⁺, and Hypoglycemia" in the When It Breaks section: covers ADH/ALDH reactions, NAD⁺ depletion, gluconeogenesis stall, pyruvate-to-lactate shift, OAA-to-malate shift, and the clinical picture of fasting hypoglycemia in a binge drinker. Chapter 11 adds the downstream note that acetate from alcohol metabolism is activated to acetyl-CoA by acetyl-CoA synthetase, completing the alcohol carbon story through to the TCA cycle.

---

## Ch. 7: CFTR as a Worked Example of a Regulated Ion Channel

**Where it belongs:** Chapter 7, after the section on ligand-gated ion channels or as part of the pump/channel clinical examples.

**What's needed:** A brief treatment of CFTR (cystic fibrosis transmembrane conductance regulator) as a chloride channel whose opening is regulated by cAMP/PKA-mediated phosphorylation. Key points: CFTR is a chloride channel, not a pump; it opens when PKA phosphorylates its regulatory domain; this is the normal intestinal secretion mechanism; loss-of-function mutations cause cystic fibrosis; gain-of-function (via cholera toxin locking the upstream G protein on) causes the secretory diarrhea of cholera.

**Why it belongs here:** Chapter 8 (Signal Transduction) references CFTR and Chapter 7 in the cholera case, but CFTR is never actually introduced in Chapter 7. The reference is currently a forward promise with no anchor. Adding CFTR to Chapter 7 would let Chapter 8 use it as established context and also gives Chapter 7 a natural clinical hook connecting ion channels to both cystic fibrosis and infectious disease.
