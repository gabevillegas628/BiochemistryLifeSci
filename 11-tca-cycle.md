# Chapter 11: The Pyruvate Dehydrogenase Complex and the TCA Cycle

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. A previously healthy man collapses at home. His family reports he found some pellets in the garage and ate a few thinking they were candy. His blood oxygen, blood glucose, and electrolytes are all normal. His heart is in ventricular fibrillation, and he dies within the hour despite resuscitation. The pellets were sodium fluoroacetate, a rodenticide. Fluoroacetate kills by blocking a single enzyme in the TCA cycle. Which enzyme, and why would that be fatal so fast?

2. A chronically malnourished patient is admitted with confusion, difficulty walking, and abnormal eye movements. Nurses start an IV glucose drip while awaiting workup. Her mental status worsens acutely. A physician orders intramuscular thiamine immediately, and within the hour her confusion clears. Why did the glucose infusion make her worse?

---

## The Big Picture

Chapter 10 ended with pyruvate. Glycolysis split glucose in half, extracted 2 ATP and 2 NADH, and left us with two 3-carbon molecules sitting at a fork: go anaerobic and reduce them to lactate, or go aerobic and oxidize them further. Under aerobic conditions, further oxidation means the TCA cycle, and the route there passes through the pyruvate dehydrogenase complex.

Here is the framing that makes the TCA cycle make sense:

The TCA cycle is primarily an **electron extraction operation**. The carbons in acetyl-CoA still hold a lot of electrons in their carbon-hydrogen bonds, and those electrons represent stored chemical potential energy. The cycle's job is to strip those electrons off, load them onto $\text{NAD}^+$ and FAD, and hand the carriers off to the electron transport chain. The TCA cycle generates very little ATP directly: one GTP (or ATP) per turn via substrate-level phosphorylation. The real yield is 3 NADH and 1 $\text{FADH}_2$ per turn, which the electron transport chain converts to roughly 9 ATP equivalents; 3x2.5ATP + 1x1.5ATP from the NADH and $\text{FADH}_2$ respectively. The cycle is the electron factory; the ETC (Chapter 12) is the ATP factory that runs on what the TCA cycle produces.

The TCA cycle is also a **biosynthetic hub**. Its intermediates are the precursors for amino acid synthesis, heme, nucleotides, and fatty acids. This creates a fundamental tension that runs through regulation: the same cycle that feeds the ETC also feeds the biosynthetic machinery, and the cell must balance extraction versus anabolism depending on what it needs at any given moment.

> **Clinical preview:** Thiamine (vitamin B1) is a cofactor for the pyruvate dehydrogenase complex and for a key TCA cycle enzyme. Deficiency knocks out both entry into the cycle and flux through part of it. Neurons, which run almost entirely on glucose oxidation, are especially vulnerable. The resulting syndrome, Wernicke's encephalopathy, is a classic consequence of chronic malnutrition or heavy alcohol use. Knowing the biochemistry tells you exactly why giving glucose to a thiamine-deficient patient before giving thiamine makes things acutely worse.

---

## From Glycolysis to the Mitochondria: Pyruvate Transport

Glycolysis runs in the cytoplasm. The TCA cycle and the pyruvate dehydrogenase complex run in the mitochondrial matrix. Pyruvate must cross two membranes to get there.

The **outer mitochondrial membrane** contains large non-selective pores (porins; named "voltage-dependent anion channels" in some nomenclatures, but unlike the voltage-gated channels from Ch07 that open and close in response to membrane potential, these are effectively constitutively open under physiological conditions) that allow small molecules including pyruvate to pass freely. It is not a barrier for pyruvate.

The **inner mitochondrial membrane** is a different story. It is essentially impermeable to charged and polar molecules, which is the whole point: the electrochemical gradient across the inner membrane is the engine that drives ATP synthesis. Pyruvate cannot cross it by diffusion.

Entry is handled by the **mitochondrial pyruvate carrier (MPC)**, a dedicated transporter in the inner membrane. The MPC cotransports pyruvate with a proton, using the proton gradient (maintained by the electron transport chain, covered in Ch12) to drive pyruvate import. This is secondary active transport: the cell is spending a small fraction of its proton gradient to import pyruvate, which is a reasonable investment when the alternative is not running the TCA cycle at all.

Once in the matrix, pyruvate meets the pyruvate dehydrogenase complex.

---

## The Pyruvate Dehydrogenase Complex

### Structure and Cofactors

The **pyruvate dehydrogenase complex (PDH complex, or PDC)** is one of the largest enzyme complexes known, with a molecular mass of several million daltons. It is not a single enzyme but an organized assembly of three distinct enzymes:

- **E1: Pyruvate decarboxylase** (pyruvate dehydrogenase in some nomenclatures)
- **E2: Dihydrolipoamide acetyltransferase**
- **E3: Dihydrolipoamide dehydrogenase**

The structure of PDC is roughly spherical with a scaffold of E2 subunits at its core, with E1 and E3 clustered around it. This architecture is not decorative: the long, flexible lipoate arm covalently attached to E2 can swing between the active sites of E1 and E3, passing reaction intermediates without releasing them into solution. The whole complex functions as a single integrated machine.

The complex requires five cofactors — four derived from B vitamins (B1, B2, B3, and B5), plus lipoic acid, which is synthesized endogenously:

| Cofactor | Vitamin precursor | Enzyme | Function |
|---|---|---|---|
| Thiamine pyrophosphate (TPP) | Thiamine (B1) | E1 | Captures and decarboxylates pyruvate |
| Lipoic acid (lipoate) | None (synthesized endogenously) | E2 | Swinging arm that carries and oxidizes the 2-carbon fragment |
| Coenzyme A (CoA) | Pantothenate (B5) | E2 | Accepts the acetyl group to form acetyl-CoA |
| FAD | Riboflavin (B2) | E3 | Reoxidizes reduced lipoate |
| $\text{NAD}^+$ | Niacin (B3) | E3 | Final electron acceptor; becomes NADH |

Five cofactors, three enzymes, one reaction. This is metabolic complexity in service of precise control.

### The Three Phases of the Reaction

The overall reaction is:

$$\text{Pyruvate} + \text{CoA} + \text{NAD}^+ \rightarrow \text{Acetyl-CoA} + \text{CO}_2 + \text{NADH} + \text{H}^+$$

