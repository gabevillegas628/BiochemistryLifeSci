# Answer Key: Chapters 01–04

*Audience: pre-med undergraduates preparing for the MCAT. Every quantitative problem shows the full calculation. Every synthesis problem walks the reasoning chain explicitly.*

---

## Chapter 1 — Thermodynamic Principles

### Chapter 1 — Problem 1

**Given:** $\Delta H^{\circ'} = +12$ kJ/mol; $\Delta S^{\circ'} = +60$ J/mol·K = 0.060 kJ/mol·K; $T = 310$ K.

**(a) Calculate $\Delta G^{\circ'}$ at 37°C.**

$$\Delta G^{\circ'} = \Delta H^{\circ'} - T\Delta S^{\circ'} = +12 - (310)(0.060) = +12 - 18.6 = \mathbf{-6.6 \text{ kJ/mol}}$$

**(b) Spontaneity under standard conditions at 37°C.**

$\Delta G^{\circ'} = -6.6$ kJ/mol is negative, so the reaction **is spontaneous** under standard conditions at this temperature. The entropy gain ($T\Delta S = +18.6$ kJ/mol) outweighs the unfavorable enthalpy ($+12$ kJ/mol).

**(c) Temperature of thermodynamic neutrality ($\Delta G^{\circ'} = 0$).**

Set $\Delta H^{\circ'} = T\Delta S^{\circ'}$:

$$T = \frac{\Delta H^{\circ'}}{\Delta S^{\circ'}} = \frac{+12{,}000 \text{ J/mol}}{60 \text{ J/molK}} = \mathbf{200 \text{ K}}$$

**Interpretation:**
- **Below 200 K:** $T\Delta S < \Delta H$, so $\Delta G > 0$ — the reaction is non-spontaneous. Enthalpy dominates unfavorably.
- **Above 200 K:** $T\Delta S > \Delta H$, so $\Delta G < 0$ — the reaction is spontaneous. Entropy wins.

This is an **entropy-driven** reaction: it only becomes favorable when temperature is high enough to make the $T\Delta S$ term overcome the endothermic enthalpy.

---

### Chapter 1 — Problem 2

**Given:** Reaction 1: $A \to B$, $\Delta G^{\circ'} = +18$ kJ/mol. Reaction 2: $B + \text{ATP} + H_2O \to C + \text{ADP} + P_i$, $\Delta G^{\circ'} = -25$ kJ/mol.

**(a) Can Reaction 1 proceed spontaneously on its own?**

No. $\Delta G^{\circ'} = +18$ kJ/mol is positive, meaning the reaction is **thermodynamically unfavorable** under standard conditions. It requires an energy input to proceed.

**(b) Net $\Delta G^{\circ'}$ for the overall conversion of $A$ to $C$.**

When reactions share an intermediate and are coupled, their free energies are additive:

$$\Delta G^{\circ'}_{\text{net}} = +18 + (-25) = \mathbf{-7 \text{ kJ/mol}}$$

The overall conversion of $A$ to $C$ is spontaneous under standard conditions. ATP hydrolysis provides the thermodynamic "pull" that rescues the unfavorable first step.

**(c) Why the student is wrong about not needing a shared intermediate.**

The student's math is arithmetically correct but mechanistically wrong. Thermodynamic coupling is not just a bookkeeping convenience — it requires a **physical connection** between the two reactions. For the free energies to add, the product of Reaction 1 (compound $B$) must be the actual substrate consumed in Reaction 2. Only then is there a single coupled equilibrium. If $B$ is not shared — if the reactions happen in separate compartments or involve entirely different molecules — there is no mechanism by which the favorable energy of ATP hydrolysis can drive the formation of $B$ from $A$. The free energy of the second reaction cannot be "transferred" to the first unless the two reactions are mechanistically linked through a common intermediate.

---

### Chapter 1 — Problem 3

**Given:** $\Delta G^{\circ'} = -30.5$ kJ/mol; $R = 0.008314$ kJ/mol·K; $T = 310$ K.

The actual free energy equation is:

$$\Delta G = \Delta G^{\circ'} + RT\ln Q = \Delta G^{\circ'} + RT\ln\frac{[\text{ADP}][P_i]}{[\text{ATP}]}$$

**(a) $\Delta G$ at resting conditions: [ATP] = 8 mM, [ADP] = 0.9 mM, $[P_i]$ = 1.0 mM.**

$$Q = \frac{(0.9 \times 10^{-3})(1.0 \times 10^{-3})}{8 \times 10^{-3}} = \frac{9.0 \times 10^{-7}}{8 \times 10^{-3}} = 1.125 \times 10^{-4}$$

$$RT = (0.008314)(310) = 2.577 \text{ kJ/mol}$$

$$\Delta G = -30.5 + 2.577 \times \ln(1.125 \times 10^{-4})$$

$$\ln(1.125 \times 10^{-4}) = \ln(1.125) + \ln(10^{-4}) = 0.118 - 9.210 = -9.092$$

$$\Delta G = -30.5 + 2.577 \times (-9.092) = -30.5 - 23.4 = \mathbf{-53.9 \text{ kJ/mol}}$$

**(b) $\Delta G$ during intense exercise: [ATP] = 6 mM, [ADP] = 2 mM, $[P_i]$ = 4 mM.**

$$Q = \frac{(2 \times 10^{-3})(4 \times 10^{-3})}{6 \times 10^{-3}} = \frac{8 \times 10^{-6}}{6 \times 10^{-3}} = 1.333 \times 10^{-3}$$

$$\ln(1.333 \times 10^{-3}) = \ln(1.333) + \ln(10^{-3}) = 0.288 - 6.908 = -6.620$$

$$\Delta G = -30.5 + 2.577 \times (-6.620) = -30.5 - 17.1 = \mathbf{-47.6 \text{ kJ/mol}}$$

**Comparison:** The actual $\Delta G$ becomes **less negative** during exercise (from $-53.9$ to $-47.6$ kJ/mol). The driving force for ATP hydrolysis decreases. This makes sense: as ATP is consumed and ADP/$P_i$ accumulate, the reaction approaches equilibrium. The cell is spending its thermodynamic currency faster than it can regenerate it.

**(c) Flaw in the "maximize [ATP]" argument.**

The flaw is self-defeating. The $\Delta G$ equation has the ratio $[\text{ADP}][P_i]/[\text{ATP}]$ inside the logarithm. Maximizing [ATP] necessarily depletes [ADP] and $[P_i]$ (the adenine nucleotide pool is conserved: [ATP] + [ADP] + [AMP] ≈ constant). As [ADP] → 0, two things happen: (1) the ratio approaches zero, making $\ln Q$ more negative and $\Delta G$ more negative — so in pure thermodynamic terms, high [ATP] does increase the driving force; but (2) ADP is the **substrate** for ATP synthase. Without ADP, the mitochondrial ATP synthase has no substrate and stops making ATP entirely. The cell would quickly burn through all ATP with no way to regenerate it. Biology needs not just favorable thermodynamics but also the substrates to sustain the chemistry.

---

### Chapter 1 — Problem 4

**(a) Protein unfolding in hot water (heat absorbed; unfolded chain more flexible).**

- $\Delta H > 0$: heat is absorbed from surroundings, so the process is endothermic.
- $\Delta S > 0$: the unfolded chain has far more conformational freedom than the folded structure, so disorder increases.
- $\Delta G$: indeterminate from the information given alone — it depends on temperature. Since the protein actually unfolds in hot water, we can infer $\Delta G < 0$ at that temperature (the $T\Delta S$ term has overcome $\Delta H$). At lower temperatures the same protein would remain folded ($\Delta G > 0$). This is the classic entropy-driven, enthalpy-opposed unfolding seen in thermal denaturation.

**(b) Ions of opposite charge forming a tight ion pair; no heat exchanged.**

- $\Delta H = 0$: no heat exchanged with surroundings by definition.
- $\Delta S < 0$: two freely diffusing ions become one constrained pair; translational and rotational degrees of freedom decrease. Water molecules around each ion also become partially reordered upon pairing.
- $\Delta G = \Delta H - T\Delta S = 0 - T(\text{negative}) > 0$: **non-spontaneous** under these stated conditions. This result is counterintuitive given that opposite charges attract, but the stated conditions (no enthalpy change) strip away the electrostatically favorable enthalpy contribution. In reality, ion pairing in water is accompanied by a favorable $\Delta H$ from electrostatic attraction and release of ordered water; the problem isolates the entropic component to show that entropy alone opposes the association.

**(c) ATP hydrolysis inside a cell at 37°C.**

- $\Delta H < 0$: phosphoanhydride bond hydrolysis is exothermic; heat is released.
- $\Delta S > 0$: one molecule becomes two ($\text{ATP} \rightarrow \text{ADP} + P_i$), increasing translational entropy; the highly charged products also disorder surrounding water.
- $\Delta G$: strongly negative under cellular conditions. As shown in Problem 3, the standard $\Delta G^{\circ'} = -30.5$ kJ/mol is pushed even more negative by the cellular [ATP]/[ADP][$P_i$] ratio to approximately $-50$ kJ/mol. Both terms ($-T\Delta S$ and $\Delta H$) favor spontaneity.

---

### Chapter 1 — Problem 5

**Given:** pKa of lactic acid = 3.86. Intracellular pH ≈ 7.2; plasma pH = 7.4.

**(a) Ratio of lactate to lactic acid at each pH.**

Henderson-Hasselbalch: $\text{pH} = \text{p}K_a + \log\frac{[\text{A}^-]}{[\text{HA}]}$, so $\log\frac{[\text{lactate}]}{[\text{lactic acid}]} = \text{pH} - \text{p}K_a$.

- **At pH 7.2:** $\log\frac{[\text{A}^-]}{[\text{HA}]} = 7.2 - 3.86 = 3.34$, so the ratio is $10^{3.34} \approx 2{,}200:1$ (lactate:lactic acid).
- **At pH 7.4:** $\log\frac{[\text{A}^-]}{[\text{HA}]} = 7.4 - 3.86 = 3.54$, so the ratio is $10^{3.54} \approx 3{,}500:1$.

Both values are enormous. Plasma has an even more extreme ratio than intracellular fluid.

**(b) Dominant form and charge on the transported molecule.**

Lactate ($\text{A}^-$, the deprotonated anion) dominates overwhelmingly in both compartments — by more than 2,000-fold over lactic acid in either location. Essentially every molecule present is lactate. The form transported across the plasma membrane is therefore **lactate**, carrying a single negative charge ($-1$). It exits the muscle cell via monocarboxylate transporters (MCTs) as lactate, not as lactic acid.

**(c) Molecular basis of enzyme disruption at pH 7.1.**

Enzyme active sites depend on ionizable residues — particularly histidine (pKa ≈ 6.0–7.0), aspartate (pKa ≈ 3–4), glutamate (pKa ≈ 4), lysine (pKa ≈ 10), and cysteine (pKa ≈ 8) — being in a precise protonation state to carry out catalysis. Normal blood pH (7.4) maintains these residues at specific charge states that enable hydrogen bonding, nucleophilic attack, and proton relay. A drop to pH 7.1 shifts equilibria toward more protonated forms. For histidine, whose pKa can be tuned toward 7 in many active sites, even a 0.3-unit pH drop meaningfully increases the fraction in the protonated ($\text{His}^+H$) form. If that residue normally acts as a general base (deprotonated), it is now partially inactivated. Beyond individual residues, protonation of surface charges can alter protein conformation by disrupting stabilizing electrostatic interactions, affecting not just catalytic residues but the overall active-site geometry. Enzymes that require a histidine-mediated proton shuttle — like carbonic anhydrase, serine proteases, and many kinases — are particularly sensitive.

---

### Chapter 1 — Problem 6

**Given:** DNP is a lipid-soluble weak acid, pKa ≈ 4. IMS pH ≈ 6.7; matrix pH ≈ 7.9.

**(a) Ionization state in the IMS (pH 6.7).**

$\log\frac{[\text{DNP}^-]}{[\text{DNPH}]} = 6.7 - 4.0 = 2.7$, so the ratio is $10^{2.7} \approx 500:1$.

DNP is **predominantly deprotonated** (DNP$^-$) in the IMS. However, the ratio of deprotonated to protonated is "only" 500:1 — meaning roughly 1 in 500 molecules is in the neutral DNPH form, available to cross the membrane.

**(b) Ionization state in the matrix (pH 7.9).**

$\log\frac{[\text{DNP}^-]}{[\text{DNPH}]} = 7.9 - 4.0 = 3.9$, so the ratio is $10^{3.9} \approx 8{,}000:1$.

DNP is **even more strongly deprotonated** in the matrix. Essentially no DNPH exists there under normal conditions.

**(c) How DNP shuttles protons and why this uncouples ATP synthesis.**

The proton gradient across the inner mitochondrial membrane creates a higher proton concentration (lower pH) in the IMS than in the matrix. DNP exploits this asymmetry:

1. In the IMS (pH 6.7), a small fraction of DNP$^-$ picks up a proton to become neutral DNPH.
2. DNPH is lipid-soluble and diffuses freely through the hydrophobic membrane into the matrix.
3. In the matrix (pH 7.9), the higher pH drives deprotonation: $\text{DNPH} \rightarrow \text{DNP}^- + \text{H}^+$. The proton is released into the matrix.
4. DNP$^-$ diffuses back to the IMS (it is membrane-permeant as a hydrophobic anion) and the cycle repeats.

Net result: protons are shuttled from IMS to matrix, **collapsing the proton-motive force** without passing through ATP synthase. ATP synthase spins only when protons flow through it; with the gradient dissipated, it stops. The energy released by electron transport is wasted as heat rather than captured as ATP. Because the cell's metabolic rate increases to compensate (attempting to restore the gradient), oxidation of fuel accelerates and calories are burned — hence historical (and dangerous) use of DNP as a weight-loss agent.

---

### Chapter 1 — Problem 7

**Given:** Bicarbonate buffer pKa = 6.1; normal blood pH = 7.4.

**(a) Hyperventilation: blowing off CO$_2$.**

The relevant equilibrium is:
$$CO_2 + H_2O \rightleftharpoons H_2CO_3 \rightleftharpoons H^+ + HCO_3^-$$

When $CO_2$ is exhaled in excess, the left side of the equilibrium is depleted. By Le Chatelier's principle, the equilibrium shifts **left**, consuming $H^+$ and $HCO_3^-$ to regenerate $CO_2$. The net effect is removal of $H^+$ from blood. Blood pH **rises** (respiratory alkalosis). Clinically, a drop in ionized $Ca^{2+}$ at higher pH (due to increased protein binding) causes the tingling and tetany described in Problem 2 of Chapter 3.

**(b) Prolonged vomiting: loss of gastric HCl.**

Gastric acid ($HCl$) secretion removes $H^+$ from the blood into the stomach lumen. Vomiting loses this $H^+$ externally rather than reabsorbing it in the intestine. Net result: $H^+$ is removed from the body, blood pH **rises** (alkalosis). Because the primary cause is loss of metabolic acid (not altered ventilation), this is **metabolic alkalosis**. The lungs may compensate by retaining $CO_2$ (hypoventilation), but the initiating disturbance is metabolic.

**(c) Why bicarbonate buffers effectively despite pKa being 1.3 units below physiological pH.**

At pH 7.4, the ratio $[\text{HCO}_3^-]/[\text{CO}_2] = 10^{(7.4 - 6.1)} = 10^{1.3} \approx 20:1$. The system is operating far from its optimal buffering range (which would be at pH ≈ 6.1 ± 1). A closed buffer at this displacement would be rapidly exhausted.

What makes bicarbonate work is that it is an **open system**. Two physiological regulators continuously replenish or drain the buffer components:
- The **lungs** control $[\text{CO}_2]$ by adjusting ventilation within seconds to minutes.
- The **kidneys** control $[\text{HCO}_3^-]$ by adjusting excretion or reabsorption over hours to days.

A standard chemical buffer has a fixed quantity of each component. The bicarbonate system has effectively unlimited capacity because the lungs can exhale $CO_2$ as fast as it is produced, and the kidneys can generate or excrete bicarbonate on demand. This physiological "buffering" of the buffer itself is what allows an apparently mismatched pKa to serve as the dominant buffer in blood.

---

### Chapter 1 — Problem 8

**The colleague is wrong. Thermodynamics and kinetics are distinct.**

The colleague confuses two separate questions: (1) *Can* this reaction proceed, and (2) *How fast* does it proceed? Thermodynamics answers the first; kinetics answers the second.

A negative $\Delta G^{\circ'} = -45$ kJ/mol means the products are more stable than the reactants — the reaction is thermodynamically favorable and will *eventually* reach equilibrium in the forward direction. But thermodynamics says nothing about the rate at which equilibrium is approached. A reaction with highly favorable $\Delta G$ can still be imperceptibly slow if the activation energy barrier is high.

**What the drug actually exploits is kinetics.** Enzyme inhibitors work by blocking or distorting the active site so that the enzyme can no longer stabilize the transition state. Enzymes accelerate reactions by lowering the activation energy $E_a$, not by changing $\Delta G^{\circ'}$. When the inhibitor prevents the enzyme from functioning, the uncatalyzed reaction proceeds at whatever its inherent (extremely slow) rate is. At 37°C with a high $E_a$, that rate may be negligible on any biologically relevant timescale.

Crucially, $\Delta G^{\circ'}$ is a **state function** — it depends only on the energy difference between reactants and products, not on the pathway or the catalyst. The enzyme's presence or absence does not change $\Delta G^{\circ'}$ or the equilibrium constant $K_{eq}$. What the enzyme changes — and what the drug blocks — is the height of the energy barrier between them. The drug does not prevent the reaction from being thermodynamically favorable; it simply removes the molecular machinery that makes it fast.

---

## Chapter 2 — Protein Composition and Structure

### Chapter 2 — Problem 1

**Peptide at pH 7.4: Asp–Trp–Lys–Pro–Glu–His**

**(a) Side-chain charges and net charge.**

| Residue | Side-chain pKa | Charge at pH 7.4 |
|---|---|---|
| Asp | ~3.65 | $-1$ (deprotonated carboxylate) |
| Trp | none | $0$ (nonpolar indole) |
| Lys | ~10.5 | $+1$ (protonated amino group) |
| Pro | none | $0$ (no ionizable side chain) |
| Glu | ~4.1 | $-1$ (deprotonated carboxylate) |
| His | ~6.0 | $\approx 0$ (predominantly deprotonated at pH 7.4) |

**Net charge (side chains only): $-1 + 0 + 1 + 0 + (-1) + 0 = -1$**

Note on His: at pH 7.4 with pKa 6.0, the ratio $[\text{His}]/[\text{His}^+\text{H}] = 10^{1.4} \approx 25$, so only ~4% is protonated. The net charge contribution is approximately $-0.04$, which rounds to zero for this analysis. For exact calculation, net charge ≈ $-1.04$.

**(b) Hydrophobic core vs. surface placement.**

- **Hydrophobic core:** **Trp**. Tryptophan has a large, nonpolar aromatic indole ring. Burial in the hydrophobic core is thermodynamically favorable because it removes the nonpolar surface from water, reducing the entropic cost of solvation (the hydrophobic effect).
- **Expected on the protein surface:** **Asp, Lys, Glu, His**. All carry ionizable, polar side chains. Charged residues are energetically penalized if buried in the low-dielectric core; they stabilize much better when exposed to solvent water, which can solvate their charges. Pro may appear at turns on the surface.

**(c) Effect of proline insertion in the middle of an alpha helix.**

Proline would **disrupt and terminate the helix** at its position. Two structural reasons:
1. Proline's side chain is covalently bonded back to its own backbone nitrogen, eliminating the N–H group. Alpha helices are stabilized by N–H···O=C hydrogen bonds between residue $i$ and residue $i+4$; without the N–H, the hydrogen bond at that position cannot form.
2. The pyrrolidine ring rigidly fixes the $\phi$ backbone dihedral angle to approximately $-60°$, which is incompatible with the regular $\phi/\psi$ angles required for a right-handed alpha helix.

The result is a pronounced kink or break at the proline position, dividing one continuous helix into two shorter ones. Proline is sometimes called a "helix breaker" for exactly this reason, and it is commonly found at turns and loops rather than in helical segments.

---

### Chapter 2 — Problem 2

**Setup:** Single-domain protein, two cysteines, one disulfide bond.

**(a) Will the protein regain activity after urea denaturation without reducing agent?**

**Yes, it should.** The Anfinsen framework states that the native conformation of a protein is determined entirely by its amino acid sequence — specifically, the native state is the thermodynamic free-energy minimum accessible to that sequence under physiological conditions. Because the disulfide bond was NOT broken (no reducing agent was used), the covalent connectivity of the protein is completely preserved. When urea is removed by dialysis, the polypeptide chain is free to refold, and the thermodynamic minimum it will find is the same native conformation it occupied before denaturation. The disulfide bond was never scrambled, so there is no obstacle to correct refolding. Enzymatic activity should be fully restored.

**(b) What does the urea + BME experiment confirm and rule out?**

This experiment **confirms** the Anfinsen hypothesis: the primary structure (sequence) alone contains all the information necessary to specify the correct three-dimensional native conformation, including the correct disulfide pairing. When both the non-covalent interactions (disrupted by urea) and the disulfide bond (reduced by BME) are eliminated and then allowed to reform under oxidizing conditions, the protein finds its way back to the unique native structure.

It **rules out** the possibility that the native conformation requires extrinsic cofactors, template proteins, or post-translational covalent modifications beyond what is encoded in the sequence. It also rules out the idea that the specific disulfide bond pairing requires assistance from cellular chaperones to be formed correctly (at least for this simple protein).

**(c) Why does a four-disulfide protein recover only 5% activity despite full secondary structure recovery?**

The discrepancy arises from **incorrect disulfide pairing**. A protein with four disulfide bonds has 8 cysteine residues. When all disulfides are reduced and the protein unfolds, the 8 cysteines must reform 4 correct disulfide bonds upon reoxidation. The number of possible pairings among 8 cysteines is $\frac{7 \times 5 \times 3 \times 1}{1} = 105$ distinct combinations, but only one combination gives the native structure. Random reoxidation produces a mixture of incorrect "scrambled" proteins, most of which happen to adopt substantial secondary structure (alpha helices and beta strands can form locally, independent of disulfide connectivity) but not the correct tertiary fold required for catalysis. Since enzymatic activity requires precise three-dimensional geometry at the active site, only the ~5% that happen to reform all four native disulfide bonds are active. Circular dichroism reports on secondary structure content, not on tertiary structure — so it looks "normal" even in the misfolded majority.

---

### Chapter 2 — Problem 3

**(a) Why the hydrophobic effect is fundamentally entropic.**

When a nonpolar solute is dissolved in water, the surrounding water molecules cannot form hydrogen bonds with it. Instead, they rearrange into highly ordered "cages" around the nonpolar surface — a configuration that is structurally ordered and entropically costly. This organized shell of water molecules represents a significant decrease in the entropy of the solvent.

When two nonpolar groups come together (aggregate), they bury their shared surface from water. The water molecules that had been caging each group are released into bulk solvent, where they can hydrogen bond freely and adopt many orientations. This **release of ordered water** is an increase in entropy of the system. The driving force for hydrophobic collapse is not attraction between the nonpolar groups themselves (there is no special "hydrophobic bond") — it is the entropy gain of the water.

**(b) Why hydrophobic driving force increases with temperature; implications for protein stability.**

In $\Delta G = \Delta H - T\Delta S$, the entropy-driven term appears as $-T\Delta S$. If $\Delta S > 0$ (water is released, disorder increases), then $-T\Delta S$ is negative and becomes more negative as $T$ increases. This means the hydrophobic contribution to protein stability *strengthens* as temperature rises, up to a point.

Counterintuitively, this predicts that proteins should become **more stable** as temperature increases modestly — and indeed many proteins show a phenomenon called "cold denaturation" at very low temperatures, where the reduced $T\Delta S$ term makes hydrophobic burial less favorable, allowing the protein to partially unfold. At very high temperatures, however, other effects (disruption of hydrogen bonds, increased conformational entropy of the chain) dominate and cause heat denaturation. The net result is a stability curve with a maximum somewhere between 0°C and the denaturation temperature.

**(c) Evaluating the argument that hydrogen bonds cannot drive folding.**

The student's argument is **partially correct but misleading**. The argument that an unfolded protein also makes hydrogen bonds with water is true — exposed backbone N–H and C=O groups in the unfolded state are fully hydrogen-bonded to water. When the protein folds, these backbone groups hydrogen bond to each other instead of to water. In a simple accounting, the number of hydrogen bonds formed is roughly conserved; the net enthalpy change from backbone hydrogen bonding alone is small.

However, the argument is incomplete. What hydrogen bonds do provide is **specificity and cooperativity**. Two hydrogen bonds between a folded helix's $i$ and $i+4$ residues are in a geometrically optimized arrangement that is more stable per bond than hydrogen bonds to water (which are dynamic and less directional). More importantly, the argument ignores that hydrogen bonds in the protein interior are in a **low-dielectric environment**, which dramatically strengthens their interaction energy compared to hydrogen bonds in aqueous solution. So while hydrogen bonding is not the primary *driving force* (that is entropy from the hydrophobic effect), hydrogen bonds stabilize specific secondary and tertiary structures and contribute meaningfully to the overall folding energy. The student is right that they cannot be *the main driving force*, but wrong to dismiss them as having no net stabilizing contribution.

---

### Chapter 2 — Problem 4

**Sickle cell disease: Glu→Val substitution at position 6 of the beta chain.**

**(a) Charges on glutamate and valine at pH 7.4.**

- **Glutamate** side chain pKa ≈ 4.1. At pH 7.4, which is far above 4.1, the side chain is fully deprotonated: $\text{charge} = -1$.
- **Valine** has no ionizable side chain (it is a branched-chain aliphatic amino acid). Its side chain carries $\text{charge} = 0$ at any physiological pH.

**(b) Why valine at a surface position is "thermodynamically frustrated."**

Position 6 is on the **surface** of the HbA subunit, where it is exposed to aqueous solvent. Residues on protein surfaces are almost always hydrophilic or charged, because placing them there allows favorable solvation by water. Glutamate at this position is perfectly placed: its $-1$ charge is stabilized by hydrogen bonding and ion-dipole interactions with surrounding water molecules.

Valine is **nonpolar**. Placing a hydrophobic residue on an exposed surface forces surrounding water to form ordered solvation shells — the same entropic penalty described in Problem 3. This is thermodynamically unfavorable: the nonpolar surface "wants" to be buried. The protein is "frustrated" because the sequence demands that valine sit on the surface (the rest of the polypeptide chain determines its position), but thermodynamically, that position is wrong for valine. This frustrated surface patch creates a hydrophobic sticky spot that drives HbS polymerization.

**(c) Why deoxygenation specifically triggers polymerization.**

The conformational difference between oxygenated hemoglobin (R-state) and deoxygenated hemoglobin (T-state) is the key. In the R-state (HbO$_2$), the beta chains are in a conformation that positions the Val-6 patch in a way that partially buries or repositions it, reducing its exposure. In the T-state (deoxy-HbS), the beta chains adopt a different conformation that exposes the Val-6 hydrophobic patch more fully and presents it in a geometry that is complementary to a hydrophobic acceptor pocket on an adjacent deoxy-HbS molecule (specifically the EF corner of the beta chain of a neighboring tetramer). This geometry is not present in the R-state. Therefore, polymerization is deoxygenation-specific: only when HbS transitions to the T-state does the surface chemistry support the intermolecular contacts required for fibril formation. Conditions that increase T-state occupancy — low pO$_2$, acidosis (Bohr effect), elevated 2,3-BPG, dehydration — all precipitate crises.

---

### Chapter 2 — Problem 5

**Active-site histidine with free-solution pKa = 6.0; nearby Lys (pKa ~10.5, always +1 at pH 7.4).**

**(a) Fraction of free histidine protonated at pH 7.4.**

Using Henderson-Hasselbalch: $\text{pH} = \text{p}K_a + \log\frac{[\text{His}]}{[\text{His}^+\text{H}]}$

$$7.4 = 6.0 + \log\frac{[\text{His}]}{[\text{His}^+\text{H}]}$$

$$\log\frac{[\text{His}]}{[\text{His}^+\text{H}]} = 1.4 \implies \frac{[\text{His}]}{[\text{His}^+\text{H}]} = 10^{1.4} \approx 25.1$$

So $\frac{[\text{His}^+\text{H}]}{[\text{His}]} \approx 0.040$. The fraction protonated $= \frac{1}{1 + 25.1} \approx 3.8\%$.

**(b) Effect of neighboring Lys$^+$ on the apparent pKa of His.**

A neighboring positive charge $\text{Lys}^+$ creates an electrostatic environment that **lowers** the apparent pKa of histidine. Here is why: for histidine to be protonated $\text{His}^+$, carrying $+1$ charge, it must exist in close proximity to the already-positive $\text{Lys}^+$. Like charges repel, so placing a $+1$ charge near another $+1$ charge is energetically unfavorable. This destabilizes the protonated form $\text{His}^+$ relative to the neutral form ( $\text{His}$ ). Destabilizing the protonated form means histidine has less tendency to hold a proton — its pKa decreases. A positive electrostatic environment makes it harder to be protonated; a negative environment (e.g., nearby $\text{Asp}^-$ ) would stabilize $\text{His}^+$ and raise the pKa.

**(c) Functional significance of pKa ≈ 7.4 at the active site.**

At pH = pKa = 7.4:

$$\text{fraction protonated} = \frac{1}{1 + 10^{(7.4-7.4)}} = \frac{1}{1+1} = \mathbf{50\%}$$

This shift from 3.8% (free histidine) to 50% (active-site histidine) is profoundly important. At physiological pH, an active-site histidine with pKa 7.4 exists in **equal amounts of the protonated and deprotonated forms**. This means:
- Half the histidines can donate a proton (act as a Brønsted acid).
- Half can accept a proton (act as a Brønsted base).
- The enzyme is poised to shuttle protons at physiological pH — the essential requirement for a general acid-base catalyst.

If the pKa remained at 6.0, only 4% of residues would be protonated at pH 7.4, leaving 96% as the deprotonated base form — a poor acid catalyst. The active-site environment effectively tunes histidine to be a maximally versatile proton shuttle at exactly the pH where the enzyme operates.

---

### Chapter 2 — Problem 6

**Cystic fibrosis $\Delta$F508: deletion of Phe-508 from CFTR.**

**(a) Why deleting Phe-508 disrupts tertiary structure.**

Phenylalanine is a large aromatic residue with a bulky hydrophobic side chain. Position 508 is in the interior of a structural domain (NBD1, the first nucleotide-binding domain). In a well-folded protein, every interior position is occupied by a residue whose size and shape contributes to the tight packing of the hydrophobic core. Phe-508 fills a specific cavity in the core; its aromatic ring makes van der Waals contacts with several surrounding residues and contributes to the burial of hydrophobic surface area.

When Phe-508 is deleted, a cavity forms in the core. This is thermodynamically destabilizing for two reasons: (1) the hydrophobic contacts that Phe provided are lost, reducing the buried nonpolar surface area; and (2) the remaining surrounding residues no longer pack tightly against anything — the geometry of the core is disrupted, introducing strain and flexibility into a region that is normally rigid. The domain cannot reach its native conformation and is instead trapped in a partially folded, kinetically accessible intermediate.

**(b) Why misfolded CFTR is a substrate for Hsp70; what Hsp70 binding prevents.**

Hsp70 recognizes and binds **exposed hydrophobic patches** on partially folded or misfolded proteins. In a correctly folded protein, hydrophobic residues are buried in the core, away from solvent. When $\Delta$F508-CFTR fails to complete folding, the disrupted NBD1 domain exposes hydrophobic segments that would normally be internal. These patches are the signal Hsp70 reads.

Hsp70 binding serves two purposes: (1) it **prevents aggregation** — exposed hydrophobic patches from different misfolded chains will tend to associate with each other unless blocked; Hsp70 caps these patches, preventing intermolecular contact; and (2) it **holds the protein in a folding-competent state**, giving it repeated opportunities to attempt folding with the assistance of co-chaperones (Hsp40, NEF). If folding still fails after repeated attempts, Hsp70 hands the substrate off to the ubiquitin-proteasome pathway for degradation.

**(c) The drug's thermodynamic mechanism — what it changes and what it does not.**

A thermodynamic intervention (as opposed to a covalent repair) does not fix the primary structure or the missing amino acid. The deletion still exists. What the corrector drug changes is the **free energy landscape of folding**: by binding to the partially folded intermediate, it stabilizes that intermediate relative to the unfolded state and lowers the energy barrier between the intermediate and the near-native conformation. In Gibbs terms, the drug shifts the folding equilibrium: $K_{eq} = [\text{folded}]/[\text{unfolded}]$ increases because the drug raises the stability of forms that resemble the native state.

What it does **not** change: the amino acid sequence is unchanged; the protein still lacks Phe-508; the mutant native state is still less stable than wild-type CFTR; and the corrector must remain present to maintain the shift. The result is a CFTR protein that reaches the plasma membrane in a conformation close enough to native to pass ER quality control and have partial channel function (typically augmented further by potentiators like ivacaftor). It is a pharmacological stabilization, not a molecular repair.

---

### Chapter 2 — Problem 7

**Two peptides of identical length and composition but different sequences: A folds, B does not.**

**(a) What the difference in folding behavior tells us.**

It tells us that amino acid **sequence** — not just composition — determines three-dimensional structure. Two polypeptides can contain exactly the same set of residues, but if those residues are arranged in different orders, the pattern of hydrophobic, polar, and charged side chains along the chain will be completely different. Peptide A has a sequence in which hydrophobic residues cluster in the right positions to form a stable buried core, and polar/charged residues are positioned on the surface. Peptide B's scrambled sequence places hydrophobic and hydrophilic residues randomly, preventing the formation of a stable hydrophobic core and coherent secondary structure contacts. The information for a specific fold is not in the amino acid *inventory* but in the *arrangement*.

**(b) What the Anfinsen refolding result tells us; what it rules out.**

The result — full structural and functional recovery after urea removal — **tells us** that the primary structure contains all the information needed to specify the native conformation. The sequence is sufficient; no external template, chaperone, or cell-specific modification is required for this protein to fold correctly. The thermodynamic minimum of the folding energy landscape is uniquely specified by the sequence.

It **rules out** that the protein's native structure depends on: (1) a template or mold from the cell that must be inherited; (2) post-translational modifications that cannot re-form in vitro; or (3) irreversible covalent changes during initial folding. It confirms Anfinsen's thermodynamic hypothesis.

**(c) Interpretation of the disulfide-trapping experiment.**

This result is a textbook illustration of the **kinetic trap problem** and its resolution through disulfide shuffling.

Without reducing agent (standard Anfinsen refolding): the protein refolds correctly because only one disulfide bond must re-form correctly — straightforward.

With BME followed by non-oxidizing dialysis: the disulfide cannot re-form. The protein's non-covalent folding information is still intact, so the backbone folds, but the disulfide is absent. Without the cross-link that stabilizes the native state, the protein may not maintain its correct tertiary geometry, explaining lost activity.

With BME + non-oxidizing dialysis + subsequent addition of a small amount of reducing agent (allowing disulfide shuffling): over 24 hours, ~90% activity is recovered. This confirms the Anfinsen framework fully: the sequence contains the thermodynamic information for the correct fold, including the correct disulfide bond. When given the opportunity to re-sample disulfide pairings (via low-level thiol/disulfide exchange), the polypeptide chain finds the thermodynamically stable native conformation with the correct bond. The 24-hour timescale reflects the slow, stochastic process of shuffling, not the absence of the information.

---

## Chapter 3 — Molecular Binding and Hemoglobin

### Chapter 3 — Problem 1

**Myoglobin $P_{50}$ = 2 mmHg; hemoglobin $P_{50}$ = 26 mmHg, Hill coefficient ≈ 2.8.**

**(a) Myoglobin fractional saturation at 100 mmHg and 30 mmHg.**

$$\theta = \frac{pO_2}{P_{50} + pO_2}$$

- **Lungs ($pO_2$ = 100 mmHg):** $\theta = \frac{100}{2 + 100} = \frac{100}{102} \approx 0.980$ (98.0%)
- **Resting tissue ($pO_2$ = 30 mmHg):** $\theta = \frac{30}{2 + 30} = \frac{30}{32} \approx 0.938$ (93.8%)

**(b) Oxygen delivery efficiency of myoglobin as a systemic carrier.**

Delivery per pass = saturation at lungs $-$ saturation at tissue $= 98.0\% - 93.8\% = \mathbf{4.2\%}$ of total oxygen-carrying capacity.

This is physiologically useless as a systemic carrier. Myoglobin's hyperbolic binding curve with a very low $P_{50}$ means it is nearly fully saturated at virtually all oxygen tensions found in the body — it grips oxygen tightly everywhere and releases very little in tissues. A systemic carrier must load efficiently in the lungs AND unload efficiently in the tissues. Myoglobin can only do the former.

**(c) Structural feature of hemoglobin that accounts for superior delivery.**

**Cooperativity**, produced by the tetrameric allosteric structure of hemoglobin ($\alpha_2\beta_2$). The T-to-R conformational transition means the first oxygen bound increases the affinity for subsequent oxygens. The result is a **sigmoidal** (S-shaped) binding curve. The sigmoid is steep in the region between tissue $pO_2$ (~30 mmHg) and lung $pO_2$ (~100 mmHg), which means hemoglobin loads and unloads oxygen efficiently over exactly the range of partial pressures encountered physiologically. A hyperbolic curve (like myoglobin's) cannot achieve this because it is already nearly flat at those partial pressures.

---

### Chapter 3 — Problem 2

**Medical student hyperventilating; fingers tingle and stiffen.**

**(a) What happens to blood pH when $pCO_2$ falls.**

The bicarbonate equilibrium: $CO_2 + H_2O \rightleftharpoons H_2CO_3 \rightleftharpoons H^+ + HCO_3^-$

Hyperventilation blows off $CO_2$, reducing $[CO_2]$ on the left side. By Le Chatelier's principle, the equilibrium shifts left, consuming $H^+$. Blood $[H^+]$ falls, so blood **pH rises** — this is acute respiratory alkalosis. Even a modest rise (e.g., pH 7.4 → 7.55) is physiologically significant.

**(b) Bohr effect: what the pH rise does to hemoglobin's oxygen affinity.**

The Bohr effect states that **higher pH increases hemoglobin's oxygen affinity** (lower $P_{50}$) and shifts the oxygen-hemoglobin dissociation curve to the **left**. Mechanistically: at higher pH, key histidine residues (particularly $\beta$His-146) on hemoglobin lose protons, weakening the salt bridges that stabilize the T-state. Hemoglobin is pushed toward the R-state (high-affinity oxy conformation), even in the absence of oxygen. The $P_{50}$ decreases; hemoglobin binds oxygen more tightly.

**(c) Why peripheral tissues receive less oxygen despite high blood oxygenation.**

Here is the apparent paradox resolved: the student's blood is near 100% saturated in the lungs (normal). But with the curve shifted **left** (lower $P_{50}$), hemoglobin holds onto its oxygen more tightly and **releases less of it** at the partial pressures found in peripheral tissues (pO$_2$ ~30–40 mmHg in resting muscle). On the sigmoidal curve, the tissue unloading point ($pO_2$ = 30 mmHg) now falls on a much flatter, higher portion of the curve — meaning less oxygen is given up per unit of $pO_2$ drop.

Fingers notice first because they are the most distal, smallest-diameter circulations. They have the lowest $pO_2$ and the highest demand-to-supply ratio at baseline, making them most vulnerable to any decrease in oxygen delivery. The tingling and stiffness reflect the effects of hypocalcemia (alkalosis increases protein binding of $Ca^{2+}$, reducing free ionized $Ca^{2+}$) and peripheral vasoconstriction, both triggered by the respiratory alkalosis.

---

### Chapter 3 — Problem 3

**2,3-BPG in stored blood: levels fall to near zero after 3 weeks at 4°C.**

**(a) Effect of 2,3-BPG loss on $P_{50}$; curve shift.**

2,3-BPG stabilizes the T-state (deoxyhemoglobin) by binding in the central cavity of the tetramer and forming salt bridges with the beta chains. This T-state stabilization reduces oxygen affinity (raises $P_{50}$). When 2,3-BPG is absent, T-state stabilization is lost, and hemoglobin shifts toward the R-state more easily.

**Loss of 2,3-BPG decreases $P_{50}$** (hemoglobin's oxygen affinity increases) and shifts the oxygen-hemoglobin dissociation curve to the **left**.

**(b) Why the patient shows tissue hypoxia despite adequate hemoglobin levels.**

With near-zero 2,3-BPG, transfused hemoglobin has a very high oxygen affinity — it loads fully in the lungs (normal) but **releases very little oxygen in tissues**. The left-shifted curve means that at the $pO_2$ prevailing in peripheral tissues (~30–40 mmHg), hemoglobin remains highly saturated rather than unloading its cargo. The lab shows a normal hemoglobin concentration, but the functional oxygen delivery per gram of hemoglobin is severely impaired. This is the clinical problem of "left-shifted" banked blood. Red blood cells restore 2,3-BPG levels over 12–24 hours after transfusion, so the problem is transient but can be critical in the immediate post-transfusion period.

**(c) Would removing all 2,3-BPG preserve cooperativity?**

**Yes, cooperativity (and its Hill coefficient) would largely be preserved**, though its magnitude might be somewhat reduced. Cooperativity arises from the allosteric T↔R equilibrium intrinsic to the tetrameric structure — the change in quaternary structure upon oxygen binding communicates between subunits. 2,3-BPG does not create cooperativity; it modulates where on the $pO_2$ axis the T↔R transition occurs by biasing the equilibrium toward T-state. Remove 2,3-BPG, and hemoglobin still undergoes the T-to-R switch as each oxygen binds — the Hill coefficient would remain above 1, reflecting sigmoidal binding. What changes is the $P_{50}$ (it falls, so the sigmoidal curve shifts left), not the fundamental cooperative mechanism.

---

### Chapter 3 — Problem 4

**Fetal hemoglobin HbF ($\alpha_2\gamma_2$), $P_{50}$ ≈ 19 mmHg vs. HbA $P_{50}$ ≈ 26 mmHg.**

**(a) Why oxygen moves from maternal HbA to fetal HbF without active transport.**

At the placenta, both maternal and fetal blood are at similar $pO_2$. At any given oxygen partial pressure, HbF — with its lower $P_{50}$ — is **more saturated** than HbA. As maternal blood delivers oxygen at the placenta (HbA unloads), the freed oxygen diffuses down its partial-pressure gradient into fetal blood, where HbF binds it preferentially (higher affinity). The two different binding curves create a thermodynamic gradient: HbF's greater affinity means it will always have a higher affinity for available oxygen than HbA at the same $pO_2$. No active transport is needed — the simple difference in affinity is sufficient to drive continuous oxygen transfer from mother to fetus.

**(b) Molecular basis: why HbF binds 2,3-BPG more weakly.**

2,3-BPG binds in the central cavity of deoxyhemoglobin, making ionic contacts with positively charged residues on both beta chains: specifically, with His-2 (N-terminus), Lys-82, and His-143 of each beta chain in HbA. Each of these residues contributes a positive charge that complements the multiple negative charges on 2,3-BPG.

In HbF, the **gamma chain** substitutes **serine at position 143** where the beta chain of HbA has **histidine**. Serine is polar but uncharged — it cannot form the ionic contact that His-143 contributes in HbA. Losing two positively charged contacts (one per gamma chain) weakens 2,3-BPG binding substantially. With weaker 2,3-BPG binding, fetal hemoglobin is less T-state-biased, less affected by the allosteric inhibitor, and therefore has a higher oxygen affinity — exactly the right property for a fetus extracting oxygen from maternal blood.

**(c) What happens to $P_{50}$ as HbF is replaced by HbA in infancy; compensation.**

As HbF is replaced by HbA over the first year of life, the $P_{50}$ **rises from ~19 to ~26 mmHg** — hemoglobin's oxygen affinity decreases (curve shifts right). This is actually **beneficial** for oxygen delivery: the higher $P_{50}$ of HbA means more oxygen is released per pass through the tissues at a given $pO_2$.

However, there is a brief period where the transition might theoretically impair oxygen loading in the lungs (lower affinity loads less at $pO_2$ = 100 mmHg — but at this high $pO_2$, even HbA is nearly fully saturated, so this is not a practical problem). The compensatory mechanism is **2,3-BPG**. As red cells mature and accumulate HbA, they contain higher 2,3-BPG levels relative to HbF red cells, fine-tuning the $P_{50}$ to match the needs of neonatal physiology.

---

### Chapter 3 — Problem 5

**Hemoglobin variant with weakened $\alpha_1\beta_2$ interface; Hill coefficient ~1.1, $P_{50}$ = 30 mmHg.**

**(a) Structural explanation for Hill coefficient dropping from ~2.8 to ~1.1.**

A Hill coefficient near 1 implies **little to no cooperativity** — essentially independent, non-communicating binding sites. This follows directly from the weakened $\alpha_1\beta_2$ interface.

In normal HbA, the $\alpha_1\beta_2$ interface is the "sliding" interface — the one that changes its contacts when hemoglobin switches between the T-state and R-state. When oxygen binds to one subunit, the conformational change propagates across this interface to alter the oxygen affinity of adjacent subunits (positive cooperativity). If the interface contacts are weakened, the subunits can no longer efficiently communicate with each other. The quaternary conformational change (T→R) becomes uncoupled from oxygen binding in individual subunits. Each subunit binds oxygen more or less independently, as if it were a monomer — hence a Hill coefficient approaching 1.

**(b) Delivery efficiency with a hyperbolic-like curve between 100 and 30 mmHg.**

A hyperbolic curve is steep at low $pO_2$ and flat at high $pO_2$. At lung $pO_2$ (100 mmHg), the curve is already flat — saturation is very high (~77% for $P_{50}$ = 30 mmHg with a hyperbola: $\theta = 100/(30+100) \approx 0.77$). At tissue $pO_2$ (30 mmHg), $\theta = 30/(30+30) = 0.50$. Delivery = 77% − 50% = ~27% per pass.

Compare to normal HbA which delivers ~30–35% per pass. The delivery is actually **comparable or slightly lower** for this variant, despite the higher $P_{50}$. The key disadvantage is that the variant doesn't load as efficiently in the lungs (only 77% vs. ~97% for normal HbA) because the high $P_{50}$ reduces affinity everywhere. The cooperativity of normal HbA allows it to be nearly fully loaded at 100 mmHg AND unload substantially at 30 mmHg — the sigmoidal curve is optimized for exactly the physiological oxygen range.

**(c) Predicted magnitude of the Bohr effect in this variant.**

The Bohr effect would be **diminished**. Both the Bohr effect and 2,3-BPG regulation work by shifting the T/R equilibrium — they stabilize or destabilize the T-state, which changes $P_{50}$. If the variant's $\alpha_1\beta_2$ interface is compromised, the quaternary T↔R transition is already impaired. The molecule is "stuck" near a single conformational state that does not fully respond to allosteric modulators. Since the Bohr effect acts by altering the pKa values of specific residues (especially $\beta$His-146) that participate in T-state salt bridges, and those salt bridges are part of the same quaternary switch that is disrupted, the Bohr protons will have less effect on oxygen affinity. Clinical implication: during exercise at altitude (low $pO_2$, high $CO_2$, low pH), normal hemoglobin right-shifts to unload more oxygen; this variant cannot respond as effectively, reducing oxygen delivery to working muscle.

---

### Chapter 3 — Problem 6

**Carbon monoxide: Haldane constant $M \approx 240$; environment $pCO$ = 0.15 mmHg, $pO_2$ = 100 mmHg.**

**(a) Calculate [HbCO]/[HbO$_2$] ratio.**

The Haldane equation: $M = \frac{[\text{HbCO}]}{[\text{HbO}_2]} \cdot \frac{pO_2}{pCO}$

Rearranging: $\frac{[\text{HbCO}]}{[\text{HbO}_2]} = M \cdot \frac{pCO}{pO_2} = 240 \times \frac{0.15}{100} = 240 \times 0.0015 = \mathbf{0.36}$

So HbCO:HbO$_2$ ≈ 0.36:1, meaning roughly 26% of hemoglobin sites are occupied by CO and 74% by O$_2$.

**(b) Why 30% HbCO is more dangerous than 30% loss of hemoglobin.**

A patient with only 70% of normal hemoglobin (anemia) has fewer sites, but those sites function normally — they bind O$_2$ in the lungs, deliver it in tissues, and undergo the cooperative T/R transition. Oxygen delivery is reduced proportionally but each remaining hemoglobin molecule works correctly.

With 30% HbCO, CO-bound subunits within the tetramer exert an **allosteric effect** on the remaining O$_2$-bound subunits: CO stabilizes the R-state (high-affinity conformation) of the tetramer. This **left-shifts the oxygen dissociation curve** for the remaining subunits. Those 70% of apparent "functional" sites release less oxygen at tissue $pO_2$ because their affinity is abnormally high. The combination of (1) reduced carrying capacity and (2) impaired unloading makes CO poisoning disproportionately more dangerous than simple anemia of the same degree.

**(c) Mechanism of 100% O$_2$ treatment.**

High-concentration O$_2$ works by **mass action / competitive displacement**. While CO's affinity for hemoglobin is 240-fold higher than O$_2$'s, the binding is still **reversible**. At any moment, HbCO is in equilibrium: $\text{HbCO} \rightleftharpoons \text{Hb} + \text{CO}$.

By breathing 100% O$_2$ at high partial pressure (hyperbaric O$_2$ raises $pO_2$ to ~1,500–2,000 mmHg), the concentration of dissolved O$_2$ is massively increased. Even though each individual O$_2$ molecule competes poorly against CO at a single site, the sheer molar excess of O$_2$ drives the equilibrium by the law of mass action: CO dissociates from one site, and before it can rebind, several hundred O$_2$ molecules are competing for that site. The half-life of HbCO falls from ~4–5 hours on room air to ~60–90 minutes on 100% normobaric O$_2$, and even shorter under hyperbaric conditions. The 240-fold affinity difference is overcome by a >200-fold increase in the competing ligand's partial pressure.

---

### Chapter 3 — Problem 7

**Voxelotor: covalently stabilizes the R-state (oxy conformation) of hemoglobin.**

**(a) Why R-state stabilization prevents HbS polymerization.**

HbS polymerizes specifically in the **T-state** (deoxy conformation). The Val-6 hydrophobic patch that initiates intermolecular contacts is exposed and presented in the correct geometry for fiber formation only in the T-state. In the R-state, the beta chains adopt a different quaternary position that buries or repositions Val-6, abolishing the polymerization-competent surface.

Voxelotor covalently modifies the alpha chain N-terminus to lock hemoglobin in the R conformation. Even when blood $pO_2$ is low (conditions that would normally shift hemoglobin toward T-state), voxelotor-modified molecules remain in R-state. With no T-state available, the polymerization-competent surface is never exposed, and fiber formation is prevented regardless of oxygenation status.

**(b) Why this raises a valid concern about oxygen delivery.**

In normal physiology, the T↔R equilibrium is what allows hemoglobin to unload oxygen at the low $pO_2$ of tissues. The R-state has a **lower $P_{50}$** (higher oxygen affinity) — it grips oxygen more tightly. If voxelotor locks hemoglobin in the R-state, the oxygen dissociation curve shifts **left**: hemoglobin loads well in the lungs but unloads poorly in tissues. The therapeutic goal (prevent T-state polymerization) and the delivery requirement (release O$_2$ in tissues) are in direct opposition. At the tissue $pO_2$ of ~30–40 mmHg, R-state-locked hemoglobin may retain substantially more oxygen than it would if allowed to shift toward T-state — potentially worsening tissue hypoxia even as it prevents sickling. Clinical trials have shown this is a real tradeoff, and the drug's net benefit depends on whether the anti-sickling effect outweighs the delivery impairment.

**(c) Mechanistic basis of reduced Bohr effect; clinical implication at altitude.**

The Bohr effect is mediated by specific residues — most importantly $\beta$His-146 — whose pKa is higher in the T-state than in the R-state. In the T-state, $\beta$His-146 forms a salt bridge with $\beta$Asp-94, which raises its pKa and allows it to take up a proton. When oxygen binds and hemoglobin shifts to R-state, the salt bridge breaks, the pKa falls, and the proton is released — contributing to the Bohr effect. If voxelotor stabilizes the R-state, hemoglobin cannot shift to the T-state even in response to acid. The pKa difference between states is abolished, so the allosteric response to pH is diminished. Less right-shift occurs in response to tissue acidosis and $CO_2$.

Clinical implication at high altitude with exercise: at altitude, $pO_2$ is reduced, and intense exercise generates $CO_2$ and lactic acid that lower tissue pH, normally triggering a Bohr right-shift to enhance O$_2$ delivery. A voxelotor-treated patient's hemoglobin cannot respond to this acid signal. Combined with the already-impaired unloading (R-state locked), oxygen delivery to exercising muscle at altitude would be significantly compromised, potentially causing earlier fatigue or hypoxic symptoms than in a normal individual.

---

## Chapter 4 — Enzymology

### Chapter 4 — Problem 1

**Enzyme: $K_m$ = 0.5 mM, $V_{max}$ = 80 nmol/min.**

**(a) $V_0$ at three substrate concentrations.**

$$V_0 = \frac{V_{max}[\text{S}]}{K_m + [\text{S}]} = \frac{80 \times [\text{S}]}{0.5 + [\text{S}]}$$

- $[\text{S}]$ = **0.5 mM** (= $K_m$): $V_0 = \frac{80 \times 0.5}{0.5 + 0.5} = \frac{40}{1.0} = \mathbf{40}$ nmol/min (exactly $V_{max}/2$, as expected at $[\text{S}] = K_m$)
- $[\text{S}]$ = **5 mM** (10× $K_m$): $V_0 = \frac{80 \times 5}{0.5 + 5} = \frac{400}{5.5} \approx \mathbf{72.7}$ nmol/min (91% of $V_{max}$)
- $[\text{S}]$ = **0.05 mM** (1/10 $K_m$): $V_0 = \frac{80 \times 0.05}{0.5 + 0.05} = \frac{4}{0.55} \approx \mathbf{7.3}$ nmol/min (9% of $V_{max}$)

**(b) Metabolic advantage of $K_m$ ≈ physiological [S].**

When $[\text{S}] \approx K_m$, the enzyme operates on the **steep, nearly linear portion** of the Michaelis-Menten curve. In this range, a small change in substrate concentration produces a large, proportional change in reaction velocity — the enzyme acts as a sensitive sensor. If the cell needs more product (substrate rises slightly), flux through the pathway increases substantially. If substrate falls, flux drops. This gives the cell fine-grained control over pathway throughput in response to small metabolic fluctuations.

**If $K_m$ = 0.001 mM:** the enzyme would already be nearly saturated at physiological [S] (~0.5 mM), operating near $V_{max}$. It would be insensitive to fluctuations in substrate concentration — the pathway would run at near-maximal rate regardless of metabolic state, making regulation impossible.

**If $K_m$ = 50 mM:** physiological [S] (~0.5 mM) would be far below $K_m$. The enzyme would operate in the first-order (linear) region, running at only ~1% of $V_{max}$. Although the enzyme would be sensitive to substrate changes, it would be so inefficient at physiological concentrations that the pathway could never achieve adequate flux.

**(c) Type of inhibition; Lineweaver-Burk change.**

Downstream product decreases $V_0$ by 50% without changing $K_m$. A decrease in $V_{max}$ with no change in $K_m$ is the hallmark of **pure (noncompetitive) inhibition**. The inhibitor binds a site other than the active site (an allosteric or regulatory site), reducing the catalytic efficiency of the enzyme regardless of substrate occupancy. Since $K_m$ reflects substrate binding affinity (not affected), and $V_{max}$ reflects the maximum catalytic output (reduced), this pattern fits noncompetitive inhibition perfectly — consistent with classic feedback inhibition by a product at an allosteric site.

On a Lineweaver-Burk plot: the **y-intercept increases** (from $1/V_{max}$ to $2/V_{max}$) and the **x-intercept is unchanged** (still $-1/K_m$), so the inhibited line is parallel to the uninhibited line, shifted upward. The lines do NOT cross the x-axis at a new point — they intersect the uninhibited line only at the x-axis ($-1/K_m$).

---

### Chapter 4 — Problem 2

**Carbonic anhydrase: $k_{cat} \approx 10^6$ s$^{-1}$; uncatalyzed reaction ~100 s; RBC transit through pulmonary capillary ~0.5 s.**

**(a) Fold-rate enhancement.**

The uncatalyzed reaction has a rate equivalent to completing once per ~100 s. The catalyzed rate is $10^6$ events per second per enzyme molecule. The rate enhancement is:

$$\text{fold enhancement} = k_{cat} \times t_{uncatalyzed} = 10^6 \text{ s}^{-1} \times 100 \text{ s} = 10^8$$

Carbonic anhydrase accelerates the reaction by approximately **$10^8$-fold** (100 million times).

**(b) Could a red blood cell complete the reaction without carbonic anhydrase?**

No. The transit time through a pulmonary capillary is ~0.5 s. The uncatalyzed half-life of CO$_2$ hydration is on the order of many seconds to minutes. In 0.5 s with no catalyst, essentially none of the dissolved CO$_2$ would be converted to bicarbonate. The physiological consequence would be catastrophic: CO$_2$ could not be efficiently converted to HCO$_3^-$ in the blood, impairing CO$_2$ transport from tissues to lungs. Blood would carry far less CO$_2$ (since ~70% of CO$_2$ is transported as bicarbonate), and the lungs could not exhale it rapidly enough. Ventilatory CO$_2$ clearance would fail, leading to hypercapnia and respiratory acidosis.

**(c) Does lowering $E_a$ change the equilibrium position?**

No. An enzyme (or any catalyst) lowers the activation energy $E_a$ for both the forward and reverse reactions equally. It speeds up the rate at which equilibrium is approached but does not change the equilibrium position itself.

The relationship between free energy and equilibrium is: $\Delta G^{\circ'} = -RT\ln K_{eq}$. This equation involves only the thermodynamic properties of the reactants and products (their free-energy difference), not the pathway between them. The enzyme does not change the free energies of CO$_2$/H$_2$O or H$_2$CO$_3$/H$^+$/HCO$_3^-$ — it does not alter the reactant or product stability. Therefore $\Delta G^{\circ'}$ is unchanged, and by the equation above, $K_{eq}$ is unchanged. At equilibrium, the same ratio of products to reactants exists whether the enzyme is present or not. What the enzyme changes is **only how fast** that ratio is reached.

---

### Chapter 4 — Problem 3

**Lineweaver-Burk data.** In a double-reciprocal (Lineweaver-Burk) plot: y-intercept = $1/V_{max}$; x-intercept = $-1/K_m$.

**(a) $K_m$ and $V_{max}$ without inhibitor.**

- y-intercept = 0.020 $\Rightarrow$ $V_{max} = 1/0.020 = \mathbf{50}$ (nmol/min or appropriate units)
- x-intercept = $-0.25$ $\Rightarrow$ $-1/K_m = -0.25 \Rightarrow K_m = 1/0.25 = \mathbf{4}$ mM (assuming [S] in mM)

**(b) Drug X: type of inhibition and apparent $K_m$.**

Drug X data: y-intercept = 0.020 (same as no inhibitor); x-intercept = $-0.10$ (changed).

- y-intercept unchanged $\Rightarrow$ $V_{max}$ is **unchanged**.
- x-intercept changed: $-1/K_{m,app} = -0.10 \Rightarrow K_{m,app} = 1/0.10 = \mathbf{10}$ mM (apparent $K_m$ doubled).

**Interpretation: Drug X is a competitive inhibitor.** Competitive inhibitors compete with substrate for the same (or overlapping) active site. They increase the apparent $K_m$ (the enzyme appears to have lower affinity for substrate because inhibitor and substrate compete) but do not reduce $V_{max}$ — at saturating substrate, the inhibitor can be outcompeted and full velocity is still achieved. The Lineweaver-Burk lines for competitive inhibition intersect the y-axis at the same point (same $V_{max}$) but have a shallower x-intercept (larger $K_{m,app}$).

**(c) Drug Y: type of inhibition; effect of adding more substrate.**

Drug Y data: y-intercept = 0.040 (doubled); x-intercept = $-0.25$ (same as no inhibitor).

- y-intercept doubled $\Rightarrow$ $1/V_{max}$ doubled $\Rightarrow$ $V_{max,app} = 1/0.040 = \mathbf{25}$ (halved).
- x-intercept unchanged $\Rightarrow$ $K_m$ is **unchanged**.

**Interpretation: Drug Y is a pure noncompetitive inhibitor.** Noncompetitive inhibitors bind a site distinct from the active site (an allosteric site) and reduce $V_{max}$ without affecting substrate binding ($K_m$ unchanged).

**Adding more substrate will NOT rescue activity.** In competitive inhibition, adding substrate outcompetes the inhibitor. In noncompetitive inhibition, the inhibitor binds regardless of whether substrate is present — even a fully substrate-occupied enzyme has its catalytic rate reduced. Saturating the active site with substrate does nothing to displace an inhibitor bound at an entirely different location. The inhibitor reduces the effective $k_{cat}$ of every enzyme molecule, so no amount of substrate can restore the original $V_{max}$.

---

### Chapter 4 — Problem 4

**Aspirin irreversibly inhibits COX-1 in anucleate platelets.**

**(a) Effect of irreversible inhibition on $V_{max}$ and $K_m$.**

Irreversible inhibition **decreases $V_{max}$** and **leaves $K_m$ unchanged**.

Mechanistically: when aspirin acetylates the active-site serine of COX-1, that particular enzyme molecule is permanently inactivated — it can never turn over substrate again. The total number of functional enzyme molecules is reduced. Since $V_{max} = k_{cat} \times [\text{E}_{total}]$, fewer functional enzyme molecules means a lower maximum rate. However, $K_m$ reflects the intrinsic affinity of the enzyme for its substrate ($K_m \approx k_{off}/k_{on}$ in the simplest model). Unmodified COX-1 molecules retain their normal active site and normal substrate affinity. The modified (irreversibly inhibited) molecules simply do not catalyze the reaction at all. The remaining uninhibited fraction functions normally — same $K_m$, same $k_{cat}$ per functional molecule — just fewer of them.

**(b) Why antiplatelet effect lasts 7–10 days despite 20-min plasma half-life of aspirin.**

Aspirin forms a **covalent, irreversible** acetyl adduct on COX-1's serine. Once formed, this modification cannot be removed by metabolism — it is permanent for that particular enzyme molecule. Aspirin itself is hydrolyzed to salicylate (inactive) quickly, but that is irrelevant: the damage has already been done. The aspirin molecule is gone, but the acetylated COX-1 molecule remains permanently inactivated.

Critically, platelets are **anucleate** — they cannot synthesize new proteins. They cannot make new COX-1 to replace the inhibited copies. The only way platelet COX-1 activity is restored is when old, aspirin-treated platelets are replaced by new ones from megakaryocytes. Platelet lifespan is 7–10 days, so the antiplatelet effect persists exactly as long as it takes to turn over the entire platelet population.

**(c) Molecular basis of the ibuprofen-aspirin interaction.**

Ibuprofen is a **reversible competitive inhibitor** of COX-1. It binds the active site and blocks it, but the binding is non-covalent and reversible. For aspirin to acetylate its serine target, it must first access and bind the active site. If ibuprofen is already occupying the active site when aspirin is taken, ibuprofen physically **blocks aspirin from reaching the serine**. Aspirin cannot acetylate a serine it cannot reach.

If ibuprofen is taken before aspirin: the active site is occupied by ibuprofen; aspirin cannot bind; the irreversible modification never occurs. When ibuprofen eventually dissociates (it is reversible), COX-1 activity returns normally — with no aspirin modification.

If aspirin is taken first: aspirin acetylates the serine before ibuprofen arrives. The modification is done; subsequent ibuprofen administration has no effect on aspirin's antiplatelet action. This explains why clinical guidance says patients on aspirin for cardiovascular protection should take aspirin first (or avoid ibuprofen), not vice versa.

---

### Chapter 4 — Problem 5

**ATCase: allosteric feedback inhibition by CTP; sigmoidal kinetics; Hill coefficient ~2.**

**(a) Why feedback inhibits the first committed step, not the last.**

If the last enzyme in the pathway were inhibited, the cell would first have to build up intermediates all the way through the pathway before accumulating enough end product to trigger inhibition. During this buildup, all the precursor molecules — amino acids, ATP, reducing equivalents — invested in creating those intermediates are wasted and potentially trapped in dead-end pools. When inhibition finally occurs, the pipeline is full of useless partially synthesized product.

By contrast, inhibiting the **first committed step** shuts off the entire pathway at the entry point. When CTP is plentiful, no more substrate enters the pipeline, and all upstream precursors are conserved for other uses. No intermediates are wasted; the entire downstream machinery idles gracefully. Feedback at the first committed step is the most metabolically economical design.

**(b) Why sigmoidal (switch-like) kinetics suits a feedback-regulated enzyme better than hyperbolic kinetics.**

A hyperbolic enzyme would show a gradual response to rising substrate: even small amounts of substrate produce some product, and the transition from low to high activity is spread over a wide substrate range. For a feedback-regulated enzyme, a gradual response means the pathway is never cleanly "on" or "off" — it always leaks some activity, wastes resources, and never gives a decisive signal.

ATCase's sigmoidal kinetics create a **threshold**: below a certain substrate concentration, activity is very low (the enzyme is largely T-state); above the threshold, activity rises sharply. This makes the pathway behave like a bistable switch — it is essentially off when CTP is high (shifting the T-to-R threshold rightward) and fully on when CTP is depleted. Clean switching maximizes the efficiency of CTP production by running the pathway only when needed and shutting it off sharply when the product is adequate.

**(c) Allosteric inhibition: mechanism of distant-site inhibition.**

This is **allosteric regulation** (specifically, heterotropic allosteric inhibition). CTP binds the **regulatory (allosteric) subunits** of ATCase, which are physically separate from the catalytic subunits. The molecular mechanism involves a **conformational change**: CTP binding to the regulatory site alters the quaternary structure of the ATCase holoenzyme — specifically, it stabilizes the T-state conformation of the catalytic subunits, which has lower affinity for substrates and lower catalytic efficiency.

The communication over 30–40 Å occurs through the protein backbone: the allosteric site and the active site are connected by a continuous network of covalent bonds and non-covalent contacts. A conformational change at the allosteric site propagates like a mechanical signal through the protein — rearranging helix-helix interfaces, changing the positions of active-site loops, and altering the geometry of residues directly involved in catalysis. This is not an informational signal in any metaphorical sense; it is a physical displacement of atoms transmitted through the protein's structural framework.

---

### Chapter 4 — Problem 6

**Organophosphate pesticide poisoning; acetylcholinesterase (AChE) activity = 8% of normal.**

**(a) Class of compound; mechanism; type of inhibition; Michaelis-Menten parameter affected.**

The compound is an **organophosphate** (e.g., parathion, malathion, diazinon). Organophosphates inhibit AChE by **covalently phosphorylating the active-site serine** of the enzyme. The phosphate group forms a stable, essentially irreversible covalent adduct on the serine hydroxyl that normally acts as the nucleophile in acetylcholine hydrolysis. With the serine blocked, the enzyme cannot complete its catalytic cycle.

This is **irreversible inhibition**. Since some fraction of AChE molecules are permanently inactivated, the total number of functional enzyme molecules is reduced, and **$V_{max}$ is decreased** (to ~8% of normal). $K_m$ is unchanged — the remaining functional AChE molecules have the same substrate binding characteristics.

Clinical signs (bradycardia, hypersalivation, lacrimation, miosis, fasciculations, bronchospasm) reflect ACh accumulation at muscarinic (heart, glands, smooth muscle) and nicotinic (NMJ, ganglia) synapses — the classic SLUDGE/DUMBELS toxidrome.

**(b) Atropine vs. pralidoxime (2-PAM): mechanisms and differential effects.**

**Atropine** is a muscarinic acetylcholine receptor antagonist. It competitively blocks ACh at muscarinic receptors (heart, smooth muscle, exocrine glands). This reverses the bradycardia, excessive secretions (salivation, lacrimation), and bronchospasm. However, atropine does not affect nicotinic receptors (NMJ) — it cannot reverse the muscle fasciculations and weakness, which are mediated through nicotinic signaling.

**Pralidoxime (2-PAM)** reactivates the phosphorylated AChE by attacking the phosphoryl-serine bond and cleaving the organophosphate from the enzyme serine, regenerating functional AChE. By restoring AChE activity at all synapses (both muscarinic and nicotinic), 2-PAM reduces ACh concentrations everywhere, addressing both the muscarinic signs (complementing atropine) and the nicotinic muscle signs. Crucially, 2-PAM must be given before **"aging"** (stabilization of the phosphoryl adduct by loss of an alkyl group), after which the bond becomes resistant to oxime attack.

**(c) Fraction of phosphoryl-AChE still reactivatable after 4 hours.**

Using first-order aging kinetics with $t_{1/2} = 1$ hour:

$$f_{\text{reactivatable}} = \left(\frac{1}{2}\right)^{t/t_{1/2}} = \left(\frac{1}{2}\right)^{4/1} = \left(\frac{1}{2}\right)^4 = \frac{1}{16} = \mathbf{6.25\%}$$

Only 6.25% of the phosphoryl-AChE complexes remain reactivatable. 2-PAM at this point would have **minimal clinical benefit** — it can reactivate only a small fraction of inhibited enzyme. With AChE at 8% of normal to begin with, and only 6.25% of that being reactivatable, even complete reactivation of the reactivatable fraction raises activity by less than 0.5 percentage points. The primary treatment at this stage is symptomatic management with atropine (muscarinic blockade) and supportive care, not reliance on 2-PAM for AChE reactivation.

---

### Chapter 4 — Problem 7

**Adenosine deaminase (ADA) transition state analog: $K_d = 3 \times 10^{-12}$ M; adenosine $K_m \approx 3 \times 10^{-5}$ M.**

**(a) Fold-difference in affinity.**

$$\text{fold difference} = \frac{K_m(\text{substrate})}{K_d(\text{analog})} = \frac{3 \times 10^{-5}}{3 \times 10^{-12}} = 10^7$$

The transition state analog binds ADA **$10^7$-fold (10 million times) more tightly** than the substrate adenosine.

**(b) Why the active site binds the transition state analog more tightly.**

The active site of an enzyme is not shaped to complement the substrate's ground-state geometry — it is shaped to complement the **transition state** geometry. This is the structural basis of catalysis: by binding the transition state more tightly than the substrate, the enzyme selectively stabilizes the highest-energy species along the reaction coordinate, which lowers the activation energy and accelerates the reaction.

For ADA, the transition state involves a distorted purine ring with a partial positive charge at C1'. The active site contains precisely positioned charges, hydrogen-bond donors and acceptors, and steric contacts that are geometrically complementary to this distorted geometry. The substrate (adenosine in its ground state) does not fully complement these features — it fits the active site, but not with optimal geometry. The transition state analog mimics the exact shape and charge distribution of the actual transition state, so it engages every complementary feature of the active site simultaneously, explaining the 10$^7$-fold affinity difference.

**(c) Inhibition kinetics: type, reversibility, and competitive considerations.**

The transition state analog binds the **active site** and is structurally similar to the substrate — it would exhibit **competitive inhibition kinetics** in the formal sense (it competes with substrate for the same site; $V_{max}$ unchanged; apparent $K_m$ increased). However, at physiological concentrations, it is **effectively irreversible in practice**.

Here is why: the $K_i$ of the inhibitor is $\approx 3$ pM. The apparent $K_i$ in the presence of substrate is $K_i(1 + [\text{S}]/K_m)$. Even with substrate at its $K_m$ (30 µM), the apparent $K_i$ rises only to ~6 pM. For substrate to outcompete the inhibitor at a given active site, the substrate concentration would need to be thousands of times higher than the inhibitor concentration. In a patient, the drug (at nanomolar or picomolar plasma concentrations) would hold every ADA molecule occupied essentially permanently because the off-rate of the analog is astronomically slow — a 3 pM $K_d$ implies an off-rate ($k_{off} = K_d \times k_{on}$) on the order of hours to days, assuming a diffusion-limited on-rate. Physiologically achievable substrate concentrations cannot compete on this timescale, so the inhibition is effectively irreversible despite being formally competitive.

---

*End of answer key for Chapters 01–04.*
