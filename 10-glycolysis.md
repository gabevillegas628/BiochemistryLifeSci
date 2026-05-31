# Chapter 10: Glycolysis and Gluconeogenesis

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. Heavy alcohol consumption causes fasting hypoglycemia, even worse than fasting alone. The person has no blood alcohol left, their liver glycogen is depleted, and their blood glucose is dropping. Why can't the liver just make more glucose?

2. During intense exercise, your muscles produce lactate even though oxygen is available. Is this a metabolic failure, or does it serve a purpose?

---

## The Big Picture

Glycolysis is the pathway most people learn first in biochemistry, and for good reason: it is ancient (it predates oxygen in Earth's atmosphere), universal (virtually every organism uses some version of it), and foundational (it connects to almost everything else in metabolism). But learning glycolysis as a list of ten reactions to memorize misses the point almost entirely.

Here is the framing that actually makes glycolysis make sense:

Glycolysis is a *controlled demolition*. The cell takes glucose, a 6-carbon sugar, breaks it in half, and extracts the energy and chemical potential embedded in those carbon-carbon bonds, a little at a time, in a form it can use. The products are ATP (from substrate-level phosphorylation), NADH (carrying electrons to the electron transport chain), and pyruvate (a 3-carbon compound that is either oxidized further or used as a biosynthetic precursor, depending on what the cell needs).

Chapter 9 gave you the toolkit: reduction potentials, activated carriers, the phosphate hierarchy, and the six reaction types. Every step of glycolysis falls into one of those types. Recognize the type, and you understand what the step is doing and why.

Gluconeogenesis is glycolysis run mostly in reverse. Not entirely: three steps of glycolysis are so thermodynamically favorable that they cannot be reversed directly. For those three steps, gluconeogenesis uses different enzymes that accomplish the same net chemistry at a thermodynamic cost. Understanding where those detours are, and why they are necessary, tells you almost everything you need to know about how the cell balances glucose production and consumption.

> **Clinical preview:** A patient admitted with severe lactic acidosis may have sepsis, a heart attack, liver failure, or poisoning with certain drugs. What those conditions share is a breakdown of aerobic metabolism, forcing cells to run glycolysis without oxygen and dump the product into the bloodstream. Understanding lactic acidosis requires understanding what glycolysis does when the electron transport chain fails.

---

## The Logic of Glycolysis

### Why Ten Steps?

A student seeing glycolysis for the first time often asks: why does it take ten reactions to break glucose in half? Couldn't you do it in one?

Chemically, yes. Burning glucose in a flame converts it to CO₂ and H₂O in a single step. But the cell cannot do what a flame does. A flame releases all the free energy as heat all at once; cells need to capture that energy *and store it* as chemical potential energy in the form of ATP or NADH. To do that, the process must be broken into small, controlled steps, each releasing a manageable amount of energy, each coupled to a useful output. Ten steps is the price of control.

The other reason for the apparent complexity is that glycolysis does two things simultaneously: it breaks glucose down, and it generates intermediates for biosynthesis. Glucose-6-phosphate feeds the pentose phosphate pathway. Dihydroxyacetone phosphate feeds glycerol-3-phosphate synthesis for lipids. 3-Phosphoglycerate is a precursor for amino acids. The steps that look like overhead are often there to produce these branch points.

This introduces a critical point that runs through all of metabolism: pathways do not exist in isolation. The cell has no concept of "Glycolysis" as a discrete unit. A pathway is a framework we invented to make sense of things. There is no thermodynamic rule that says an intermediate must stay inside the pathway it entered. Intermediates get diverted, shared, and repurposed constantly. Pathways cross-talk and regulate each other until the full picture is a web of hundreds of interconnected reactions we call the **metabolic map**.

### Two Phases: Investment and Payoff

The ten reactions split cleanly into two phases.

**The investment phase (steps 1-5)** spends 2 ATP to phosphorylate glucose and then splits the 6-carbon sugar into two 3-carbon units. Nothing is earned yet; the cell is activating the substrate for later payoff.

**The payoff phase (steps 6-10)** converts each 3-carbon unit into pyruvate, generating 2 NADH and 2 ATP per unit, or 4 NADH + 4 ATP for the two units from one glucose.

**Net per glucose: 2 ATP spent, 4 ATP produced = net 2 ATP. Plus 2 NADH.**

That number looks small, especially compared to the roughly 30-32 ATP that complete glucose oxidation eventually yields. But the bulk of those 30-32 ATP come from NADH and FADH₂ generated later by the TCA cycle and the electron transport chain. Glycolysis is the entry point, not the main event.

### A Note on Directionality

All ten reactions of glycolysis run in the direction glucose → pyruvate under normal cellular conditions. But only three are strongly irreversible: the hexokinase step (step 1), the phosphofructokinase step (step 3), and the pyruvate kinase step (step 10). These are the steps with large negative $\Delta G$ under cellular conditions. The other seven are near-equilibrium and can in principle run in either direction depending on concentration. Gluconeogenesis exploits this: it bypasses the three irreversible steps using different enzymes and runs the remaining seven in reverse.

---

## Part I: The Investment Phase (Steps 1-5)

### Step 1: Glucose is Trapped

$$\text{Glucose} + \text{ATP} \rightarrow \text{Glucose-6-phosphate} + \text{ADP}$$

**Enzyme:** Hexokinase (most tissues) or Glucokinase (liver and pancreatic β cells)

**Reaction type:** Group transfer (phosphoryl transfer)

**$\Delta G^{\circ'}$:** −16.7 kJ/mol

This is the trapping step. Adding a charged phosphate group to glucose does two things: it makes glucose-6-phosphate unable to cross the plasma membrane (glucose transporters won't touch it and the negative charge and polarity of the molecule makes it virtually impossible for it to cross the plasma membrane on its own), trapping it inside the cell, and it activates the molecule for the chemistry that follows. Glucose-6-phosphate is not yet committed to glycolysis specifically; it can still be diverted to the pentose phosphate pathway or glycogen synthesis. Full commitment to glycolysis comes at step 3.

The enzyme matters as much as the reaction. **Hexokinase**, used in most tissues, has a low $K_m$ for glucose (around 0.1 mM), meaning it is nearly saturated at normal blood glucose concentrations of about 5 mM (normal fasting ~90mg/dL). It is also allosterically inhibited by its product, glucose-6-phosphate: G6P binds a regulatory site distinct from the active site and reduces hexokinase activity. This is not a Le Chatelier effect. The reaction is irreversible ($\Delta G^{\circ'} = -16.7$ kJ/mol), so product accumulation cannot push it backward thermodynamically; the braking is a dedicated conformational mechanism. When downstream glycolysis stalls and G6P accumulates, hexokinase is switched off, preventing glucose from being trapped when there is nowhere for it to go.

**Glucokinase**, expressed in the liver and pancreatic β cells, behaves differently. It has a high $K_m$ (around 10 mM or 180mg/dL) and exhibits sigmoidal kinetics with a hill coefficient of ~1.7, and it is not product-inhibited. This means glucokinase activity rises steeply as blood glucose rises above the normal fasting level. The liver uses this as a glucose sensor: at normal blood glucose, glucokinase runs well below its maximal rate; after a meal, when glucose rises, glucokinase revs up and the liver aggressively phosphorylates it to G6P, but mainly for storage, diverting only a small percentage towards glycolysis. In pancreatic β cells, glucokinase activity is the sensor that tells the cell blood glucose has risen, triggering insulin secretion. Mutations in glucokinase cause a form of maturity-onset diabetes (MODY type 2), which is essentially a miscalibrated glucose sensor in the β cell.

### Step 2: Isomerization

$$\text{Glucose-6-phosphate} \rightarrow \text{Fructose-6-phosphate}$$

**Enzyme:** Phosphoglucose isomerase

**Reaction type:** Isomerization

**$\Delta G^{\circ'}$:** +1.7 kJ/mol (near-equilibrium)

The carbonyl moves from C1 (making the molecule an aldose) to C2 (making it a ketose). The proximate reason is that PFK-1 needs to phosphorylate C1, which requires C1 to be a free hydroxyl rather than a carbonyl. But the deeper reason becomes clear two steps later: aldolase requires a carbonyl at C2 to generate an enolate at C3, and it is that enolate that drives the cleavage of the C3-C4 bond. If the carbonyl were still at C1, aldolase would cleave a different bond and produce one 2-carbon fragment and one 4-carbon fragment. Now you have two structurally different products that need two separate downstream pathways. Moving the carbonyl to C2 ensures aldolase cleaves symmetrically at C3-C4, yielding two 3-carbon compounds that both feed into the same payoff phase. One pathway instead of two. The isomerization at step 2 is ultimately doing setup work for step 4, not just step 3.

The reaction is near-equilibrium and runs freely in both directions; the slightly positive $\Delta G^{\circ'}$ is overcome by downstream reactions pulling fructose-6-phosphate forward.

### Step 3: The Committed Step

$$\text{Fructose-6-phosphate} + \text{ATP} \rightarrow \text{Fructose-1,6-bisphosphate} + \text{ADP}$$

**Enzyme:** Phosphofructokinase-1 (PFK-1)

**Reaction type:** Group transfer (phosphoryl transfer)

**$\Delta G^{\circ'}$:** −14.2 kJ/mol (strongly irreversible under cellular conditions)

This is the rate-controlling step of glycolysis and the primary site of regulation. Adding a second phosphate at C1 commits the molecule to glycolysis: fructose-1,6-bisphosphate has nowhere to go except through the next seven steps. The large negative $\Delta G$ makes this step effectively irreversible.

PFK-1 is a homotetramer, each subunit contains an active site which binds F6P and ATP. Each subunit also has allosteric binding sites for ATP/AMP and citrate. Like hemoglobin PFK-1 can exist in an active R state or inactive T state and exhibits cooperativity and sigmoidal kinetics. The allosteric effectors (shown below) act to stabilize either the R or T state allowing for fine regulation of the reaction. PFK-1 is regulated by almost everything that tells the cell whether it needs more or less ATP:

- **ATP** stabilizes the T-state, inhibiting PFK-1. At high ATP concentrations, the allosteric site is occupied and the enzyme is held in its less active conformation. *ATP is therefore both a substrate (active site) and an allosteric inhibitor (regulatory site) of PFK-1.*
- **AMP** stabilizes the R-state by competing with ATP for the same allosteric site, preventing ATP from locking the enzyme into the T-state. AMP has no independent stimulatory effect; the net result looks like activation but the mechanism is de-inhibition. AMP accumulates when ATP is rapidly depleted (via the adenylate kinase reaction: 2 ADP → ATP + AMP), so a rising AMP/ATP ratio is a sensitive signal of energy emergency.
- **Fructose-2,6-bisphosphate (F-2,6-BP)** is the most potent R-state stabilizer and therefore the most potent activator of PFK-1. It is a separate regulatory molecule, not a glycolytic intermediate, synthesized in response to insulin and glucagon. We will return to it in the regulation section.
- **Citrate** stabilizes the T-state, inhibiting PFK-1. Citrate is a TCA cycle intermediate that is exported from the mitochondria via a dedicated inner membrane transporter when the cycle is running faster than needed. High citrate signals that the cell is already well-supplied with fuel and glycolysis should slow.
- **H⁺** inhibits PFK-1 by stabilizing the T-state, which increases sensitivity to ATP inhibition at the allosteric site. Physiologically this serves as a brake: when lactic acidosis begins to develop, falling pH shifts PFK-1 toward the T-state, slowing the enzyme responsible for producing more lactate and providing a degree of self-limitation.

### Step 4: The Split

$$\text{Fructose-1,6-bisphosphate} \rightarrow \text{Dihydroxyacetone phosphate (DHAP)} + \text{Glyceraldehyde-3-phosphate (G3P)}$$

**Enzyme:** Aldolase

**Reaction type:** C-C bond cleavage (retro-aldol condensation)

**$\Delta G^{\circ'}$:** +23.8 kJ/mol (endergonic under standard conditions; spontaneous under cellular conditions)

The 6-carbon bisphosphate is split into two 3-carbon units, each carrying one phosphate. DHAP and G3P (interchangeably referred to as GAP) are constitutional isomers; only G3P feeds directly into the payoff phase.

The standard free energy is positive, meaning this cleavage is thermodynamically unfavorable at standard concentrations. Inside the cell, however, the products are immediately consumed by downstream enzymes, keeping their concentrations extremely low. As established in Chapter 9 (and in the Problem 3 worked example there), product removal pulls near-equilibrium steps forward. Under cellular conditions, aldolase runs in the forward direction.

### Step 5: The Shuttle

$$\text{DHAP} \rightarrow \text{Glyceraldehyde-3-phosphate}$$

**Enzyme:** Triose phosphate isomerase (TPI)

**Reaction type:** Isomerization

**$\Delta G^{\circ'}$:** +7.5 kJ/mol (near-equilibrium)

DHAP cannot directly enter the payoff phase; G3P can. TPI converts DHAP (a ketose) to G3P (an aldose), effectively doubling the yield from the split. The equilibrium at standard conditions actually favors DHAP (roughly 97% DHAP, 3% G3P), but the downstream enzymes keep cellular G3P concentrations very low, pulling the reaction toward G3P. This is the same principle again: product removal keeps a near-equilibrium step running forward.

TPI is sometimes called a "perfect enzyme" because its catalytic rate is limited not by chemistry but by diffusion: with a $\frac{k_{cat}}{K_m}\approx4\times 10^8 \text{M}^{-1}\text{s}^{-1}$ substrate arrives at the active site as fast as random thermal motion allows, and the enzyme converts it immediately. It is hard to imagine improving it.

After step 5, both halves of glucose are in G3P form, and two G3P molecules enter the payoff phase. All yields from here are doubled per glucose.

---

## Part II: The Payoff Phase (Steps 6-10)

The payoff phase is where the energy comes out. Each step is counted twice (once for each G3P from the split).

### Step 6: The Energy-Capturing Step

$$\text{G3P} + \text{NAD}^+ + \text{P}_i \rightarrow \text{1,3-Bisphosphoglycerate} + \text{NADH} + \text{H}^+$$

**Enzyme:** Glyceraldehyde-3-phosphate dehydrogenase (GAPDH)

**Reaction type:** Oxidation-reduction coupled to group transfer

**$\Delta G^{\circ'}$:** −6.3 kJ/mol

This step does two things simultaneously:
1. it oxidizes G3P (NAD⁺ accepts a hydride, producing NADH), and it conserves the energy of that oxidation by forming a thioester intermediate via a conserved cysteine residue in the active site.
2. Inorganic phosphate then attacks the thioester directly in a phosphorolysis reaction, displacing the cysteine and transferring the acyl group to Pᵢ. The energy of oxidation is carried through the thioester and deposited into the acyl-phosphate product; nothing is released as heat.

The result is 1,3-BPG, with a high-energy acyl-phosphate bond at C1. The product, 1,3-bisphosphoglycerate (1,3-BPG), sits well above ATP in the phosphate energy hierarchy (recall from Chapter 9: $\Delta G^{\circ'}$ of hydrolysis = −49.4 kJ/mol, versus −30.5 kJ/mol for ATP). The energy of carbon oxidation has been temporarily stored as a reactive acyl-phosphate, waiting to be cashed in at the next step.

GAPDH requires NAD⁺. This is a critical constraint: if the cell runs out of NAD⁺ because NADH cannot be reoxidized (as in oxygen deprivation), this step stalls and the entire payoff phase stops. The regeneration of NAD⁺ is not a minor housekeeping detail; it is what keeps glycolysis running at all and the cell has mechanisms in place to replenish it even in the absence of Oxygen.

### Step 7: First Substrate-Level Phosphorylation

$$\text{1,3-Bisphosphoglycerate} + \text{ADP} \rightarrow \text{3-Phosphoglycerate} + \text{ATP}$$

**Enzyme:** Phosphoglycerate kinase

**Reaction type:** Group transfer (phosphoryl transfer)

**$\Delta G^{\circ'}$:** −18.9 kJ/mol

The acyl-phosphate on 1,3-BPG transfers to ADP, making ATP. This is substrate-level phosphorylation: ATP is generated directly from a high-energy substrate, no electron transport chain required.

Because 1,3-BPG is above ATP in the phosphate hierarchy, the transfer is favorable. Stack the two half-reactions to see it explicitly:

$$
\begin{array}{rcll}
\text{1,3-BPG} + \cancel{\text{H}_2\text{O}} & \rightarrow & \text{3-PG} + \cancel{\text{P}_i} & \Delta G^{\circ'} = -49.4 \text{ kJ/mol} \\
\text{ADP} + \cancel{\text{P}_i} & \rightarrow & \text{ATP} + \cancel{\text{H}_2\text{O}} & \Delta G^{\circ'} = +30.5 \text{ kJ/mol} \\
\hline
\text{1,3-BPG} + \text{ADP} & \rightarrow & \text{3-PG} + \text{ATP} & \Delta G^{\circ'} = -18.9 \text{ kJ/mol}
\end{array}
$$

Phosphate flows downhill from 1,3-BPG to ADP because 1,3-BPG sits higher in the hierarchy. This step generates 2 ATP per glucose (once for each G3P), fully recovering the 2 ATP invested in steps 1 and 3. Everything beyond this point is profit.

### Step 8: Repositioning

$$\text{3-Phosphoglycerate} \rightarrow \text{2-Phosphoglycerate}$$

**Enzyme:** Phosphoglycerate mutase

**Reaction type:** Isomerization (intramolecular phosphoryl transfer)

**$\Delta G^{\circ'}$:** +0.8 kJ/mol (near-equilibrium)

The phosphate moves from C3 to C2. This is a repositioning step: enolase, which follows immediately, requires the phosphate at C2 to carry out the dehydration that generates PEP.

### Step 9: Creating the High-Energy Product

$$\text{2-Phosphoglycerate} \rightarrow \text{Phosphoenolpyruvate (PEP)} + \text{H}_2\text{O}$$

**Enzyme:** Enolase

**Reaction type:** Elimination (dehydration)

**$\Delta G^{\circ'}$:** +1.7 kJ/mol (near-equilibrium)

Water is removed from 2-phosphoglycerate, generating phosphoenolpyruvate. The reaction converts a modest phosphate ester ($\Delta G^{\circ'}$ of hydrolysis ≈ −17 kJ/mol) into PEP, one of the most reactive phosphate compounds in the cell ($\Delta G^{\circ'}$ of hydrolysis = −61.9 kJ/mol). No external energy input is required; enolase is an energy *transformer*, not an energy source.

Where does the extra reactivity come from? Track the carbon oxidation states across the reaction:

| Carbon | 2-PG | PEP | Change |
|---|---|---|---|
| C1 (carboxylate) | +3 | +3 | none |
| C2 | 0 | +1 | oxidized |
| C3 | −1 | −2 | reduced |

The dehydration is simultaneously an intramolecular redox reaction: C2 is oxidized and C3 is reduced as the double bond forms between them. Electron density shifts from C2 toward C3, and the phosphate at C2 is left on a carbon that has lost electron density, making it far more electrophilic and reactive. This is not a separate electron carrier being reduced, no NAD⁺ or FAD is involved. The electrons simply move within the same molecule, and the result is a phosphate group under much greater chemical tension than before.

As explained in Chapter 9, the full story of PEP's reactivity also involves what happens downstream: once PEP loses its phosphate, the enol spontaneously tautomerizes to the more stable keto form of pyruvate, releasing additional free energy. The −61.9 kJ/mol comes from both the intramolecular electron redistribution that strains the phosphate group and the thermodynamic pull of the enol→keto collapse that follows.

### Step 10: Second Substrate-Level Phosphorylation

$$\text{Phosphoenolpyruvate} + \text{ADP} \rightarrow \text{Pyruvate} + \text{ATP}$$

**Enzyme:** Pyruvate kinase

**Reaction type:** Group transfer (phosphoryl transfer)

**$\Delta G^{\circ'}$:** −31.4 kJ/mol (strongly irreversible)

PEP donates its phosphate to ADP, the enol spontaneously tautomerizes to keto-pyruvate, and 31.4 kJ/mol is released. This generates 2 ATP per glucose (once for each G3P), adding net 2 ATP to the 2 ATP from step 7. Total payoff phase yield: 4 ATP + 2 NADH per glucose.

The large negative $\Delta G$ makes this reaction irreversible in the forward direction. As shown in Chapter 9, ATP cannot phosphorylate pyruvate back to PEP because the reverse reaction has $\Delta G^{\circ'} = +31.4$ kJ/mol; the thermodynamics simply do not permit it. This is why gluconeogenesis needs a completely different two-enzyme workaround to get from pyruvate back to PEP, at a cost of two high-energy phosphate bonds.

Pyruvate kinase is regulated, though less elaborately than PFK-1. ATP and alanine (which signals amino acid surplus, meaning no need to burn more glucose) inhibit it. Fructose-1,6-bisphosphate activates it by feedforward: the product of PFK-1 (step 3) activates pyruvate kinase (step 10), so once the cell commits glucose at step 3, the whole back half of glycolysis runs at full speed.

---

## Part III: The Complete Accounting

| Step | ATP consumed | ATP produced | NADH produced |
|---|---|---|---|
| Step 1 (Hexokinase) | −1 | | |
| Step 3 (PFK-1) | −1 | | |
| Step 6 (GAPDH) ×2 | | | +2 |
| Step 7 (Phosphoglycerate kinase) ×2 | | +2 | |
| Step 10 (Pyruvate kinase) ×2 | | +2 | |
| **Net** | **−2** | **+4** | **+2** |

**Net per glucose: 2 ATP, 2 NADH, 2 pyruvate.**

### All Ten Steps: Reactions and Free Energies

The table below shows each reaction, its standard free energy change, and the estimated actual free energy change under typical cellular conditions. Steps with large negative $\Delta G$ (cellular) are irreversible; steps near zero are near-equilibrium and run in whichever direction concentrations favor.

| Step | Enzyme | Reaction | $\Delta G^{\circ'}$ (kJ/mol) | $\Delta G$ cellular (kJ/mol) |
|---|---|---|---|---|
| 1 | Hexokinase | Glucose + ATP → G6P + ADP | −16.7 | −33.4 |
| 2 | Phosphoglucose isomerase | G6P → F6P | +1.7 | −2.5 |
| 3 | PFK-1 | F6P + ATP → F1,6BP + ADP | −14.2 | −22.2 |
| 4 | Aldolase | F1,6BP → DHAP + G3P | +23.8 | −1.3 |
| 5 | Triose phosphate isomerase | DHAP → G3P | +7.5 | +2.5 |
| 6 | GAPDH | G3P + NAD⁺ + Pᵢ → 1,3-BPG + NADH + H⁺ | −6.3 | −1.1 |
| 7 | Phosphoglycerate kinase | 1,3-BPG + ADP → 3-PG + ATP | −18.9 | +0.1 |
| 8 | Phosphoglycerate mutase | 3-PG → 2-PG | +0.8 | +0.8 |
| 9 | Enolase | 2-PG → PEP + H₂O | +1.7 | −3.3 |
| 10 | Pyruvate kinase | PEP + ADP → Pyruvate + ATP | −31.4 | −16.7 |

*Cellular $\Delta G$ values are estimates under typical erythrocyte/hepatocyte conditions and vary with metabolic state. Steps 1, 3, and 10 are irreversible under all physiological conditions.*

A few things worth noticing in this table. Step 4 (aldolase) has a strongly positive $\Delta G^{\circ'}$ but a near-zero cellular $\Delta G$: it is product removal by downstream enzymes that keeps it running. Steps 6 and 7 are interesting together: step 6 (GAPDH) has a modest $\Delta G^{\circ'}$ but runs close to equilibrium under cellular conditions, while step 7 (phosphoglycerate kinase) has a large negative $\Delta G^{\circ'}$ but also runs close to equilibrium — the two are so tightly coupled that they effectively function as a single unit, with the thermodynamics of step 7 pulling step 6 forward.

### The Balanced Net Reaction

Combining all ten steps and accounting for the fact that the payoff phase runs twice per glucose:

$$\text{Glucose} + 2\text{NAD}^+ + 2\text{ADP} + 2\text{P}_i \rightarrow 2\text{Pyruvate} + 2\text{NADH} + 2\text{H}^+ + 2\text{ATP} + 2\text{H}_2\text{O}$$

$$\Delta G^{\circ'} = -106.1 \text{ kJ/mol} \qquad \Delta G \text{ (cellular)} \approx -97 \text{ kJ/mol}$$

The cellular $\Delta G$ is somewhat less negative than the standard value because the near-equilibrium steps are running close to equilibrium under cellular conditions — their cellular $\Delta G$ values are near zero rather than equal to their $\Delta G^{\circ'}$. The irreversible steps (1, 3, 10) retain large negative cellular $\Delta G$ values and provide the thermodynamic driving force for the whole pathway. Note that some textbooks cite a net $\Delta G^{\circ'}$ around −73 kJ/mol for glycolysis; that value is derived from standard free energies of formation of the overall reactants and products rather than by summing the individual enzymatic steps, and the two methods do not always agree due to differences in reference conditions and accumulated measurement error across sources.

Under aerobic conditions, the 2 NADH will be reoxidized by the electron transport chain, yielding roughly 5 ATP (2 × 2.5 per NADH). The pyruvate will enter the TCA cycle via pyruvate dehydrogenase, generating considerably more. Glycolysis's 2 ATP per glucose looks modest because it is only the first chapter of complete glucose oxidation.

Glycolysis's real value is speed and independence. It runs in the cytoplasm without oxygen, requires no membrane, and can respond to an energy deficit within seconds. No other pathway matches that combination.

---

## Part IV: What Happens to Pyruvate

Pyruvate sits at a metabolic fork. The cell can go one of two directions depending on oxygen availability and the rate of downstream oxidation.

### Aerobic Conditions: Toward the TCA Cycle

Under aerobic conditions (when oxygen is available and abundant), pyruvate enters the mitochondria and is converted to acetyl-CoA by **pyruvate dehydrogenase (PDH)**. PDH is the bridge between glycolysis and the TCA cycle, and it deserves more than a sentence, so we will cover it at the start of Chapter 11. The short version: PDH removes CO₂ from pyruvate, oxidizes the remaining 2-carbon fragment, and attaches it to Coenzyme A, generating acetyl-CoA + NADH + CO₂. Acetyl-CoA then enters the TCA cycle.

### Anaerobic Conditions: Lactate Fermentation

When oxygen is unavailable, or when glycolysis is running faster than the electron transport chain can handle (as in maximally contracting muscle), the cell faces a specific crisis: step 6 of glycolysis requires NAD⁺. If NADH is not being reoxidized by the ETC, NAD⁺ runs out and glycolysis stops (since NAD⁺ is a substrate of GAPDH).

The solution is to dump the electrons from NADH back onto pyruvate just to keep going:

$$\text{Pyruvate} + \text{NADH} + \text{H}^+ \rightarrow \text{Lactate} + \text{NAD}^+$$

**Enzyme:** Lactate dehydrogenase (LDH)

This regenerates NAD⁺, allowing GAPDH to keep running and glycolysis to continue producing ATP. Stack glycolysis and the two LDH reactions together and the intermediates cancel:

$$
\begin{array}{rcll}
\text{Glucose} + \cancel{2\text{NAD}^+} + 2\text{ADP} + 2\text{P}_i & \rightarrow & \cancel{2\text{Pyruvate}} + 2\cancel{\text{NADH}} + 2\cancel{\text{H}^+} + 2\text{ATP} + 2\text{H}_2\text{O} & \text{(glycolysis)} \\
2\cancel{\text{Pyruvate}} + 2\cancel{\text{NADH}} + 2\cancel{\text{H}^+} & \rightarrow & 2\text{Lactate} + 2\cancel{\text{NAD}^+} & \text{(LDH} \times 2\text{)} \\
\hline
\text{Glucose} + 2\text{ADP} + 2\text{P}_i & \rightarrow & 2\text{Lactate} + 2\text{ATP} + 2\text{H}_2\text{O} & \text{(net)}
\end{array}
$$

Pyruvate, NADH, H⁺, and NAD⁺ all cancel. NADH/NAD⁺ become **catalytic**: they cycle between the two pathways without any net change. In effect as long as we have *any* NADH/NAD⁺ we can ignore them completely. The net reaction is proton-neutral, a point we will return to in the lactic acidosis section: lactate production itself generates no H⁺. The cell sacrifices pyruvate as a TCA cycle fuel but keeps the 2 ATP per glucose from substrate-level phosphorylation.

Lactate is not a waste product. The liver can take it up and convert it back to glucose, a recycling circuit called the **Cori cycle** that we will return to once gluconeogenesis is on the table.

---

## Part V: Gluconeogenesis

### Why Not Just Reverse Glycolysis?

Seven of the ten glycolytic reactions are near-equilibrium and will run in reverse under appropriate concentration conditions. Three cannot: hexokinase (step 1), PFK-1 (step 3), and pyruvate kinase (step 10) all have large negative $\Delta G$ values under cellular conditions. Running them in reverse would require large energy inputs the cell cannot practically supply using those same enzymes. Gluconeogenesis bypasses each irreversible step with a dedicated enzyme or pair of enzymes.

### The Four Bypass Reactions

**Bypass 1: Pyruvate → PEP (bypasses pyruvate kinase)**

Getting from pyruvate back to PEP requires two sequential reactions that together cost 2 **ATP equivalents**. ATP equivalent is the standard way to count energy expenditure when different high-energy nucleoside triphosphates are involved: GTP, CTP, and UTP are all interconvertible with ATP via nucleoside diphosphate kinase (GDP + ATP ⇌ GTP + ADP), so they carry the same free energy per phosphate bond and can be counted on the same scale. One ATP equivalent = one high-energy phosphate bond hydrolyzed, regardless of which nucleotide carries it.

**Reaction A:**

$$\text{Pyruvate} + \text{CO}_2 + \text{ATP} \rightarrow \text{Oxaloacetate} + \text{ADP} + \text{P}_i \quad \Delta G^{\circ'}\approx −9.0 kJ/mol$$

*Enzyme:* Pyruvate carboxylase. A ligation reaction (Chapter 9 reaction type 6) that uses ATP and biotin (recall: biotin carries CO₂) to carboxylate pyruvate, generating oxaloacetate (OAA). This runs in the mitochondria.

Pyruvate carboxylase is allosterically activated by acetyl-CoA. When acetyl-CoA accumulates, signaling that the cell has more carbon fuel arriving than it currently needs to burn, the liver is cued to make glucose rather than oxidize more carbon. This is a sensible logic: excess fuel should be stored as glucose, not wasted.

**Reaction B:**

$$\text{Oxaloacetate} + \text{GTP} \rightarrow \text{PEP} + \text{CO}_2 + \text{GDP} \quad \Delta G^{\circ'}\approx +3.0 kJ/mol$$

*Enzyme:* Phosphoenolpyruvate carboxykinase (PEPCK). A group transfer reaction. This reaction uses GTP (thermodynamically equivalent to ATP as noted above) to decarboxylate and phosphorylate OAA, regenerating the 3-carbon PEP. The same CO₂ that was added by pyruvate carboxylase is removed here; the net result is conversion of pyruvate to PEP using 1 ATP + 1 GTP. Two high-energy bonds are spent to climb over the barrier of the −31.4 kJ/mol pyruvate kinase step.

**Bypass 2: Fructose-1,6-bisphosphate → Fructose-6-phosphate (bypasses PFK-1)**

$$\text{Fructose-1,6-bisphosphate} + \text{H}_2\text{O} \rightarrow \text{Fructose-6-phosphate} + \text{P}_i \quad \Delta G^{\circ'}\approx −16.7 kJ/mol$$

*Enzyme:* Fructose-1,6-bisphosphatase (FBPase-1)

A hydrolysis reaction: the phosphate at C1 is removed as free phosphate rather than transferred to ADP. This sidesteps the thermodynamic problem of running PFK-1 in reverse; the energy is lost as heat rather than captured, which is the point. FBPase-1 is not trying to make ATP; it is trying to get the phosphate off without consuming ATP.

FBPase-1 and PFK-1 are reciprocally regulated. AMP activates PFK-1 and inhibits FBPase-1. ATP and citrate inhibit PFK-1 but activate FBPase-1. F-2,6-BP activates PFK-1 and inhibits FBPase-1. You cannot run both enzymes at full speed simultaneously without wasteful futile cycling; the reciprocal regulation prevents it.

**Bypass 3: Glucose-6-phosphate → Glucose (bypasses hexokinase)**

$$\text{Glucose-6-phosphate} + \text{H}_2\text{O} \rightarrow \text{Glucose} + \text{P}_i \quad \Delta G^{\circ'}\approx −13.8 kJ/mol$$

*Enzyme:* Glucose-6-phosphatase

Glucose-6-phosphatase is located on the inner face of the endoplasmic reticulum membrane and is expressed primarily in the liver and kidney (not in muscle or brain). This is why only the liver and kidney can release glucose into the bloodstream: muscle and brain lack this enzyme and cannot export glucose even if they have glucose-6-phosphate.

**Von Gierke disease** (glycogen storage disease type Ia) results from glucose-6-phosphatase deficiency. Without this enzyme, glucose-6-phosphate accumulates, glycogen synthesis goes into overdrive, glycogen cannot be broken down to release free glucose, and fasting hypoglycemia results. The liver becomes massively enlarged from glycogen accumulation. It is a striking illustration of how a single enzyme at an apparently peripheral step controls whether glucose makes it into the bloodstream at all.

### The Complete Gluconeogenic Cost

Starting from 2 pyruvate (the equivalent of 1 glucose worth of carbon from glycolysis):

$$2 \text{ Pyruvate} + 4 \text{ ATP} + 2 \text{ GTP} + 2 \text{ NADH} + 6 \text{ H}_2\text{O} \rightarrow \text{Glucose} + 4 \text{ ADP} + 2 \text{ GDP} + 6 \text{ P}_i + 2 \text{ NAD}^+$$

The 4 ATP breaks down as: 2 ATP for pyruvate carboxylase + 2 ATP for phosphoglycerate kinase running in reverse. The 2 GTP is for PEPCK. The 2 NADH is consumed at GAPDH running in reverse.

Glycolysis nets 2 ATP per glucose. Gluconeogenesis costs 6 high-energy phosphate equivalents (4 ATP + 2 GTP) per glucose synthesized. The difference of 4 equivalents is the thermodynamic price of running the pathway uphill, and it must be paid from somewhere, typically from hepatic fatty acid oxidation during fasting.

### Reciprocal Regulation and Futile Cycling

The cost calculation above makes a critical problem obvious: if glycolysis and gluconeogenesis ran simultaneously at full speed, the cell would be spinning in circles, making glucose and breaking it down at the same time, burning 4 ATP equivalents per cycle and generating nothing but heat. This is called **futile cycling**, and it would be catastrophic. A cell running both pathways flat out would drain its ATP in minutes. You can see this directly by adding the two net reactions and canceling intermediates:

$$
\begin{array}{rcll}
\cancel{\text{Glc}} + \cancel{2\text{NAD}^+} + \cancel{2\text{ADP}} + \cancel{2\text{P}_i} & \rightarrow & \cancel{2\text{Pyr}} + \cancel{2\text{NADH}} + 2\text{H}^+ + \cancel{2\text{ATP}} + \cancel{2\text{H}_2\text{O}} & \text{(glycolysis)} \\
\cancel{2\text{Pyr}} + \overset{2}{\cancel{4\text{ATP}}} + 2\text{GTP} + 2\cancel{\text{NADH}} + \overset{4}{\cancel{6\text{H}_2\text{O}}} & \rightarrow & \cancel{\text{Glc}} + \overset{2}{\cancel{4\text{ADP}}} + 2\text{GDP} + \overset{4}{\cancel{6\text{P}_i}} + 2\cancel{\text{NAD}^+} & \text{(gluconeogenesis)} \\
\hline
2\text{ATP} + \cancel{2\text{GTP}} + 4\text{H}_2\text{O} & \rightarrow & 2\text{ADP} + \cancel{2\text{GDP}} + 4\text{P}_i + 2\text{H}^+ & \text{(net)} \\
\cancel{2\text{GDP}} + 2\text{ATP} & \rightarrow & \cancel{2\text{GTP}} + 2\text{ADP} & \text{(NDPK)} \\
\hline
4\text{ATP} + 4\text{H}_2\text{O} & \rightarrow & 4\text{ADP} + 4\text{P}_i & \text {net}
\end{array}
$$

Glucose, pyruvate, NADH, and NAD⁺ all cancel. What remains is the hydrolysis of 4 high-energy phosphate bonds, 2 ATP and 2 GTP (effectively 4 ATP through the action of nucleoside diphosphate kinase (NDPK)), producing nothing of metabolic value. Pure heat.

The solution is reciprocal regulation: the key opposing enzyme pairs are wired so that when one is active, the other is suppressed. The same signals that activate glycolysis inhibit gluconeogenesis and vice versa, making simultaneous full activity essentially impossible.

The clearest example is the PFK-1 / FBPase-1 pair. Both catalyze reactions at the same metabolic node ($\text{F6P} \leftrightarrow \text{F1,6BP}$), in opposite directions:

| Signal | PFK-1 (glycolysis) | FBPase-1 (gluconeogenesis) |
|---|---|---|
| High AMP | Activated (R-state) | Inhibited |
| High ATP | Inhibited (T-state) | Activated |
| High citrate | Inhibited (T-state) | Activated |
| High F-2,6-BP | Strongly activated | Strongly inhibited |

Every signal pushes both enzymes in the same metabolic direction. AMP signals energy deficit: glycolysis on, gluconeogenesis off. High ATP and citrate signal energy surplus: glycolysis off, gluconeogenesis on. F-2,6-BP is the master switch that glucagon and insulin use to throw the liver between the two states (covered in Part VI).

The hexokinase / glucose-6-phosphatase pair is reciprocally regulated more simply: hexokinase is product-inhibited by G6P, while glucose-6-phosphatase is a constitutively active hydrolase in the ER membrane. The cell avoids the futile cycle here primarily through tissue specificity; muscle lacks glucose-6-phosphatase entirely, so the hexokinase / G6Pase futile cycle is not a problem outside the liver and kidney.

The pyruvate kinase / pyruvate carboxylase-PEPCK pair is regulated partly through allosteric signals (acetyl-CoA activates pyruvate carboxylase; alanine and ATP inhibit pyruvate kinase) and partly through hormonal control of gene expression. Glucagon suppresses pyruvate kinase transcription in the liver during fasting, reducing its abundance so the bypass can run without competition.

The broader point: reciprocal regulation is not just a tidying-up mechanism. It is a thermodynamic necessity. Given that running both pathways simultaneously would cost the cell 4 ATP per futile cycle, evolution selected hard for regulatory mechanisms that make simultaneous full activation essentially impossible.

### The Cori Cycle

Now that gluconeogenesis is established, the Cori cycle mentioned above makes full sense. During high-intensity exercise, oxygen delivery to the muscle is insufficient, meaning that the NADH generated by GAPDH cannot efficiently be oxidized by the mitochndria/electron transport chain. In order to continue Glucose utilization, this NADH but be removed, inthe absence of oxygen the only other mechanism to remove NADH is via lactic acid fermentation. The muscle therfore runs **anaerobic** glycolysis (reducing pyruvate to lactate as shown above) and exports lactate into the bloodstream. The liver takes up that lactate, converts it back to pyruvate via LDH, and runs gluconeogenesis to regenerate glucose, which is released back into the blood for the muscle to use again.

The energetics are deliberately asymmetric. Muscle makes 2 ATP per glucose via anaerobic glycolysis. The liver spends 6 ATP equivalents (4 ATP + 2 GTP) to reverse that and regenerate the glucose. The net cost is 4 ATP equivalents per cycle, subsidized by hepatic fatty acid oxidation. The Cori cycle is not a perpetual motion machine; it is a short-term strategy that lets muscle keep contracting by offloading the metabolic debt to the liver.

The cycle also has a tissue-specificity consequence: because only liver and kidney express glucose-6-phosphatase, only those organs can complete gluconeogenesis and export free glucose. Muscle can export lactate but not glucose. The liver is the obligate intermediary.

---

## Part VI: Regulation and the Fed/Fasted Switch

### The Liver Is a Special Case

Before getting into the molecular details, it is worth stepping back to ask why regulation of this pathway is complicated at all. Most tissues answer that question simply: run glycolysis when you need ATP, slow it down when you don't. The primary signal is energy charge, and the allosteric regulators of PFK-1 (AMP activates, ATP inhibits) handle it automatically. Muscle, brain, and red blood cells are essentially glycolysis-only tissues from a regulatory standpoint.

The liver is different. It is the body's metabolic hub, and it needs to do the opposite of what other tissues do: in the fed state it consumes glucose and stores it, diverting only a small amount towards its own energy needs; in the fasted state it produces glucose and exports it. That means the liver has to switch cleanly between glycolysis and gluconeogenesis depending on nutritional status. The two pathways cannot run simultaneously at full throttle without wasting energy in a futile cycle as we saw above. The liver therefore has a dedicated hormonal switching mechanism layered on top of the basic energy-charge regulation that other tissues use.

The other liver-specific features of this chapter follow the same logic. Glucokinase (instead of hexokinase) lets the liver act as a glucose buffer only when glucose is truly abundant; its high $K_m$ means it does not compete with other tissues for glucose at normal blood concentrations, so glucose is left for the brain and muscle until there is genuinely more than enough. Glucose-6-phosphatase (expressed in liver and kidney, but not muscle) lets those organs release free glucose when they finish gluconeogenesis. Phosphorylation of pyruvate kinase during fasting (covered below) prevents the liver from short-circuiting its own gluconeogenesis at the last step. These are not arbitrary details: each one makes sense once you appreciate that the liver's job description is fundamentally different from every other metabolically active tissue: *The role of the liver is to keep everyone else happy*.

### The Central Regulator: Fructose-2,6-Bisphosphate

The most important regulator of glycolysis versus gluconeogenesis in the liver is not a simple feedback signal from ATP or AMP; it is a dedicated regulatory molecule called **fructose-2,6-bisphosphate (F-2,6-BP)**.

F-2,6-BP is made and destroyed by a **single bifunctional** enzyme with two catalytic domains on the same polypeptide chain: **PFK-2** (a kinase that makes F-2,6-BP from fructose-6-phosphate and ATP) and **FBPase-2** (a phosphatase that destroys F-2,6-BP back to fructose-6-phosphate). Which domain is active depends on whether a regulatory serine residue is phosphorylated:

**Fed state (high insulin, low glucagon):** Insulin signaling activates a protein phosphatase (PP2A) that dephosphorylates the regulatory serine on PFK-2/FBPase-2. With the serine dephosphorylated, the PFK-2 kinase domain is active and the FBPase-2 phosphatase domain is inactive. F-2,6-BP accumulates. F-2,6-BP activates PFK-1 powerfully and inhibits FBPase-1. Net effect: glycolysis on, gluconeogenesis off.

**Fasted state (low insulin, high glucagon):** Glucagon → cAMP → PKA → phosphorylates the regulatory serine on PFK-2/FBPase-2. Now the kinase domain is inactive and the phosphatase domain is active. F-2,6-BP levels fall. Without F-2,6-BP, PFK-1 loses its most potent activator; FBPase-1 runs freely. PKA simultaneously phosphorylates and inhibits the liver isoform of pyruvate kinase (PK-L), preventing PEP from being converted back to pyruvate and short-circuiting gluconeogenesis at its final step. Net effect: glycolysis slowed at two points, gluconeogenesis on. The liver makes glucose and releases it into the bloodstream to maintain blood glucose during the fast.

The elegance of this system is that a single small molecule simultaneously throws opposite switches at both regulatory enzymes, making reciprocal regulation automatic. This is also why Chapter 8's cAMP/PKA cascade has direct metabolic consequences: glucagon's signal through PKA does not just affect gene expression; it rewires the liver's metabolism within minutes by flipping this molecular switch.

### Summary of Key Regulatory Points

| Enzyme | Tissue | Activated by | Inhibited by |
|---|---|---|---|
| Hexokinase | Most tissues | — | Glucose-6-phosphate (product inhibition) |
| Glucokinase | Liver, β cells | Glucose (cooperative kinetics) | — |
| PFK-1 | All tissues | AMP, F-2,6-BP | ATP, citrate, H⁺ |
| Pyruvate kinase (M2 isoform) | Muscle, most tissues | F-1,6-BP (feedforward) | ATP, alanine |
| Pyruvate kinase (L isoform) | Liver | F-1,6-BP (feedforward) | ATP, alanine, PKA phosphorylation (fasting) |
| Pyruvate carboxylase | Liver, kidney | Acetyl-CoA | — |
| FBPase-1 | Liver, kidney | — | AMP, F-2,6-BP |

---

## When It Breaks

### Lactic Acidosis

Lactate is always being produced and cleared. Resting blood lactate is about 1 mM; hard exercise can push it transiently to 10-15 mM without clinical consequence. Lactic acidosis is defined as blood lactate above 4 mM with a pH below 7.35 (normal blood pH is 7.35–7.45). It is a medical emergency.

**Type A lactic acidosis** arises from tissue hypoxia: the electron transport chain cannot run without oxygen, NADH cannot be reoxidized, NAD⁺ runs out, and cells are forced to reduce pyruvate to lactate to keep any glycolysis running at all. Any condition that severely reduces oxygen delivery can cause type A: massive myocardial infarction, cardiogenic shock, severe anemia, carbon monoxide poisoning, or sepsis. The key feature is a failing ETC.

**Type B lactic acidosis** arises without obvious hypoxia and includes drug toxicity (metformin in overdose, nucleoside reverse transcriptase inhibitors used in HIV treatment, and propofol infusion syndrome are notable examples), liver failure (the liver is the primary organ for lactate clearance via gluconeogenesis; if it fails, lactate accumulates), and certain cancers.

Rapidly dividing cells often run high rates of **aerobic glycolysis** (glycolysis that produces lactate even though oxygen is present and available. The term distinguishes this from the normal situation, where pyruvate is oxidized further rather than reduced to lactate). This is the **Warburg effect**: the tumor cell preferentially uses glycolysis rather than oxidative phosphorylation, for reasons related to biosynthetic demand (fast-dividing cells need glycolytic intermediates for anabolic pathways, not just ATP) and signaling. The Warburg effect is the basis of PET scanning in oncology: tumors take up glucose so avidly that an un-metabolizable ¹⁸F-labeled glucose analog lights up the scan.

In every form of lactic acidosis, the common biochemical thread is either excess lactate production (high glycolytic flux with an impaired ETC), impaired lactate clearance (liver failure), or both.

A note on mechanism worth getting right: despite the name, lactate itself does not cause the acidosis. The LDH reaction actually consumes a proton (pyruvate⁻ + NADH + H⁺ → lactate⁻ + NAD⁺), and the net reaction of anaerobic glycolysis through LDH is proton-neutral. The acidosis comes from ATP hydrolysis: ATP⁴⁻ + H₂O → ADP³⁻ + HPO₄²⁻ + H⁺. When ATP is being made and immediately consumed faster than oxidative phosphorylation can regenerate it, each hydrolysis releases a proton. Lactate and H⁺ co-accumulate because they are both products of the same underlying crisis, not because one causes the other. "Lactic acidosis" is really a metabolic acidosis caused by ATP hydrolysis, with lactate as a reliable but mechanistically innocent bystander. The clinical correlation between blood lactate and pH is real and useful; the traditional causal story is not.

### Alcohol, NAD⁺, and Hypoglycemia

Ethanol is metabolized to acetaldehyde by **alcohol dehydrogenase** and then to acetate by **aldehyde dehydrogenase**. Both steps reduce NAD⁺ to NADH:

$$\text{Ethanol} + \text{NAD}^+ \xrightarrow{\text{ADH}} \text{Acetaldehyde} + \text{NADH} + \text{H}^+$$

$$\text{Acetaldehyde} + \text{NAD}^+ \xrightarrow{\text{ALDH}} \text{Acetate} + \text{NADH} + \text{H}^+$$

Heavy alcohol consumption floods the liver with NADH, collapsing the NAD⁺/NADH ratio. The consequences ripple through everything that depends on NAD⁺:

**Gluconeogenesis stalls.** The GAPDH step runs in the gluconeogenic direction and requires NAD⁺. With NAD⁺ depleted, gluconeogenesis cannot run. The liver, the body's main source of blood glucose during fasting, stops making glucose. Blood glucose falls.

**Pyruvate is diverted to lactate.** Excess NADH pushes the lactate dehydrogenase equilibrium toward lactate: NADH + pyruvate → NAD⁺ + lactate. Pyruvate is consumed as a hydrogen sink, removing the primary gluconeogenic substrate.

**Oxaloacetate is diverted to malate.** Excess NADH drives malate dehydrogenase in reverse, converting OAA to malate. OAA is a gluconeogenic precursor; its diversion to malate starves gluconeogenesis of its TCA-cycle-derived substrate.

**The TCA cycle slows.** High NADH product-inhibits multiple TCA cycle dehydrogenases, reducing aerobic ATP production in the liver.

The clinical picture: a patient who drank heavily and did not eat, presenting with hypoglycemia, elevated blood lactate, and possibly lactic acidosis. Treatment is glucose infusion. The mechanism is a pharmacological collapse of the hepatic NAD⁺/NADH ratio, and it is essentially a real-world demonstration of why that ratio, introduced in Chapter 9, governs whole-body metabolic flux.

---

## The MCAT Angle

**Net yield from glycolysis:** 2 ATP, 2 NADH, 2 pyruvate per glucose. The 2 NADH yield roughly 5 ATP via the electron transport chain (2.5 per NADH under aerobic conditions), for a subtotal of 7 ATP from glycolysis and its NADH. Complete glucose oxidation (glycolysis + TCA + ETC) yields 30-32 ATP.

**The three irreversible steps:** Hexokinase (step 1), PFK-1 (step 3), pyruvate kinase (step 10). These are the regulation points and the steps gluconeogenesis must bypass with different enzymes. If a question asks where regulation of glycolysis occurs, these three are the answers; PFK-1 is the primary one.

**Gluconeogenesis and tissue specificity:** Glucose can be synthesized in the liver and kidney. Muscle cannot release free glucose into the blood because it lacks glucose-6-phosphatase. Instead, muscle contributes lactate (Cori cycle) and alanine (glucose-alanine cycle) as gluconeogenic precursors for the liver.

**F-2,6-BP as the master switch:** High F-2,6-BP activates PFK-1 and inhibits FBPase-1 (fed state, glycolysis on). Low F-2,6-BP activates FBPase-1 and reduces PFK-1 activity (fasted state, gluconeogenesis on). Glucagon lowers F-2,6-BP via PKA. Insulin raises it.

**Cori cycle:** Muscle produces lactate under high-intensity conditions; the liver converts it back to glucose at a cost of 6 ATP equivalents per glucose. The net energy cost is covered by liver fatty acid oxidation.

**Warburg effect:** Aerobic glycolysis in cancer cells is clinically important because it underlies PET scanning (¹⁸F-deoxyglucose accumulates in metabolically active tumor cells) and is a target for cancer metabolism research. In an exam context, "aerobic glycolysis" and "the Warburg effect" describe the same phenomenon.

---

## Worked Problems

### Problem 1: ATP Accounting

A red blood cell (RBC) has no mitochondria.

(a) What is the net ATP yield per glucose in an RBC?

(b) RBCs run glycolysis continuously yet maintain low cytoplasmic NADH. How do they regenerate NAD⁺?

(c) Why can't RBCs use the electron transport chain? What would need to be structurally different?

**Solution:**

(a) Substrate-level phosphorylation still works in the absence of mitochondria: steps 7 and 10 each produce 2 ATP per glucose (4 total), with 2 ATP spent in steps 1 and 3. Net: **2 ATP per glucose.** The 2 NADH cannot be fed to an ETC and thus yield no additional ATP.

(b) Lactate dehydrogenase regenerates NAD⁺: pyruvate + NADH → lactate + NAD⁺. RBCs run glycolysis to pyruvate (making 2 ATP), then immediately reduce pyruvate to lactate to regenerate the NAD⁺ needed at step 6. Lactate is exported into the bloodstream and cleared primarily by the liver.

(c) To use the ETC, RBCs would need an inner mitochondrial membrane, ATP synthase, all four ETC complexes, and pyruvate dehydrogenase. The absence of mitochondria in RBCs is a design trade-off: it maximizes the hemoglobin-carrying volume of the cell and eliminates a source of reactive oxygen species adjacent to fragile hemoglobin. The cost is that each RBC's energy metabolism is permanently capped at 2 ATP per glucose.

---

### Problem 2: Gluconeogenic Bypass Energetics

A liver cell needs to synthesize one glucose from two lactate molecules (each lactate is first converted to pyruvate by LDH, producing NADH). The cell now has 2 pyruvate and must reach PEP before it can run the near-equilibrium gluconeogenic steps backward.

(a) How many ATP and GTP equivalents are consumed specifically in converting 2 pyruvate to 2 PEP?

(b) Why can't the cell simply supply 2 ATP to run pyruvate kinase in reverse?

(c) Accounting for all steps from 2 pyruvate to glucose, what is the total energetic cost?

**Solution:**

(a) The bypass from 2 pyruvate to 2 PEP requires:

- Pyruvate carboxylase: 2 Pyruvate + 2 CO₂ + **2 ATP** → 2 OAA + 2 ADP + 2 Pᵢ
- PEPCK: 2 OAA + **2 GTP** → 2 PEP + 2 CO₂ + 2 GDP

Total for this bypass: **2 ATP + 2 GTP** (4 high-energy phosphate bonds) to get 2 PEP.

(b) The pyruvate kinase reaction has $\Delta G^{\circ'} = -31.4$ kJ/mol forward. Running it in reverse requires $+31.4$ kJ/mol per reaction. ATP hydrolysis provides at most 30.5 kJ/mol under standard conditions, which barely covers the standard barrier and cannot account for the additional unfavorable $\Delta G$ under the cellular conditions of gluconeogenesis (high ATP/ADP ratio makes the reverse even harder). No enzyme catalyzes this reverse reaction because the bypass route is thermodynamically more tractable and allows independent regulation. Evolution selected for the detour.

(c) From 2 PEP, gluconeogenesis runs steps 9 through 2 in reverse. The only near-equilibrium steps that require energy input are the phosphoglycerate kinase step (step 7 of glycolysis running backward): 2 3-PG + **2 ATP** → 2 1,3-BPG + 2 ADP. GAPDH running in reverse uses **2 NADH**. The FBPase-1 and glucose-6-phosphatase steps are hydrolysis reactions and cost no ATP.

Grand total per glucose: 2 ATP (carboxylase) + 2 GTP (PEPCK) + 2 ATP (PGK reverse) + 2 NADH (GAPDH reverse)

$$= \textbf{4 ATP} + \textbf{2 GTP} + \textbf{2 NADH}$$

This matches the net equation given in Part VI. The glycolytic path returned 2 ATP per glucose; gluconeogenesis costs 6 high-energy phosphate bonds to reverse it. The difference is the thermodynamic price of running uphill.

---

### Problem 3: Regulation and Clinical Context

A patient with type 2 diabetes is started on metformin. Recall from Chapter 9 that metformin partially inhibits Complex I of the electron transport chain, raising the NADH/NAD⁺ ratio and reducing the ATP/AMP ratio.

(a) What happens to PFK-1 activity in the liver when AMP rises?

(b) What happens to gluconeogenesis in the liver when the NAD⁺/NADH ratio collapses?

(c) Metformin lowers fasting blood glucose. Based on what you know about gluconeogenesis, what is the most likely mechanism?

**Solution:**

(a) AMP activates PFK-1 allosterically. Rising AMP signals an energy deficit, and PFK-1 speeds up, increasing glycolytic flux toward pyruvate.

(b) Gluconeogenesis requires NAD⁺ at the GAPDH step (running in the gluconeogenic direction: 1,3-BPG → G3P needs NADH, but the reaction also regenerates NAD⁺ running forward in glycolysis; in the reverse direction for gluconeogenesis, GAPDH uses NADH to reduce 1,3-BPG to G3P). More directly: the conversion of lactate or alanine to pyruvate (the initial gluconeogenic precursors in the fasted liver) by LDH requires NAD⁺. When NADH is high and NAD⁺ is depleted, the LDH equilibrium is pushed toward lactate production rather than pyruvate production. Gluconeogenic substrate supply is compromised. The pathway stalls.

(c) The primary mechanism is suppression of hepatic gluconeogenesis. In type 2 diabetes, the liver overproduces glucose because insulin resistance blunts the normal suppression of gluconeogenesis by insulin (including the F-2,6-BP pathway), and glucagon signaling goes relatively unopposed. Metformin's elevation of NADH/NAD⁺ impairs gluconeogenic substrate supply, and the rise in AMP activates AMPK (AMP-activated protein kinase), which directly suppresses the expression of gluconeogenic enzymes (PEPCK, glucose-6-phosphatase). Less glucose leaves the liver, and fasting blood glucose falls. Metformin does not stimulate insulin secretion; it works by reducing hepatic glucose output. This is why it does not cause hypoglycemia in most patients: it only reduces the excess production, not physiological glucose release.

---

## Opener Questions Revisited

**1. Heavy alcohol consumption causes fasting hypoglycemia. Why can't the liver just make more glucose?**

The liver maintains blood glucose during fasting primarily through gluconeogenesis, and gluconeogenesis depends on NAD⁺ at multiple steps. Alcohol metabolism (both the alcohol dehydrogenase and aldehyde dehydrogenase reactions) generates NADH and depletes NAD⁺, collapsing the hepatic NAD⁺/NADH ratio. Without NAD⁺, gluconeogenesis stalls. Simultaneously, excess NADH pushes the lactate dehydrogenase equilibrium toward lactate (consuming pyruvate, the primary gluconeogenic substrate) and drives malate dehydrogenase in reverse (consuming OAA, another substrate). The liver loses the ability to synthesize glucose from pyruvate, lactate, or alanine. Once liver glycogen is also depleted from fasting, there is no backup source of blood glucose, and severe hypoglycemia results. The mechanism is entirely traceable to the NAD⁺/NADH ratio.

**2. During intense exercise, your muscles produce lactate even though oxygen is available. Is this a metabolic failure?**

It is not. At high exercise intensities, glycolytic flux exceeds the rate at which the mitochondria can oxidize pyruvate via PDH and the TCA cycle. Pyruvate accumulates faster than it can be consumed, creating a bottleneck. Rather than allowing the NADH buildup to stall GAPDH and halt ATP production, lactate dehydrogenase converts excess pyruvate to lactate, regenerating NAD⁺ and keeping glycolysis running. The lactate is not wasted: it is exported into the bloodstream, taken up by the heart (which oxidizes it directly as fuel), the liver (which converts it back to glucose via the Cori cycle), and less-loaded skeletal muscle fibers. What looks like a metabolic failure is actually a coordinated inter-organ strategy that keeps ATP production going during a demand spike that oxidative phosphorylation cannot immediately meet. The "oxygen is available but lactate still appears" observation is sometimes called a paradox, but it only seems paradoxical if you think the bottleneck is oxygen. It is not; it is the rate of mitochondrial pyruvate oxidation.

---

*Chapter 11 (The TCA Cycle and Oxidative Phosphorylation): We start with pyruvate dehydrogenase, the bridge from glycolysis to the TCA cycle, and then follow the acetyl group through eight steps that complete the oxidation of carbon and transfer all its electrons to the transport chain.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*