$$\Delta G^{\circ'} = -33.4 \text{ kJ/mol} \qquad (\text{irreversible})$$

It proceeds in three conceptual phases:

**Phase 1: Decarboxylation (E1 + TPP)**

E1 uses TPP as its cofactor. The thiazolium ring of TPP contains a carbon atom with an unusual negative charge that acts as a nucleophile. This carbon attacks the carbonyl of pyruvate, and the bond between pyruvate's carbonyl carbon and its carboxylate group breaks. $\text{CO}_2$ is released. The remaining 2-carbon fragment (a hydroxyethyl group at the oxidation level of an alcohol) stays covalently attached to TPP.

**Phase 2: Oxidation and transfer (E2 + lipoate + CoA)**

Lipoate is covalently attached to a specific lysine residue of E2 via an amide bond, forming a long flexible arm that can reach between the active sites of E1 and E3. E2's lipoate arm swings over to E1 and picks up the 2-carbon fragment. As the fragment transfers, it is oxidized from the alcohol level to the thioester level: the hydroxyethyl group becomes an acetyl group, and lipoate's disulfide is reduced to a dithiol (dihydrolipoic acid is now holding the electrons from this redox reaction). In the active site of E2, Coenzyme A then attacks the acetyl-thioester bond, pulling the acetyl group off lipoate and forming **acetyl-CoA**. This is the product the TCA cycle needs. Lipoate is left in its reduced (dithiol) form.

**Phase 3: Electron handoff (E3 + FAD + $\text{NAD}^+$)**

Reduced lipoate cannot do another round until it is reoxidized. E3 reoxidizes lipoate using FAD, forming $\text{FADH}_2$ and restoring lipoate. E3 then transfers the electrons from $\text{FADH}_2$ to $\text{NAD}^+$, forming **NADH** and regenerating FAD. This is the same logic as GAPDH in glycolysis: the enzyme uses a tightly bound electron carrier (FAD) as an internal relay, then dumps the electrons onto $\text{NAD}^+$ for export. Lipoate is now back in its oxidized (disulfide) form, ready for the next pyruvate. Note that the reduction of $\text{NAD}^+$ by $\text{FADH}_2$ appears strange: return to Chapter 9 and recall that $E^{\circ'}_{\text{NAD}^+/\text{NADH}} = -0.32$ V. The FAD in E3 is tightly protein-bound, which shifts its $E^{\circ'}$ to approximately $-0.29$ V (distinct from the succinate dehydrogenase context of $\approx 0$ V noted in Chapter 9). Using these two values, calculate $\Delta G^{\circ'}$ for the electron transfer from $\text{FADH}_2$ to $\text{NAD}^+$. Is it favorable? Why can the reaction proceed anyway?

Per pyruvate: one $\text{CO}_2$ is released, one acetyl-CoA is produced, and one NADH is made. Per glucose (two pyruvates): 2 $\text{CO}_2$, 2 acetyl-CoA, 2 NADH.

### Regulation of PDH

The PDH complex is regulated by phosphorylation, and the logic of that regulation follows directly from the overall principle: phosphorylation inactivates the complex, dephosphorylation activates it.

Two dedicated regulatory enzymes control the switch:

**PDH kinase (PDK)** phosphorylates a serine on E1, inactivating the complex. It is activated by: high **NADH** (product of the reaction), high **acetyl-CoA** (product of the reaction), and high **ATP** (energy surplus). All three signals say the same thing: we already have more than enough product, slow down.

PDK is inhibited by: high **pyruvate** (substrate: if pyruvate is building up, the complex should run faster, not slower), high **ADP** (energy deficit: need more), and free **CoA** (substrate: available CoA means the reaction hasn't run yet).

**PDH phosphatase (PDP)** dephosphorylates E1, reactivating the complex. It is activated by **insulin** (the fed state signal: glucose is available, run the cycle) and by **$\text{Ca}^{2+}$** (in muscle: the same calcium released from the sarcoplasmic reticulum to trigger contraction also activates PDH, coordinating ATP production with mechanical demand).

The result is a tightly responsive switch. When the cell has plenty of NADH and acetyl-CoA, PDK phosphorylates and silences PDH, stopping it from making more of what is already abundant. When the cell needs acetyl-CoA and energy, pyruvate accumulates, PDK is suppressed, PDP is activated, and PDH runs at full speed.

One more point worth holding: the $\alpha$-ketoglutarate ($\alpha$-KG) dehydrogenase complex (step 4 of the TCA cycle, discussed below) is structurally and mechanistically nearly identical to PDH. It uses the same five cofactors: TPP, lipoate, CoA, FAD, and $\text{NAD}^+$. This is not a coincidence: both complexes perform oxidative decarboxylation of an $\alpha$-keto acid. The shared mechanism means that anything interfering with those cofactors (particularly TPP and lipoate) knocks out both reactions simultaneously, with compounding effects on cell energetics.

---

## The TCA Cycle: Overview

Before walking through the eight steps, it is worth zooming out on acetyl-CoA itself. We arrived here from glucose: glycolysis → pyruvate → PDH → acetyl-CoA. That path gets the introductory attention because glucose is where we started, but acetyl-CoA is where multiple fuel streams converge, and the TCA cycle is indifferent to where the acetyl group came from. Fatty acid β-oxidation produces acetyl-CoA directly, two carbons at a time, which is why fat is a richer fuel per gram than glucose. Ketogenic amino acids (leucine, lysine, and several others partially) are degraded to acetyl-CoA or acetoacetyl-CoA (a 4-carbon acyl-CoA that is either cleaved to two acetyl-CoA or converted to ketone bodies, covered in a later chapter). Ethanol is oxidized to acetate and then activated to acetyl-CoA by acetyl-CoA synthetase in the liver, which is why alcohol has real caloric value. All of these enter the TCA cycle at this same point. When you encounter later that resting muscle runs primarily on fat, or that certain amino acids are "ketogenic," the biochemical translation is: their carbon ends up here, as acetyl-CoA, condensing with OAA.

Acetyl-CoA enters the cycle by condensing with **oxaloacetate (OAA)**, a 4-carbon compound. The 2-carbon acetyl group and the 4-carbon OAA combine to form **citrate**, a 6-carbon tricarboxylic acid. (The cycle's alternate names, "citric acid cycle" and "Krebs cycle," reflect this: citrate is the first product, and Hans Krebs elucidated the cycle in 1937, earning the Nobel Prize in 1953.) The 6-carbon citrate is then progressively oxidized over eight steps, releasing two carbons as $\text{CO}_2$ and regenerating OAA at the end. OAA is not consumed in a net sense: it is a catalyst, cycling through the same positions turn after turn.

**What goes in per turn:** 1 acetyl-CoA (2C), 3 $\text{NAD}^+$, 1 FAD, 1 GDP, 1 $\text{P}_\text{i}$, 2 $\text{H}_2\text{O}$

**What comes out per turn:** 2 $\text{CO}_2$, 3 NADH, 1 $\text{FADH}_2$, 1 GTP, CoA (recycled)

A critical clarification about those two $\text{CO}_2$: they do not come from the acetyl carbons that entered in the same turn. The carbons released as $\text{CO}_2$ in steps 3 and 4 originate from OAA. The two acetyl-CoA carbons are incorporated into OAA by the end of the first turn and are released as $\text{CO}_2$ only in subsequent turns. If you label the carbonyl carbon of acetyl-CoA with $^{14}\text{C}$, it appears in OAA at the end of turn 1 and is released as $^{14}\text{CO}_2$ during turn 2. Complete combustion of the original acetyl carbons requires multiple turns.

All eight reactions occur in the **mitochondrial matrix**, with one important exception: step 6 (succinate dehydrogenase) is embedded in the inner mitochondrial membrane. This is not incidental: succinate dehydrogenase is also Complex II of the electron transport chain as we'll see, making it a shared component of both pathways. The $\text{FADH}_2$ it generates is directly attached to the protein and feeds electrons into the ETC without ever being a free cofactor.

---

## The Eight Reactions of the TCA Cycle

### Step 1: Citrate Synthase

$$\text{Oxaloacetate} + \text{Acetyl-CoA} \rightarrow \text{Citrate} + \text{CoA}$$

**Enzyme:** Citrate synthase

**Reaction type:** Condensation (C-C bond formation)

**$\Delta G^{\circ'}$:** −32.2 kJ/mol (strongly irreversible)

The methyl carbon of acetyl-CoA attacks the carbonyl carbon of OAA in an aldol-like condensation. The thioester bond of acetyl-CoA is hydrolyzed in the process, releasing CoA. That hydrolysis releases additional free energy that drives the condensation forward: the overall reaction is strongly favorable.

Citrate synthase is the gatekeeper of the cycle. Its substrate OAA is present at very low concentrations in the matrix; citrate synthase has high affinity for OAA ($K_m$ in the micromolar range), and its activity is tightly coupled to OAA availability. When OAA is scarce because the cycle is being drawn on for biosynthesis, citrate synthase slows automatically and less acetyl-CoA enters.

The enzyme is inhibited by: citrate (product feedback), NADH, ATP, and succinyl-CoA (signals that the cycle is running faster than the ETC can handle). It is activated by ADP and by high concentrations of its substrates.

### Step 2: Aconitase

$$\text{Citrate} \rightleftharpoons \text{Isocitrate}$$

**Enzyme:** Aconitase (aconitate hydratase)

**Reaction type:** Isomerization (dehydration then rehydration, proceeding via cis-aconitate intermediate)

**$\Delta G^{\circ'}$:** +6.3 kJ/mol (near-equilibrium)

Citrate is a symmetric molecule in appearance but is not metabolized symmetrically. Aconitase removes a water molecule across one C-C bond and adds it back across an adjacent bond, repositioning the hydroxyl group from C3 of citrate to C2 of isocitrate. The purpose is chemical: isocitrate has a hydroxyl group adjacent to a carboxylate, which is the arrangement needed by the next enzyme for oxidative decarboxylation.

Aconitase contains an iron-sulfur cluster ([4Fe-4S]) in its active site. One of the iron atoms directly coordinates the hydroxyl group of the substrate rather than participating in electron transfer, an unusual use of an iron-sulfur center. The cluster is sensitive to reactive oxygen species: superoxide can disrupt the cluster and inactivate the enzyme, linking oxidative stress to TCA cycle suppression.

The reaction is near-equilibrium and runs freely in both directions. Flux toward isocitrate is driven by the strongly favorable step 3 pulling isocitrate forward.

### Step 3: Isocitrate Dehydrogenase

$$\text{Isocitrate} + \text{NAD}^+ \rightarrow \alpha\text{-Ketoglutarate} + \text{CO}_2 + \text{NADH} + \text{H}^+$$

**Enzyme:** Isocitrate dehydrogenase ($\text{NAD}^+$-dependent, mitochondrial isoform)

**Reaction type:** Oxidative decarboxylation

**$\Delta G^{\circ'}$:** −20.9 kJ/mol (irreversible)

Two events happen in one step. First, the hydroxyl group at C2 of isocitrate is oxidized by $\text{NAD}^+$, producing an unstable intermediate ($\beta$-oxalosuccinate) and NADH. Second, the adjacent carboxylate group spontaneously decarboxylates: $\text{CO}_2$ is released and the product, $\alpha$-ketoglutarate, is a 5-carbon $\alpha$-keto acid. This is the first $\text{CO}_2$ produced per turn and the first NADH.

This is a key regulatory step. Isocitrate dehydrogenase is **inhibited** by NADH and ATP (the cycle is already adequately productive) and **activated** by ADP and $\text{Ca}^{2+}$ (energy deficit; demand for ATP production). The enzyme is also activated by its own substrate, isocitrate, at physiological concentrations: the kinetics are sigmoidal, so the enzyme responds steeply to substrate availability.

A clinically important point: the $\text{NAD}^+$-dependent isocitrate dehydrogenase (IDH1 in the cytoplasm, IDH2 in the mitochondria) is frequently mutated in certain cancers, particularly gliomas and acute myeloid leukemia. Mutant IDH does not oxidize isocitrate; instead it reduces $\alpha$-ketoglutarate to a compound called 2-hydroxyglutarate, an oncometabolite that accumulates and dysregulates chromatin methylation. IDH mutation is now a major diagnostic and prognostic marker in glioma classification.

### Step 4: $\alpha$-Ketoglutarate Dehydrogenase Complex

$$\alpha\text{-Ketoglutarate} + \text{NAD}^+ + \text{CoA} \rightarrow \text{Succinyl-CoA} + \text{CO}_2 + \text{NADH} + \text{H}^+$$

**Enzyme:** $\alpha$-Ketoglutarate dehydrogenase complex ($\alpha$-KG dehydrogenase complex)

**Reaction type:** Oxidative decarboxylation

**$\Delta G^{\circ'}$:** −33.5 kJ/mol (strongly irreversible)

This step is the direct mechanistic parallel of PDH. $\alpha$-Ketoglutarate is an $\alpha$-keto acid; the complex oxidatively decarboxylates it using the same three-enzyme architecture (E1-E2-E3) and the same five cofactors (TPP, lipoate, CoA, FAD, $\text{NAD}^+$). $\text{CO}_2$ is released, the 4-carbon fragment is oxidized and transferred to CoA, and NADH is generated. The product, succinyl-CoA, is a high-energy thioester.

This is the second $\text{CO}_2$ per turn and the second NADH. Both $\text{CO}_2$ produced in steps 3 and 4 come from carbons that were originally in OAA.

The complex is inhibited by its products: succinyl-CoA and NADH. It is also inhibited by ATP and activated by $\text{Ca}^{2+}$, following the same logic as isocitrate dehydrogenase.

Because $\alpha$-KG dehydrogenase uses the same cofactors as PDH, it is equally susceptible to thiamine deficiency (loss of TPP) and to arsenite poisoning (which attacks lipoate). When thiamine is depleted, both PDH and $\alpha$-KG dehydrogenase fail simultaneously: pyruvate cannot enter the cycle, and $\alpha$-ketoglutarate backs up inside it. The TCA cycle is interrupted at two points at once.

### Step 5: Succinyl-CoA Synthetase

$$\text{Succinyl-CoA} + \text{GDP} + \text{P}_i \rightarrow \text{Succinate} + \text{GTP} + \text{CoA}$$

**Enzyme:** Succinyl-CoA synthetase (succinate thiokinase)

**Reaction type:** Substrate-level phosphorylation (thioester cleavage coupled to nucleotide phosphorylation)

**$\Delta G^{\circ'}$:** −2.9 kJ/mol (near-equilibrium)

The high-energy thioester bond of succinyl-CoA is cleaved, and the energy is used to phosphorylate GDP to GTP rather than being released as heat. This is substrate-level phosphorylation, the same mechanism as steps 7 and 10 of glycolysis, but using GTP here rather than ATP. GTP is thermodynamically equivalent to ATP; the cell interconverts them freely via nucleoside diphosphate kinase (GTP + ADP ⇌ GDP + ATP), so one GTP per turn is one ATP equivalent per turn.

This is the only step of the TCA cycle that generates a nucleotide triphosphate directly. CoA is released and recycled for use again. The enzyme exists in two tissue-specific isoforms that differ in their β-subunit: the isoform predominating in heart and skeletal muscle produces ATP directly, while the isoform predominating in liver and kidney produces GTP. Since GTP and ATP are freely interconverted by nucleoside diphosphate kinase, the energetic yield is identical; the physiological reason for the difference is not fully settled, but it may relate to the different roles GTP plays in hepatic gluconeogenesis (PEPCK uses GTP) versus the more straightforward ATP demands of contracting muscle.

### Step 6: Succinate Dehydrogenase

$$\text{Succinate} + \text{FAD} \rightarrow \text{Fumarate} + \text{FADH}_2$$

**Enzyme:** Succinate dehydrogenase (SDH)

**Reaction type:** Oxidation

**$\Delta G^{\circ'}$:** ≈ 0 kJ/mol (near-equilibrium)

Succinate is oxidized to fumarate by removal of two hydrogens (one from each of two adjacent carbons), forming a trans double bond. FAD is the electron acceptor, producing $\text{FADH}_2$.

Why FAD rather than $\text{NAD}^+$? The oxidation of succinate to fumarate is not thermodynamically favorable enough to reduce $\text{NAD}^+$ (which has a relatively negative reduction potential of $-0.32$ V). FAD, tightly bound to the enzyme, has a reduction potential of approximately $+0.03$ V, which is high enough to accept electrons from succinate. Using FAD is not a quirk: it is the only thermodynamically viable option for this particular oxidation. As noted in Chapter 9, when you see FAD as the electron acceptor, the substrate is typically a compound where $\text{NAD}^+$-linked oxidation would be endergonic.

Succinate dehydrogenase is physically embedded in the inner mitochondrial membrane and is simultaneously **Complex II of the electron transport chain**. The $\text{FADH}_2$ it produces transfers its electrons directly into the ubiquinone pool of the ETC, bypassing Complex I. This is why $\text{FADH}_2$ from the TCA cycle yields fewer ATP than NADH: its electrons enter the chain downstream of one proton-pumping complex. We will see the mechanistic implications of this in the next chapter.

Succinate dehydrogenase is inhibited by malonate, a structural analog of succinate that binds the active site competitively without being oxidized. Malonate inhibition of SDH was one of the key experiments that established the cyclic nature of the pathway: adding malonate to respiring cells caused succinate to accumulate, demonstrating that succinate was being consumed by the next step.

Certain SDH subunits act as tumor suppressors: proteins whose loss of function, rather than gain of function, promotes cancer. When they are lost, succinate accumulates in the cell. Excess succinate competitively inhibits prolyl hydroxylases, the enzymes that normally mark $\text{HIF-1}\alpha$ (hypoxia-inducible factor, a transcription factor that activates genes for oxygen delivery and glycolysis) for proteasomal degradation, so $\text{HIF-1}\alpha$ builds up even when oxygen is plentiful. The cell responds as if it were starved of oxygen: it promotes new blood vessel growth and shifts toward glycolytic gene expression, creating conditions that favor tumor expansion. Germline SDH mutations predispose to paragangliomas and pheochromocytomas, tumors of the adrenal gland and surrounding neural tissue, which appear at younger ages and in unusual locations because of this misfired hypoxia response.

### Step 7: Fumarase

$$\text{Fumarate} + \text{H}_2\text{O} \rightarrow \text{L-Malate}$$

**Enzyme:** Fumarase (fumarate hydratase)

**Reaction type:** Hydration

**$\Delta G^{\circ'}$:** −3.8 kJ/mol (near-equilibrium)

Water is added across the double bond of fumarate to produce L-malate. The stereochemistry is strict: fumarase adds water across the double bond in an anti (trans) fashion, generating exclusively the L-(S)-isomer of malate. D-malate is not a substrate.

Fumarase is a cytoplasmic enzyme as well as a mitochondrial one; the cytoplasmic version participates in the urea cycle (a liver pathway that converts toxic ammonium to urea for urinary excretion, covered in a later chapter) and in fumarate metabolism in the argininosuccinate lyase reaction (a urea cycle step that releases fumarate as a byproduct). Fumarate hydratase is also a tumor suppressor gene, with loss-of-function mutations associated with hereditary leiomyomatosis and renal cell cancer syndrome.

### Step 8: Malate Dehydrogenase

$$\text{L-Malate} + \text{NAD}^+ \rightarrow \text{Oxaloacetate} + \text{NADH} + \text{H}^+$$

**Enzyme:** Malate dehydrogenase (MDH2, mitochondrial)

**Reaction type:** Oxidation

**$\Delta G^{\circ'}$:** +29.7 kJ/mol (near-equilibrium under cellular conditions)

The hydroxyl group at C2 of malate is oxidized to a carbonyl, regenerating OAA. $\text{NAD}^+$ accepts the electrons, forming NADH. This is the third NADH per turn.

The standard free energy is significantly positive: this reaction is thermodynamically uphill at standard concentrations. Inside the mitochondria, OAA is kept at extremely low concentrations because citrate synthase (step 1) consumes it immediately. Product removal by step 1 pulls step 8 forward despite the unfavorable $\Delta G^{\circ'}$. This is the same product-removal logic seen in glycolysis at aldolase (step 4) and TPI (step 5): near-equilibrium enzymes run in whichever direction concentrations dictate, and downstream enzymes that consume product effectively pull them forward.

The regenerated OAA closes the cycle, ready for another turn of citrate synthase.

---

## The Complete Accounting

### Per Turn of the Cycle (per acetyl-CoA)

| Step | Enzyme | Product(s) |
|---|---|---|
| 1 | Citrate synthase | — |
| 2 | Aconitase | — |
| 3 | Isocitrate dehydrogenase | **NADH**, $\text{CO}_2$ |
| 4 | $\alpha$-KG dehydrogenase complex | **NADH**, $\text{CO}_2$ |
| 5 | Succinyl-CoA synthetase | **GTP** |
| 6 | Succinate dehydrogenase | **$\text{FADH}_2$** |
| 7 | Fumarase | — |
| 8 | Malate dehydrogenase | **NADH** |
| **Net per turn** | | **3 NADH, 1 $\text{FADH}_2$, 1 GTP, 2 $\text{CO}_2$** |

### Per Glucose (Two Turns, Including PDH)

Each glucose yields 2 pyruvate. Each pyruvate passes through PDH and then one full turn of the TCA cycle. Combining everything from the mitochondrion:

| Stage | NADH | $\text{FADH}_2$ | GTP/ATP | $\text{CO}_2$ |
|---|---|---|---|---|
| PDH (×2) | 2 | — | — | 2 |
| TCA cycle (×2 turns) | 6 | 2 | 2 | 4 |
| **Mitochondrial total** | **8** | **2** | **2** | **6** |

Adding glycolysis (2 cytoplasmic NADH, 2 ATP net, substrate-level):

| Stage | NADH | $\text{FADH}_2$ | Direct ATP/GTP | $\text{CO}_2$ |
|---|---|---|---|---|
| Glycolysis | 2 (cytoplasmic) | — | 2 | — |
| Mitochondria (PDH + TCA) | 8 | 2 | 2 | 6 |
| **Grand total per glucose** | **10** | **2** | **4** | **6** |

The 10 NADH and 2 $\text{FADH}_2$ feed the electron transport chain. At approximately 2.5 ATP per NADH and 1.5 ATP per $\text{FADH}_2$:

$$10 \times 2.5 + 2 \times 1.5 + 4 = 25 + 3 + 4 = \textbf{32 ATP per glucose}$$

This is the "roughly 30-32 ATP" figure commonly cited for complete aerobic glucose oxidation. The actual number varies with the coupling efficiency of the ETC, the cost of the pyruvate carrier, and whether cytoplasmic NADH uses the malate-aspartate or glycerol-3-phosphate shuttle to get its electrons into the mitochondria (the two shuttles yield different amounts of ATP per NADH). The important point is the order of magnitude and where the ATP comes from: glycolysis contributes about 6%, the TCA cycle directly (GTP) contributes another 6%, and the ETC running on NADH and $\text{FADH}_2$ contributes the remaining 88%.

### The Balanced Net Reaction

For one turn of the cycle (one acetyl-CoA entering):

$$\text{Acetyl-CoA} + 3\text{NAD}^+ + \text{FAD} + \text{GDP} + \text{P}_i + 2\text{H}_2\text{O} \rightarrow 2\text{CO}_2 + 3\text{NADH} + \text{FADH}_2 + \text{GTP} + \text{CoA} + 3\text{H}^+$$

For the complete oxidation of one pyruvate (PDH + one turn):

$$\text{Pyruvate} + 4\text{NAD}^+ + \text{FAD} + \text{GDP} + \text{P}_i + 2\text{H}_2\text{O} \rightarrow 3\text{CO}_2 + 4\text{NADH} + \text{FADH}_2 + \text{GTP} + \text{CoA} + 4\text{H}^+$$

For complete oxidation of one glucose (glycolysis + 2×PDH + 2×TCA turns), cancelling all shared intermediates (pyruvate, acetyl-CoA, CoA, and water):

$$\text{Glucose} + 10\text{NAD}^+ + 2\text{FAD} + 2\text{ADP} + 2\text{GDP} + 4\text{P}_i + 2\text{H}_2\text{O} \rightarrow 6\text{CO}_2 + 10\text{NADH} + 2\text{FADH}_2 + 2\text{ATP} + 2\text{GTP} + 10\text{H}^+$$

The 6 $\text{CO}_2$ account for all six carbons of glucose: none appear until PDH and the TCA cycle. The 10 NADH and 2 $\text{FADH}_2$ are what the electron transport chain will use to generate the remaining ~28 ATP.

---

## Anaplerosis: Feeding and Drawing from the Cycle

The TCA cycle is not an isolated loop. Its intermediates are constantly diverted for biosynthesis (a process called **cataplerosis**, from the Greek for "falling away"), and they must be constantly replenished (a process called **anaplerosis**, "filling up again").

### What Gets Drawn Off (Cataplerosis)

- **Citrate** is exported from the mitochondria via the citrate carrier when it accumulates above the cycle's needs. Because acetyl-CoA cannot cross the inner mitochondrial membrane directly, citrate serves as its transport form: once in the cytoplasm, ATP citrate lyase cleaves it back to OAA and acetyl-CoA. That cytoplasmic acetyl-CoA is the primary carbon source for fatty acid synthesis. High cytoplasmic citrate also inhibits PFK-1 (Chapter 10), signaling to glycolysis that the mitochondria are well-supplied.

- **$\alpha$-Ketoglutarate** is the carbon skeleton of glutamate (and, by extension, glutamine, proline, arginine, and other amino acids). Transamination of $\alpha$-KG with glutamate produces glutamate and a new $\alpha$-keto acid. The TCA cycle provides the carbon backbone that nitrogen metabolism hangs amino groups onto.

- **Succinyl-CoA** is the precursor for heme synthesis. The first committed step of the porphyrin pathway (synthesis of $\delta$-aminolevulinate, or ALA, the first committed precursor of the porphyrin ring) combines succinyl-CoA with glycine. Without adequate TCA cycle flux, heme production is compromised, which limits hemoglobin assembly and can contribute to sideroblastic anemia in B6-deficient states (B6 is the cofactor for $\delta$-aminolevulinate synthase, but the point is that succinyl-CoA is the upstream carbon source).

- **Oxaloacetate** is a gluconeogenic precursor in the liver (Chapter 10 covered this: OAA → PEP via PEPCK) and can be transaminated to aspartate, which feeds nucleotide synthesis and the urea cycle (covered in a later chapter).

### Replenishment (Anaplerosis)

Draining intermediates without replenishing them would grind the cycle to a halt: if OAA runs low, citrate synthase has nothing to condense with acetyl-CoA, and the whole cycle stops. Anaplerotic reactions prevent this.

The most important anaplerotic reaction in the liver is **pyruvate carboxylase**: pyruvate + $\text{CO}_2$ + ATP → OAA. This is the same reaction introduced in Chapter 10 as the first bypass of gluconeogenesis. From the TCA cycle's perspective, it is an OAA replenishment mechanism. Pyruvate carboxylase is activated by acetyl-CoA: when acetyl-CoA is abundant (more carbon arriving than the cycle can immediately process), acetyl-CoA signals pyruvate carboxylase to make more OAA, expanding the cycle's capacity.

The other major anaplerotic route is amino acid catabolism. Glutamate, glutamine, and most other amino acids can be degraded to TCA cycle intermediates. Glutamate is converted to $\alpha$-KG by glutamate dehydrogenase (releasing $\text{NH}_3$) or by transamination (transfer of the amino group from glutamate to an α-keto acid, producing a new amino acid and regenerating α-KG; covered in detail in the amino acid metabolism chapter). Aspartate is converted to OAA. Isoleucine, valine, methionine, and threonine are converted to succinyl-CoA via propionyl-CoA. These routes explain why protein breakdown supports gluconeogenesis during prolonged fasting: amino acids feed the TCA cycle, which supplies OAA for gluconeogenesis.

Propionyl-CoA (a 3-carbon acyl-CoA produced as the final fragment when fatty acids with an odd number of carbons are oxidized two carbons at a time) is another source of succinyl-CoA, via the propionyl-CoA carboxylase → methylmalonyl-CoA (the carboxylated intermediate) → succinyl-CoA pathway; the final isomerization requires vitamin B12, and B12 deficiency impairs this step, causing methylmalonic acid to accumulate in urine.

---

## Regulation of the TCA Cycle

The cycle is regulated primarily at three steps: citrate synthase (step 1), isocitrate dehydrogenase (step 3), and $\alpha$-KG dehydrogenase (step 4). The regulatory logic is consistent across all three: **products inhibit, substrates and energy deficits activate**.

| Enzyme | Activated by | Inhibited by |
|---|---|---|
| Citrate synthase | OAA (substrate), ADP | Citrate (product), NADH, succinyl-CoA, ATP |
| Isocitrate dehydrogenase | ADP, $\text{Ca}^{2+}$, $\text{NAD}^+$ | NADH, ATP, NADPH |
| $\alpha$-KG dehydrogenase | $\text{Ca}^{2+}$ | NADH, succinyl-CoA (product), ATP |

The overall effect of these controls is that the cycle rate is proportional to the cell's energy deficit. When ATP is high and NADH is high (the cycle has already been running and the ETC is fully loaded), all three regulatory enzymes are inhibited, and the cycle slows. When ADP is high and NADH is low (energy deficit, ETC is running fast and clearing NADH), the inhibition lifts and the cycle accelerates. The cycle is essentially self-regulating through product accumulation and product removal.

**Calcium as a special integrator:** In contracting muscle (and to a lesser extent in other excitable tissues), $\text{Ca}^{2+}$ rises when work is being done. $\text{Ca}^{2+}$ activates PDH phosphatase (activating PDH), isocitrate dehydrogenase, and $\alpha$-KG dehydrogenase simultaneously. All three respond within seconds. This coordinates the ATP supply side (the cycle + ETC) with the demand side (actomyosin ATPase). The same signal that says "contract now" also says "make more ATP now," without waiting for ADP to accumulate. It is a feedforward activation: the anticipatory ramp-up of ATP production triggered by the same signal that increases ATP consumption.

---

## When It Breaks

### Thiamine (Vitamin B1) Deficiency: Wernicke-Korsakoff Syndrome

Thiamine is the dietary precursor of thiamine pyrophosphate (TPP). TPP is the essential cofactor for E1 in both the PDH complex and the $\alpha$-KG dehydrogenase complex. Without adequate thiamine, both enzymes fail.

The consequence is a double block: pyruvate cannot be converted to acetyl-CoA (PDH block), and even what little acetyl-CoA enters the cycle cannot complete the full oxidation past $\alpha$-KG (step 4 block). ATP production from glucose oxidation collapses. The cell is left with only glycolysis, which produces 2 ATP per glucose and forces pyruvate into lactate.

Most cells can cope, at least partially, with this switch to glycolytic metabolism. Neurons cannot. Neurons have extremely high energy demands relative to their mass, essentially no glycogen stores, limited capacity to use fatty acids (the blood-brain barrier is restrictive for long-chain fatty acids), and nearly complete dependence on glucose oxidation. In thiamine deficiency, they are the first to fail.

The clinical syndrome is **Wernicke's encephalopathy**: a triad of confusion, oculomotor dysfunction (most commonly nystagmus, with lateral rectus palsy and, less frequently, ophthalmoplegia), and ataxia (loss of coordination, often presenting as an unsteady gait). Certain deep brain regions, particularly the mammillary bodies and areas of the brainstem, are selectively vulnerable because of their unusually high metabolic rates. Without treatment, the condition can progress to **Korsakoff syndrome**: permanent damage to these regions leaves patients unable to form new memories, and they often fill in the gaps with invented stories without realizing they are doing so, a phenomenon called confabulation.

At-risk populations: chronic heavy alcohol users (alcohol impairs both thiamine absorption and hepatic thiamine storage), patients with prolonged vomiting or inadequate IV nutrition, and anyone receiving glucose infusions while thiamine-depleted.

The clinical trap is giving glucose to a thiamine-deficient patient before giving thiamine. Glycolysis converts that glucose to pyruvate rapidly. Without PDH, pyruvate cannot proceed. It backs up, shifts to lactate (worsening metabolic acidosis), and the demand for the remaining scant TPP rises. Any residual PDH activity is overwhelmed. Symptoms acutely worsen. This is why clinicians treating suspected thiamine deficiency give thiamine before or alongside glucose rather than after.

Treatment is intravenous or intramuscular thiamine. Recovery of the eye movement abnormalities and the confusional state can be dramatic within hours; the memory deficit of Korsakoff syndrome is less reliably reversible.

**Wet beriberi** is the cardiac form. Heart muscle is as oxidatively dependent as neurons, and thiamine deficiency impairs its energy supply in the same way. The heart weakens, fluid accumulates in the tissues and limbs (the edema is what makes it "wet"), and lactic acidosis from impaired oxidative metabolism causes blood vessels to dilate, forcing the already-struggling heart to pump even harder against a larger vascular bed.

**Dry beriberi** is the neurological form, without fluid accumulation (hence "dry"). It presents as numbness, weakness, and eventually motor loss starting in the feet and legs before the hands and arms. The longest nerve fibers in the body fail first because their tips are the farthest from the cell body that sustains them, and when energy metabolism is compromised, the most distal parts of those axons are the first to lose support.

> *The name "beriberi" comes from Sinhalese, a language of Sri Lanka, where "beri" means weakness. The reduplication, saying it twice, is an intensifier: roughly "extreme weakness" or "I cannot, I cannot." The disease was historically epidemic in populations subsisting on polished white rice, because the milling process that makes rice white strips away the thiamine-rich bran. The observation that chickens fed polished rice developed a beriberi-like illness while those fed whole grain rice did not, made by Dutch physician Christiaan Eijkman in the 1890s, was one of the first clues that disease could result from the absence of something essential rather than from an infection. It helped establish the concept of vitamins entirely.*

### Arsenic Poisoning

Arsenite ($\text{As}^{3+}$, the reduced and more toxic form of arsenic) has a high affinity for vicinal dithiols: pairs of sulfhydryl groups close together in space. Lipoate, in its reduced (dithiol) form during the reaction cycle, is exactly such a pair.

Arsenite forms a stable cyclic complex with reduced lipoate, trapping it in the dithiol form and preventing E3 from reoxidizing it. With lipoate stuck, E2 cannot accept new 2-carbon fragments from E1, E1 cannot continue decarboxylation, and the entire complex stalls.

This traps both the PDH complex and the $\alpha$-KG dehydrogenase complex simultaneously, for the same reason as thiamine deficiency: both use lipoate. The resulting clinical picture overlaps with thiamine deficiency: peripheral neuropathy, cardiovascular dysfunction, encephalopathy. The diagnostic distinction often requires measurement of arsenic levels (urine, hair, or nails, which accumulate arsenic over time), though clinically the two can be difficult to separate for obvious reasons.

Treatment includes chelation with BAL (British Anti-Lewisite, dimercaprol), which itself contains two thiols that compete with lipoate for arsenic and drag it into excretion. The development of BAL was specifically motivated by understanding that arsenical war gases (Lewisite) worked by attacking lipoate.

### Fluoroacetate and Lethal Synthesis

Sodium fluoroacetate is used as a rodenticide and has occasionally caused human poisonings. The mechanism is an example of **lethal synthesis**: the cell makes the actual toxic compound from a relatively innocuous precursor.

**Step 1:** Fluoroacetate (2C) is activated by **acetyl-CoA synthetase** in the cytoplasm, forming **fluoroacetyl-CoA**. Acetyl-CoA synthetase is the enzyme that normally activates acetate (a 2-carbon product of various metabolic reactions, including alcohol metabolism) by attaching it to CoA, producing acetyl-CoA: acetate + CoA + ATP → acetyl-CoA + AMP + $\text{PP}_\text{i}$. It treats fluoroacetate as a substrate because fluoroacetate is structurally identical to acetate except for the fluorine substitution at C2.

**Step 2:** Fluoroacetyl-CoA condenses with OAA via citrate synthase, forming **fluorocitrate**. Citrate synthase also cannot distinguish fluoroacetyl-CoA from normal acetyl-CoA.

**Step 3:** Fluorocitrate is a structural analog of citrate and binds aconitase (step 2 of the TCA cycle) at its active site. It is a **mechanism-based inhibitor** (suicide inhibitor): aconitase begins to process it as if it were a normal substrate, but the reaction generates a species that irreversibly blocks the enzyme. Aconitase is inactivated, not just outcompeted.

**Step 4:** With aconitase blocked, the TCA cycle cannot proceed past citrate. Citrate accumulates massively. No further NADH or $\text{FADH}_2$ is generated from the TCA cycle. The ETC slows. Oxidative phosphorylation collapses.

**Step 5:** Without oxidative phosphorylation, cellular ATP falls. The heart, which is almost entirely dependent on oxidative phosphorylation (it has minimal glycogen and cannot sustain ATP production glycolytically under normal conditions), loses its energetic supply. Ventricular fibrillation follows.

The lethality is rapid because the heart cannot tolerate ATP depletion; skeletal muscle and liver can compensate longer with glycolysis, but cardiac muscle cannot. Poisoning by fluoroacetate is essentially a directed sabotage of cardiac bioenergetics via a disguised metabolic substrate.

There is no effective antidote. Treatment is supportive, aimed at controlling arrhythmias and seizures (which also occur because the brain shares the heart's vulnerability to oxidative phosphorylation failure).

---

## The MCAT Angle

**TCA cycle per turn:** 3 NADH, 1 $\text{FADH}_2$, 1 GTP, 2 $\text{CO}_2$. Memorize this. MCAT questions consistently ask for the per-turn yield, the per-glucose yield, or ask which step produces which product.

**Per glucose, total aerobic oxidation:** 10 NADH, 2 $\text{FADH}_2$, 4 direct ATP/GTP, 6 $\text{CO}_2$ (combining glycolysis + PDH + TCA). The ETC converts those to approximately 30-32 ATP.

**Succinate dehydrogenase is Complex II:** It is simultaneously a TCA cycle enzyme and the second complex of the electron transport chain. $\text{FADH}_2$ from SDH enters the ETC via ubiquinone, bypassing Complex I, which is why it yields fewer ATP than NADH (1.5 vs. 2.5 per electron pair).

**Carbon tracking:** In any one turn of the cycle, the two $\text{CO}_2$ released come from OAA, not from the incoming acetyl-CoA. The acetyl-CoA carbons are incorporated into OAA at the end of the turn and are released only in subsequent turns. A labeled acetyl carbon takes at least two turns to appear as $^{14}\text{CO}_2$.

**OAA is catalytic:** It is not consumed in the net sense. The 4-carbon OAA is regenerated at the end of each turn. What is consumed is the 2-carbon acetyl group from acetyl-CoA.

**Cofactor targets in deficiency:** Thiamine (B1) deficiency knocks out PDH and $\alpha$-KG dehydrogenase. Riboflavin (B2) would affect $\text{FADH}_2$ production. Niacin (B3) would affect $\text{NAD}^+$ availability. Pantothenate (B5) deficiency would impair CoA synthesis. For MCAT purposes, thiamine deficiency is by far the most clinically important, connecting to Wernicke-Korsakoff syndrome and wet/dry beriberi.

**PDH regulation shorthand:** PDH is inactivated when NADH, acetyl-CoA, and ATP are high (products inhibit). It is activated when pyruvate, ADP, and CoA are high (substrates/need signals activate). Insulin and $\text{Ca}^{2+}$ activate by stimulating the phosphatase that removes the inhibitory phosphate from E1.

**Anaplerosis on MCAT:** The most important anaplerotic reaction is pyruvate carboxylase (pyruvate → OAA), activated by acetyl-CoA. Questions about why the TCA cycle needs to be "fed" from outside, or why propionate or amino acid carbon enters the cycle, are testing anaplerosis.

---

## Worked Problems

### Problem 1: Counting Cofactors and Carbon

A cell metabolizes one molecule of glucose completely to $\text{CO}_2$ and $\text{H}_2\text{O}$ under aerobic conditions. Answer the following:

(a) How many $\text{CO}_2$ molecules are released, and at which steps?

(b) How many molecules of $\text{NAD}^+$ are reduced to NADH, and at which steps?

(c) How many molecules of FAD are reduced to $\text{FADH}_2$, and at which steps?

**Solution:**

(a) **6 $\text{CO}_2$ per glucose, released at:**
- Pyruvate dehydrogenase (×2): 2 $\text{CO}_2$ total, one per pyruvate
- Isocitrate dehydrogenase (step 3, ×2 turns): 2 $\text{CO}_2$ total
- $\alpha$-KG dehydrogenase (step 4, ×2 turns): 2 $\text{CO}_2$ total

Glycolysis releases no $\text{CO}_2$: it rearranges and cleaves carbons but does not oxidize them to $\text{CO}_2$. All 6 $\text{CO}_2$ from one glucose come from the pyruvate dehydrogenase complex and the TCA cycle.

(b) **10 NADH per glucose:**
- Glycolysis step 6 (GAPDH) ×2: 2 NADH (cytoplasmic)
- PDH ×2: 2 NADH (mitochondrial)
- TCA step 3 (isocitrate dehydrogenase) ×2: 2 NADH
- TCA step 4 ($\alpha$-KG dehydrogenase) ×2: 2 NADH
- TCA step 8 (malate dehydrogenase) ×2: 2 NADH

(c) **2 $\text{FADH}_2$ per glucose:**
- TCA step 6 (succinate dehydrogenase) ×2: 2 $\text{FADH}_2$

All $\text{FADH}_2$ comes from succinate dehydrogenase. The PDH complex and $\alpha$-KG dehydrogenase complex use FAD internally in their E3 subunits, but it is a tightly bound, catalytic cofactor that transfers electrons to $\text{NAD}^+$ within the complex. No net $\text{FADH}_2$ leaves those complexes.

---

### Problem 2: PDH Regulation and the Fasted Liver

A person has been fasting for 24 hours. Plasma glucose is low, plasma fatty acids are high, and the liver has shifted to fatty acid oxidation as its primary fuel. $\beta$-oxidation of fatty acids generates large amounts of acetyl-CoA and NADH in the mitochondria.

(a) What happens to PDH activity in the fasted liver, and what signal mediates it?

(b) OAA is both a TCA cycle intermediate and a gluconeogenic precursor. If the liver needs to run gluconeogenesis, OAA is diverted to the cytoplasm. What effect does this have on TCA cycle flux, and what compensates?

(c) Acetyl-CoA cannot be converted to net glucose in mammals. Explain why, using the stoichiometry of the TCA cycle.

**Solution:**

(a) PDH is inactivated in the fasted liver. $\beta$-oxidation produces large amounts of NADH and acetyl-CoA. Both activate PDH kinase (PDK), which phosphorylates and inactivates E1. This makes metabolic sense: there is no point in converting pyruvate to acetyl-CoA when acetyl-CoA is already abundant. Pyruvate is preserved for gluconeogenesis (via pyruvate carboxylase) rather than being oxidized to acetyl-CoA that will just exceed what the TCA cycle can handle.

(b) OAA diversion to gluconeogenesis depletes the mitochondrial OAA pool. With less OAA, citrate synthase slows (its substrate is limited), and the cycle turns more slowly. The compensating mechanism is anaplerosis: pyruvate carboxylase (activated by the high acetyl-CoA from $\beta$-oxidation) converts pyruvate to OAA, replenishing what was drained. This is the critical cross-link: in the fasted liver, $\beta$-oxidation generates acetyl-CoA, which activates pyruvate carboxylase, which makes OAA. Some OAA condenses with acetyl-CoA via citrate synthase to keep the cycle turning; the rest is diverted to PEPCK for gluconeogenesis. Acetyl-CoA simultaneously drives the anaplerosis that supplies the cycle and gluconeogenesis.

(c) Acetyl-CoA contributes 2 carbons per turn of the TCA cycle. Both carbons are released as $\text{CO}_2$ over the course of subsequent turns. There is no net carbon left that could be exported from the cycle as a gluconeogenic precursor. The math is explicit: one turn of the TCA cycle beginning with OAA (4C) + acetyl-CoA (2C) produces one OAA (4C) at the end. The 2 $\text{CO}_2$ released come from OAA carbons; those OAA carbons are replaced by the acetyl-CoA carbons. Net result: the OAA pool is maintained, but no new carbon escapes. To make glucose via gluconeogenesis, the liver needs a 3-carbon or 4-carbon compound to emerge from the cycle, which cannot happen when the only input is acetyl-CoA. This is why fat cannot be converted to net glucose in mammals: fatty acid $\beta$-oxidation produces only acetyl-CoA, which cycles without net carbon contribution to gluconeogenesis. (Plants and bacteria can use the glyoxylate cycle, a modified TCA cycle with two extra enzymes (isocitrate lyase and malate synthase) that allow the net conversion of acetyl-CoA carbon to OAA; mammals lack those enzymes.)

---

### Problem 3: Clinical Reasoning — TCA Cycle Disruption

A patient presents to the emergency department with seizures, a lactic acidosis, and elevated plasma pyruvate. Brain MRI shows bilateral lesions in the basal ganglia and brainstem. The patient's mother reports that these episodes have been occurring since infancy, triggered by febrile illness or high-carbohydrate meals.

(a) The combination of elevated pyruvate, elevated lactate, and normal or elevated lactate-to-pyruvate ratio (normal is <20) is a classic biochemical signature. What does it suggest about the site of the metabolic block?

(b) The patient's lactate-to-pyruvate ratio is 22 (mildly elevated). Does this finding point toward a PDH defect or toward a defect in the electron transport chain?

(c) These episodes worsen with high-carbohydrate intake but improve on a high-fat (ketogenic) diet. Explain why, using your understanding of PDH and TCA cycle fuel inputs.

(d) If this were a deficiency of $\alpha$-KG dehydrogenase rather than PDH, would the lactate-to-pyruvate ratio be expected to rise? Why or why not?

**Solution:**

(a) Elevated pyruvate with elevated lactate suggests a block at the point where pyruvate is consumed. The main pyruvate-consuming pathway under aerobic conditions is PDH. A pyruvate block forces pyruvate into lactate via LDH, explaining both elevations. The differential includes PDH deficiency, pyruvate carboxylase deficiency, and electron transport chain defects (which raise NADH, shift LDH equilibrium toward lactate, and cause secondary pyruvate accumulation). The bilateral symmetric brain lesions and episodic worsening in response to carbohydrate loads are highly characteristic of Leigh syndrome, a mitochondrial disease spectrum that includes PDH deficiency and Complex I/IV defects.

(b) A lactate-to-pyruvate ratio of 22 (mildly elevated above the normal threshold of 20) points toward PDH deficiency rather than an electron transport chain defect.

In ETC defects, NADH cannot be reoxidized. The excess NADH drives the malate dehydrogenase and LDH equilibria strongly toward OAA reduction and pyruvate reduction respectively, creating a very high lactate-to-pyruvate ratio (often >25, sometimes >40). In PDH deficiency, the NADH/$\text{NAD}^+$ ratio is not primarily elevated; the problem is that pyruvate cannot enter the TCA cycle. Pyruvate accumulates and is secondarily shunted to lactate, but the ratio rises only modestly because $\text{NAD}^+$ is not depleted. The mild elevation here is more consistent with PDH deficiency (or pyruvate carboxylase deficiency). In an ETC defect, you would also typically see elevated lactate without necessarily elevated pyruvate and the ratio would be higher.

(c) High carbohydrate intake floods the cell with glucose, which glycolysis converts to pyruvate. A PDH-deficient patient cannot convert that pyruvate to acetyl-CoA; it backs up, overwhelms LDH, produces lactic acidosis, and starves the TCA cycle of substrate. Seizures are triggered because neurons cannot maintain their ATP levels.

A ketogenic diet bypasses PDH entirely. Fatty acids are $\beta$-oxidized to acetyl-CoA without requiring PDH (PDH is only needed to decarboxylate pyruvate; acetyl-CoA from fat oxidation requires no decarboxylation step). Ketone bodies (acetoacetate and $\beta$-hydroxybutyrate, small water-soluble molecules produced by hepatic fatty acid oxidation when glucose is unavailable, covered in a later chapter) are produced in the liver and cross the blood-brain barrier, where they are converted directly to acetyl-CoA by two steps that also bypass PDH. The TCA cycle can be supplied with acetyl-CoA from ketones even when PDH is non-functional. Symptoms improve because the brain's metabolic demands can now be met without going through the defective PDH step.

(d) An $\alpha$-KG dehydrogenase deficiency would not primarily raise the lactate-to-pyruvate ratio. The block is at step 4 of the TCA cycle ($\alpha$-KG → succinyl-CoA), inside the cycle and downstream of PDH. Pyruvate can still enter the cycle normally and become acetyl-CoA; it is $\alpha$-ketoglutarate that backs up, not pyruvate. Without a pyruvate accumulation, LDH is not driven toward lactate, and the lactate/pyruvate ratio is not expected to rise. Instead, plasma $\alpha$-ketoglutarate and its transamination product glutamate would be elevated. The clinical pattern would also differ: $\alpha$-KG dehydrogenase deficiency causes a distinct syndrome with elevated $\alpha$-ketoglutaric acid in urine (2-oxoglutaric aciduria) and progressive neurodegeneration, without the prominent lactic acidosis pattern of PDH deficiency.

---

## Opener Questions Revisited

**1. A man collapses after eating sodium fluoroacetate pellets. His oxygen is normal but he dies of ventricular fibrillation. Fluoroacetate blocks which TCA enzyme, and why does it kill so fast?**

Fluoroacetate undergoes lethal synthesis in the cell. Acetyl-CoA synthetase activates it to fluoroacetyl-CoA, which citrate synthase condenses with OAA to form fluorocitrate. Fluorocitrate is a structural analog of citrate that potently inhibits aconitase (step 2 of the TCA cycle). With aconitase blocked, citrate cannot be converted to isocitrate; the TCA cycle stops after step 1. No further NADH or $\text{FADH}_2$ is produced. The electron transport chain, deprived of electron donors, ceases to pump protons. Oxidative phosphorylation collapses and cellular ATP falls. The heart is the critical vulnerable organ because cardiac muscle is almost entirely dependent on oxidative phosphorylation under normal conditions: it carries minimal glycogen, has a high and continuous ATP demand, and cannot sustain adequate ATP production through glycolysis alone. When its mitochondrial ATP synthesis fails, the cardiac action potential destabilizes and ventricular fibrillation follows within minutes.

**2. A malnourished patient gets glucose before thiamine. Her symptoms worsen. Why?**

Thiamine deficiency depletes TPP, the cofactor E1 requires in both the PDH complex and the $\alpha$-KG dehydrogenase complex. With residual TPP barely sufficient, the cell is already functioning at the edge of what these complexes can manage. When the nurses infuse glucose, glycolysis rapidly converts it to pyruvate. More pyruvate arrives at PDH than before, and the already-limited PDH complex is overwhelmed. The remaining TPP is consumed faster than it would have been without the glucose load, and the last traces of PDH activity are exhausted. Pyruvate backs up and is forced into lactate, deepening the metabolic acidosis. The ATP deficit in the brain worsens acutely because neurons were depending on whatever oxidative metabolism was still occurring. Giving thiamine first (or simultaneously) replenishes TPP before the glucose load arrives, allowing PDH to process the incoming pyruvate rather than be overwhelmed by it.

---

*Chapter 12 (The Electron Transport Chain and Oxidative Phosphorylation): The NADH and $\text{FADH}_2$ generated by the TCA cycle hand their electrons to the ETC, where four membrane complexes pass them down an energy gradient to oxygen, pumping protons across the inner mitochondrial membrane. ATP synthase then converts that proton gradient into ATP. We will account for where all 30-32 ATP come from and examine what happens when the chain is blocked.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*

---

## Problem Set

**Problem 1.**
For one complete turn of the TCA cycle starting with one acetyl-CoA:

(a) List every step that produces an electron carrier (NADH or $\text{FADH}_2$), identify the enzyme, and state which type of reaction (from the Chapter 9 classification) each represents.

(b) The only direct ATP-equivalent produced per turn is one GTP at step 5. Explain why the cycle still generates far more than 1 ATP per turn when coupled to the electron transport chain. Use approximate ATP equivalents per NADH and $\text{FADH}_2$.

(c) Steps 3 and 4 both release $\text{CO}_2$. Do these carbons come from the acetyl-CoA that entered in the same turn? Explain where they actually originate, and predict what would happen if you labeled the methyl carbon of acetyl-CoA with $^{14}\text{C}$ and followed it for two full turns of the cycle.

---

**Problem 2.**
The pyruvate dehydrogenase complex (PDH) requires five cofactors.

(a) For each cofactor, identify the vitamin precursor (if any), which subunit it is associated with (E1, E2, or E3), and its specific chemical role in the reaction.

(b) Arsenite poisoning and thiamine deficiency both knock out PDH. Identify the molecular target of each and explain why they produce overlapping but not identical biochemical effects.

(c) Inside the PDH complex, $\text{FADH}_2$ in E3 transfers its electrons to $\text{NAD}^+$. This seems to run backward from the usual direction (NADH is normally a better electron donor than $\text{FADH}_2$). The chapter notes that the FAD in E3 has a shifted $E^{\circ'}$ of approximately −0.29 V, compared to −0.32 V for $\text{NAD}^+$. Calculate $\Delta G^{\circ'}$ for the E3 electron transfer using these values (n = 2). Is it favorable or not? If not, how does the reaction still proceed?

---

**Problem 3.** *(Synthesis)*
In the fasted state, a liver cell is running fatty acid beta-oxidation extensively. This produces large amounts of acetyl-CoA and NADH inside the mitochondria.

(a) Predict the effect of elevated mitochondrial acetyl-CoA and NADH on PDH activity. Identify the specific regulatory enzyme and the phosphorylation state of E1 that results.

(b) Elevated acetyl-CoA simultaneously activates pyruvate carboxylase. Explain why activating both PDH inhibition and pyruvate carboxylase at the same time (in response to the same signal) is metabolically coherent.

(c) Citrate synthase (step 1) slows when OAA is scarce. During gluconeogenesis, OAA is diverted to PEP via PEPCK, reducing its availability in the matrix. How does the acetyl-CoA signal compensate for this, and what determines how much OAA goes to the TCA cycle versus gluconeogenesis?

---

**Problem 4.** *(Synthesis)*
Sodium fluoroacetate, a rodenticide, is converted by cells to fluoroacetyl-CoA and then to fluorocitrate, which potently inhibits aconitase.

(a) Aconitase is near-equilibrium in the normal cycle. If it is inhibited, what metabolite accumulates upstream, and what metabolite would be depleted immediately downstream?

(b) With aconitase blocked, which NADH- and $\text{FADH}_2$-generating steps of the TCA cycle can still run? Which cannot? Explain by reference to the position of aconitase in the cycle.

(c) The heart is the first organ to fail in fluoroacetate poisoning, before the liver or skeletal muscle. Explain why using the concept of each tissue's dependence on oxidative phosphorylation versus glycolysis. What would you expect to happen to plasma lactate levels, and why?

---

**Problem 5.**
The TCA cycle is both a catabolic engine and a biosynthetic hub.

(a) Name three TCA cycle intermediates that are drawn off for biosynthesis (cataplerosis) and identify one biosynthetic product each feeds into.

(b) If cataplerosis depletes OAA, the cycle can grind to a halt. Describe two distinct anaplerotic routes that replenish OAA or other intermediates, and identify the enzyme and substrate for each.

(c) A mammalian cell is given $^{13}\text{C}$-labeled acetyl-CoA as its only carbon source. It has no other carbon inputs to the TCA cycle. Explain why this cell cannot perform net gluconeogenesis from acetyl-CoA alone, using the stoichiometry of carbon entry and exit from the cycle.

---

**Problem 6.** *(Synthesis)*
Malate dehydrogenase (step 8) has a $\Delta G^{\circ'} = +29.7$ kJ/mol, yet it runs in the forward direction inside the mitochondrion.

(a) What is the primary thermodynamic mechanism that drives this unfavorable reaction forward? Be specific about which enzyme and which molecular interaction is responsible.

(b) If citrate synthase (step 1) were completely inhibited, predict what would happen to the direction of flux through malate dehydrogenase and explain your reasoning using the relationship between $\Delta G^{\circ'}$ and actual $\Delta G$.

(c) Step 8 produces the third NADH of the cycle. Given that malate dehydrogenase is near-equilibrium and responds sensitively to OAA concentrations, explain why this step can also function as a "rate-reporting" sensor of overall cycle activity.

---

**Problem 7.**
Calcium ion ($\text{Ca}^{2+}$) activates three enzymes in the pyruvate dehydrogenase and TCA cycle system: PDH phosphatase, isocitrate dehydrogenase, and $\alpha$-KG dehydrogenase.

(a) In contracting skeletal muscle, $\text{Ca}^{2+}$ is released from the sarcoplasmic reticulum to trigger contraction. Explain why activating these three enzymes at the same moment is an example of feedforward regulation rather than feedback regulation.

(b) In contrast, NADH inhibits isocitrate dehydrogenase and $\alpha$-KG dehydrogenase. What type of regulation is this, and what metabolic signal does high NADH convey?

(c) These two regulatory mechanisms — $\text{Ca}^{2+}$ activation and NADH inhibition — appear to work at cross-purposes: one turns the cycle up, the other turns it down. Under what physiological conditions would $\text{Ca}^{2+}$ be high and NADH also be high simultaneously? How might the cell resolve this conflict?

---

**Problem 8.** *(Synthesis)*
A patient with a lifelong history of episodic neurological crises is found to have a deficiency of succinate dehydrogenase (SDH, Complex II).

(a) SDH oxidizes succinate to fumarate using FAD. Why is FAD used here rather than $\text{NAD}^+$? Show using reduction potentials why $\text{NAD}^+$ cannot serve as the electron acceptor for this specific oxidation. ($E^{\circ'}_{\text{fumarate/succinate}} = +0.03$ V, $E^{\circ'}_{\text{NAD}^+/\text{NADH}} = -0.32$ V, $E^{\circ'}_{\text{FAD/FADH}_2} \approx 0$ V)

(b) SDH is simultaneously Complex II of the electron transport chain. When SDH is deficient, $\text{FADH}_2$ from this step is not produced. Using ATP equivalents, quantify the loss per glucose molecule in terms of direct ATP output from this enzyme.

(c) SDH subunit mutations cause succinate to accumulate. Excess succinate inhibits the prolyl hydroxylases that target HIF-1α for degradation. Predict the downstream effects on gene expression and cell behavior, and identify one class of tumors known to arise from SDH mutations.

---

## References

1. Berg JM, Tymoczko JL, Gatto GJ, Stryer L. *Biochemistry*, 9th ed. W.H. Freeman; 2019.
2. Nelson DL, Cox MM. *Lehninger Principles of Biochemistry*, 8th ed. W.H. Freeman; 2021.
3. Krebs HA, Johnson WA. The role of citric acid in intermediate metabolism in animal tissues. *Enzymologia*. 1937;4:148-156. [Reprinted: FEBS Lett. 1980;117(Suppl):K1-K10. doi:10.1016/0014-5793(80)80564-3]
4. Patel MS, Nemeria NS, Furey W, Jordan F. The pyruvate dehydrogenase complexes: structure-based function and regulation. *J Biol Chem*. 2014;289(24):16615-16623. doi:10.1074/jbc.R114.563148
5. Dang L, White DW, Gross S, et al. Cancer-associated IDH1 mutations produce 2-hydroxyglutarate. *Nature*. 2009;462(7274):739-744. doi:10.1038/nature08617
6. Hinkle PC. P/O ratios of mitochondrial oxidative phosphorylation. *Biochim Biophys Acta*. 2005;1706(1-2):1-11. doi:10.1016/j.bbabio.2004.09.004
7. Gibson GE, Blass JP. Thiamine-dependent processes and treatment strategies in neurodegeneration. *Antioxid Redox Signal*. 2007;9(10):1605-1619. doi:10.1089/ars.2007.1766
8. Hazell AS, Butterworth RF. Hepatic encephalopathy: an update of pathophysiologic mechanisms. *Proc Soc Exp Biol Med*. 1999;222(2):99-112. doi:10.1046/j.1525-1373.1999.d01-120.x
9. Goncharov NV, Jenkins RO, Radilov AS. Toxicology of fluoroacetate: a review, with possible directions for therapy research. *J Appl Toxicol*. 2006;26(2):148-161. doi:10.1002/jat.1118
10. Baysal BE, Ferrell RE, Willett-Brozick JE, et al. Mutations in SDHD, a mitochondrial complex II gene, in hereditary paraganglioma. *Science*. 2000;287(5454):848-851. doi:10.1126/science.287.5454.848
11. Selak MA, Armour SM, MacKenzie ED, et al. Succinate links TCA cycle dysfunction to oncogenesis by inhibiting HIF-alpha prolyl hydroxylase. *Cancer Cell*. 2005;7(1):77-85. doi:10.1016/j.ccr.2004.11.022
12. Owen OE, Kalhan SC, Hanson RW. The key role of anaplerosis and cataplerosis for citric acid cycle function. *J Biol Chem*. 2002;277(34):30409-30412. doi:10.1074/jbc.R200006200
13. Houten SM, Violante S, Ventura FV, Wanders RJ. The biochemistry and physiology of mitochondrial fatty acid β-oxidation and its genetic disorders. *Annu Rev Physiol*. 2016;78:23-44. doi:10.1146/annurev-physiol-021115-105045
