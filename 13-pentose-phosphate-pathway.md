# Chapter 13: The Pentose Phosphate Pathway

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. A 22-year-old man recently diagnosed with malaria is started on primaquine to eliminate dormant liver-stage parasites. Two days later he presents with fatigue, jaundice, and dark brown urine. His hemoglobin has fallen from 14 g/dL to 8 g/dL. A blood smear shows deformed red cells and dark inclusion bodies within them. A family history reveals that his maternal uncle had a similar reaction to an antimalarial drug years ago. His female cousin who took the same drug had no symptoms. What enzyme deficiency explains this, and why are his red blood cells the primary target?

2. A cancer biologist studying rapidly proliferating tumor cells makes a surprising observation: the cells are consuming large amounts of glucose, but much of it is not being oxidized to CO₂ or used to make ATP. Isotope tracing shows substantial flux through the pentose phosphate pathway. The cells have perfectly functional mitochondria and adequate ATP. Why would a cell that doesn't need more ATP still divert glucose into a pathway that generates no ATP?

---

## The Big Picture

The pentose phosphate pathway (PPP) is a glucose-processing route that runs in parallel with glycolysis in the cytoplasm. It does not generate ATP. By any ATP-accounting logic, it looks like a waste of glucose.

That framing misses the point entirely. The PPP solves two problems that glycolysis cannot:

**Problem 1: Biosynthesis requires reducing power in the form of NADPH.** Fatty acid synthesis, cholesterol synthesis, nucleotide synthesis, and a dozen other anabolic reactions need electrons to add to molecules. Those electrons come from NADPH, not NADH. NADH hands its electrons to the ETC to make ATP. NADPH hands its electrons to biosynthetic enzymes. They are not interchangeable in the cell.

**Problem 2: Nucleotide synthesis requires five-carbon sugars.** DNA and RNA backbones are built from ribose-5-phosphate. Glycolysis only produces three- and six-carbon intermediates. The PPP produces ribose-5-phosphate directly.

A cell that is building membranes, synthesizing DNA, detoxifying reactive oxygen species, and defending itself against oxidative damage needs NADPH constantly. The PPP is how it gets that NADPH. Every aerobic cell runs some flux through the PPP for this reason, but cells with high biosynthetic demand or high oxidative stress run a lot: liver, adrenal cortex, adipose tissue, mammary gland, and red blood cells each depend on it heavily for different reasons.

---

## Why NADPH Is Not NADH

Before getting into the pathway mechanics, it is worth establishing exactly why NADPH and NADH cannot substitute for each other, because this distinction is the whole reason the PPP exists.

NADH and NADPH are structurally nearly identical: both are dinucleotides with a nicotinamide ring that accepts or donates a hydride ($\text{H}^-$, one hydrogen plus two electrons). The only difference is a single phosphate group on the 2' position of the adenosine ribose in NADPH. That structural difference is small enough that it seems irrelevant, but enzymes distinguish them with high specificity.

Cells maintain the two pools at very different redox states:

- **NADH/NAD⁺:** mostly in the oxidized form (NAD⁺). The cell keeps this ratio low because NAD⁺ is needed as an oxidizing substrate for glycolysis and the TCA cycle. If NAD⁺ ran out, glycolysis would stop. NADH is "spent" by handing electrons to the ETC to make ATP, regenerating NAD⁺.

- **NADPH/NADP⁺:** mostly in the reduced form (NADPH). The ratio of NADPH to NADP⁺ in the cytoplasm is roughly 100:1, the opposite of the NADH/NAD⁺ ratio. Cells keep NADPH reduced because it is always being consumed by biosynthetic reactions and antioxidant defense, and the supply must not run dry.

The logic: NADH is a product of catabolism that gets reoxidized to drive ATP synthesis. NADPH is a product of the PPP (and a few other reactions) that gets reoxidized to drive biosynthesis and protection. The two pools are thermodynamically isolated from each other and kept at opposite redox poise on purpose.

What does NADPH actually do?

- **Fatty acid synthesis:** Acetyl groups are assembled into fatty acids by adding pairs of carbons with electrons donated by NADPH at two steps per round. Synthesizing one palmitate (16-carbon) consumes 14 NADPH.
- **Cholesterol synthesis:** Similarly electron-intensive; synthesis of one cholesterol requires ~18 NADPH.
- **Antioxidant defense:** Glutathione peroxidase neutralizes hydrogen peroxide by oxidizing reduced glutathione (GSH) to oxidized glutathione (GSSG). Glutathione reductase regenerates GSH from GSSG using NADPH. Without NADPH, glutathione stays oxidized and cannot protect the cell from $\text{H}_2\text{O}_2$ and lipid peroxides.
- **Cytochrome P450 reactions:** Drug and steroid metabolism in the liver and adrenal cortex requires NADPH to donate electrons to P450 enzymes.
- **NADPH oxidase in phagocytes:** Neutrophils and macrophages intentionally generate superoxide ($\text{O}_2^{\bullet-}$) to kill ingested pathogens. The enzyme that does this, NADPH oxidase, consumes NADPH. The respiratory burst of a neutrophil engulfing bacteria is powered entirely by PPP-derived NADPH.

Each of these processes consumes NADPH and raises the NADP⁺/NADPH ratio slightly. That rising NADP⁺ concentration is the signal that more NADPH is needed, which activates the PPP, as covered in the regulation section below.

---

## The Oxidative Phase

The PPP is typically referred to as split into two phases, the oxidative phase and the non-oxidative phase. The oxidative phase is the irreversible part of the PPP. It takes glucose-6-phosphate (G6P) and converts it to ribulose-5-phosphate, releasing one carbon as $\text{CO}_2$ and generating two NADPH in the process. Three enzyme-catalyzed steps accomplish this.

### Step 1: Glucose-6-Phosphate Dehydrogenase

$$\text{Glucose-6-phosphate} + \text{NADP}^+ \rightarrow \text{6-Phosphoglucono-}\delta\text{-lactone} + \text{NADPH} + \text{H}^+$$

This is the committed step of the pathway and the primary site of regulation. Glucose-6-phosphate dehydrogenase (G6PDH) oxidizes the C1 position of G6P, converting the aldehyde carbon to a lactone while reducing NADP⁺ to NADPH. The product, 6-phosphoglucono-δ-lactone, is a cyclic ester.

The reaction is essentially irreversible under cellular conditions, driven both by the large negative free energy and by the removal of products as subsequent reactions consume them.

### Step 2: Lactonase

$$\text{6-Phosphoglucono-δ-lactone} + \text{H}_2\text{O} \rightarrow \text{6-Phosphogluconate}$$

6-Phosphogluconolactonase hydrolyzes the lactone ring, opening it to the linear 6-phosphogluconate. This step is not regulated and proceeds spontaneously at a useful rate, though the enzyme accelerates it. No cofactors, no energy input.

### Step 3: 6-Phosphogluconate Dehydrogenase

$$\text{6-Phosphogluconate} + \text{NADP}^+ \rightarrow \text{Ribulose-5-phosphate} + \text{CO}_2 + \text{NADPH} + \text{H}^+$$

This is the second NADPH-generating step. 6-Phosphogluconate dehydrogenase oxidizes and decarboxylates 6-phosphogluconate in a single reaction, reducing another NADP⁺ to NADPH and releasing C1 as $\text{CO}_2$. The mechanism is analogous to isocitrate dehydrogenase in the TCA cycle: oxidation generates a $\beta$-keto acid intermediate, which then decarboxylates spontaneously.

The net result of the oxidative phase:

$$\text{Glucose-6-phosphate} + 2\text{NADP}^+ + \text{H}_2\text{O} \rightarrow \text{Ribulose-5-phosphate} + \text{CO}_2 + 2\text{NADPH} + 2\text{H}^+$$

One G6P in. One ribulose-5-phosphate plus one $\text{CO}_2$ out. Two NADPH generated. An important thing to keep in mind is that we have now lost one carbon as $\text{CO}_2$ meaning that it is no longer available to generate ATP as we've discussed: Generating NADPH incurs a direct and measureable energy cost.

---

## The Non-Oxidative Phase

Once ribulose-5-phosphate is produced, the cell faces a choice: use it as ribose-5-phosphate for nucleotide synthesis, or convert it back into glycolytic intermediates (fructose-6-phosphate and glyceraldehyde-3-phosphate) to finish oxidizing the carbon for energy. The non-oxidative phase provides the enzymatic machinery to do either.

The reactions are reversible, which is the key. The pathway can run forward (pentoses into glycolytic intermediates) or backward (glycolytic intermediates into pentoses), depending on what the cell needs.

### Starting Interconversions

Ribulose-5-phosphate, the output of the oxidative phase, is not itself used for nucleotide synthesis. Two enzymes convert it to the useful pentose forms:

- **Phosphopentose isomerase** converts ribulose-5-phosphate to **ribose-5-phosphate**, which feeds nucleotide synthesis.
- **Phosphopentose epimerase** converts ribulose-5-phosphate to **xylulose-5-phosphate**, a different stereoisomer that feeds the transketolase reactions.

### Transketolase and Transaldolase

These two enzymes are the heart of the non-oxidative phase. They interconvert three-, four-, five-, six-, and seven-carbon sugar phosphates by shuffling carbon fragments between them.

**Transketolase** transfers two-carbon units from a ketose donor to an aldose acceptor. It requires **thiamine pyrophosphate (TPP)** as a cofactor, the same cofactor used by pyruvate dehydrogenase and $\alpha$-ketoglutarate dehydrogenase. The two-carbon unit is transiently held on the TPP while it waits for an acceptor aldose. Transketolase catalyzes two distinct reactions in the non-oxidative phase.

**Transaldolase** transfers three-carbon units from a ketose donor to an aldose acceptor. It uses no cofactor; instead it forms a transient Schiff base between the carbonyl carbon of the donor and an active-site lysine residue, holding the three-carbon fragment covalently while the remaining carbon skeleton dissociates, then transferring it to an acceptor.

### The Carbon Shuffling Sequence

Starting from three molecules of ribulose-5-phosphate, the non-oxidative phase proceeds as follows. The intermediate names matter less than the logic of what is happening.

**Step A** (isomerase and epimerase): 3 Ribulose-5-phosphate $\rightarrow$ 1 Ribose-5-phosphate + 2 Xylulose-5-phosphate

**Step B** (Transketolase 1): Xylulose-5-phosphate (5C) + Ribose-5-phosphate (5C) $\rightarrow$ Sedoheptulose-7-phosphate (7C) + Glyceraldehyde-3-phosphate (3C)

Transketolase takes a two-carbon unit from xylulose-5-phosphate and transfers it onto ribose-5-phosphate, yielding a seven-carbon product and leaving a three-carbon glyceraldehyde-3-phosphate.

**Step C** (Transaldolase): Sedoheptulose-7-phosphate (7C) + Glyceraldehyde-3-phosphate (3C) $\rightarrow$ Erythrose-4-phosphate (4C) + Fructose-6-phosphate (6C)

Transaldolase takes a three-carbon unit from sedoheptulose-7-phosphate and transfers it onto glyceraldehyde-3-phosphate, yielding erythrose-4-phosphate and fructose-6-phosphate.

**Step D** (Transketolase 2): Xylulose-5-phosphate (5C) + Erythrose-4-phosphate (4C) $\rightarrow$ Glyceraldehyde-3-phosphate (3C) + Fructose-6-phosphate (6C)

Transketolase takes another two-carbon unit from the second xylulose-5-phosphate and transfers it onto erythrose-4-phosphate.

**Net from 3 ribulose-5-phosphate:**

$$3 \text{ Ribulose-5-P} \rightarrow 2 \text{ Fructose-6-P} + \text{ Glyceraldehyde-3-P}$$

Fructose-6-phosphate and glyceraldehyde-3-phosphate are both glycolytic intermediates. They can enter glycolysis directly and be oxidized to pyruvate, or they can be used in gluconeogenesis to regenerate glucose-6-phosphate.

---

## Matching Output to Need: The PPP as a Flexible Hub

The real elegance of the PPP is its flexibility. The cell does not have a fixed ratio of NADPH to ribose-5-phosphate that it always needs. Different situations call for different outputs, and the PPP adjusts.

**When the cell needs NADPH but not ribose-5-phosphate** (for example, a liver cell synthesizing fatty acids): run the oxidative phase at high flux and then funnel the ribulose-5-phosphate into the non-oxidative phase to regenerate glycolytic intermediates, which can eventually become G6P again. This effectively converts glucose into NADPH while recycling the carbon. If you run six molecules of G6P through the oxidative phase and recycle the products back, you net 12 NADPH and release 6 CO$_2$, at the cost of one full glucose equivalent.

**When the cell needs both NADPH and ribose-5-phosphate** (for example, a rapidly dividing cell synthesizing DNA): run the oxidative phase to generate both. The ribulose-5-phosphate can be isomerized to ribose-5-phosphate for nucleotide synthesis, and the NADPH goes to biosynthesis and defense.

**When the cell needs ribose-5-phosphate but not much NADPH** (for example, a cell making nucleotides under conditions of adequate antioxidant capacity): run the non-oxidative phase in reverse. Take fructose-6-phosphate and glyceraldehyde-3-phosphate from glycolysis and interconvert them into ribose-5-phosphate via transketolase and transaldolase, without touching the oxidative phase at all. No NADPH is generated; the cell just converts glycolytic intermediates into the pentose it needs.

This reversibility is the reason the non-oxidative phase matters. If ribose-5-phosphate were only accessible by running G6P through the oxidative phase, the cell would be forced to produce NADPH every time it needed nucleotides, even if NADPH were already abundant. The non-oxidative phase decouples ribose-5-phosphate production from NADPH production.

### Regulation

The PPP is regulated primarily at G6PD, the committed first step. G6PD is subject to product inhibition by NADPH: when NADPH is abundant, the enzyme slows down. When NADPH is depleted and NADP$^+$ rises, the enzyme speeds up. The ratio of NADP$^+$/NADPH is the sensor.

This is straightforward feedback control, and it is appropriate: the purpose of the oxidative phase is to produce NADPH, so NADPH itself signals when enough has been made. No other elaborate regulatory mechanism is needed because the substrate (G6P) is also the substrate for glycolysis, and any G6P not diverted to the PPP simply stays available for glycolysis.

---

## When It Breaks: G6PD Deficiency

### The Biochemistry of Hemolysis

Glucose-6-phosphate dehydrogenase deficiency is the most common enzyme deficiency in humans, affecting approximately 400 million people worldwide. The gene encoding G6PD is on the X chromosome, which means males have only one copy. A single defective copy produces the phenotype. Females with one defective copy are carriers; they are usually asymptomatic but can have intermediate enzyme activity depending on X-inactivation patterns.

The clinical presentation is not chronic disease. Most people with G6PD deficiency are perfectly healthy most of the time. The problem is triggered by oxidative stress: hemolytic anemia appears episodically when red blood cells are exposed to oxidizing agents, and resolves when the exposure stops.

Why are red blood cells the primary target?

Most cells protect themselves from oxidative stress through multiple backup systems: they can synthesize glutathione, they have catalase and superoxide dismutase, and their mitochondria can generate some NADPH via the TCA cycle (specifically through isocitrate dehydrogenase and the transhydrogenase reaction). Red blood cells have none of these alternatives. Mature erythrocytes have no nucleus and no mitochondria. They cannot synthesize new proteins to replace damaged enzymes. They cannot run the TCA cycle. The **PPP is their only source of NADPH**, and G6PD is the only gatekeeper. If G6PD fails, NADPH falls, reduced glutathione (GSH) cannot be regenerated, and the cell loses its sole defense against oxidative damage.

When reactive oxygen species accumulate, they attack hemoglobin directly. Oxidized hemoglobin denatures and precipitates inside the red cell, forming visible dark inclusions called **Heinz bodies**. The deformed cells are rigid and fragile. As they circulate through the spleen, the splenic sinusoids physically strip out the Heinz body-containing portions of the membrane, producing bite cells visible on a blood smear. Eventually the cells lyse, releasing hemoglobin into the plasma. Plasma hemoglobin is filtered at the kidney and appears in urine as hemoglobinuria, causing the characteristic dark brown or cola-colored urine that often brings patients to attention.

### What Triggers the Crisis

The oxidative stress that tips G6PD-deficient cells over the edge can come from several sources:

**Infections** are the most common trigger. The inflammatory response generates reactive oxygen species, and even without any medication, a bacterial or viral infection can trigger hemolysis in a G6PD-deficient patient.

**Certain drugs** are powerful oxidizing agents: primaquine (the 8-aminoquinoline antimalarial used to eliminate liver-stage Plasmodium vivax and for PQ prophylaxis), dapsone (used for leprosy and Pneumocystis prophylaxis), rasburicase (urate oxidase, used for tumor lysis syndrome), and nitrofurantoin (a urinary antibiotic). These drugs or their metabolites directly oxidize glutathione, consuming NADPH faster than a G6PD-deficient cell can replenish it.

**Fava beans** (broad beans) contain the glycosides divicine and isouramil, which are oxidizing compounds. The hemolytic crisis triggered by fava bean ingestion in G6PD-deficient individuals is called **favism** and was likely the first clinical description of G6PD deficiency, documented in populations around the Mediterranean thousands of years before the biochemistry was understood.

### The Malaria Connection

G6PD deficiency is extraordinarily common in sub-Saharan Africa, the Mediterranean, the Middle East, and parts of Southeast Asia. These are also the regions where malaria has been historically most prevalent. This overlap is not coincidental.

The molecular epidemiology is striking: G6PD deficiency alleles in African populations (notably G6PD A$^-$, named for the electrophoretic variant) reach carrier frequencies of 10–25% in malaria-endemic regions. This is far too high for a disease-causing mutation to maintain without selection pressure. The explanation is that G6PD-deficient red blood cells are inhospitable to *Plasmodium falciparum*. The parasite depends on red cell glutathione and reducing capacity to manage its own oxidative stress; in a G6PD-deficient cell, the oxidative environment is lethal to the parasite. Heterozygous females appear to have the strongest protection, which likely explains why the allele has been maintained rather than selected out despite its clinical cost in affected males.

G6PD deficiency is the canonical example of balanced polymorphism in human genetics: an allele that causes harm in one context (exposure to oxidizing drugs or infections) confers survival advantage in another (malaria). The sickle cell trait is a parallel example from a different gene in the same disease context.

### The Glutathione Redox Cycle

The molecular logic is worth spelling out explicitly because it appears repeatedly in clinical and research contexts:

$$\text{GSSG} + \text{NADPH} + \text{H}^+ \xrightarrow{\text{glutathione reductase}} 2\text{ GSH}$$

$$2\text{ GSH} + \text{H}_2\text{O}_2 \xrightarrow{\text{glutathione peroxidase}} \text{GSSG} + 2\text{H}_2\text{O}$$

Every molecule of $\text{H}_2\text{O}_2$ neutralized consumes one NADPH (via the glutathione cycle). When NADPH production is impaired by G6PD deficiency, GSSG accumulates, GSH is depleted, and $\text{H}_2\text{O}_2$ and lipid peroxides are no longer neutralized. In most cells, NADPH from other sources (malate dehydrogenase in the mitochondria, folate metabolism) provides backup. In the red cell, there is no backup.

---

## Transketolase, Thiamine, and Wernicke's Encephalopathy

Transketolase requires thiamine pyrophosphate (TPP) as its cofactor. The TPP is covalently bound at the active site and holds the two-carbon fragment during transfer. Without TPP, the non-oxidative phase stops.

This is relevant clinically because thiamine (vitamin B1) deficiency is relatively common in populations with poor nutrition, chronic alcoholism, malabsorption, or prolonged parenteral nutrition without supplementation. Thiamine deficiency impairs three TPP-dependent enzymes simultaneously: pyruvate dehydrogenase (PDH), $\alpha$-ketoglutarate dehydrogenase in the TCA cycle, and transketolase. The result is a combined block in aerobic glucose metabolism at multiple levels.

**Wernicke's encephalopathy** is the acute neurological emergency that results from severe thiamine deficiency. The classic triad is confusion, ataxia (unsteady gait), and ophthalmoplegia (abnormal eye movements), though all three are present simultaneously in only a minority of cases. Lesions occur preferentially in the mammillary bodies, thalamus, and periaqueductal gray.

The reason neuronal injury dominates in thiamine deficiency is that the brain is almost entirely dependent on glucose metabolism and runs its neurons at very high aerobic metabolic rates. When PDH and $\alpha$-KGDH fail, ATP production in neurons collapses. The selective regional vulnerability reflects local differences in metabolic rate and in the ratio of thiamine-dependent enzyme activity to reserve capacity.

Critically: **administering glucose before thiamine can precipitate or worsen Wernicke's encephalopathy.** A glucose load increases the demand for thiamine-dependent metabolism (more pyruvate is produced that needs PDH to proceed into the TCA cycle) in a patient whose thiamine stores are already critically depleted. The residual TPP is consumed rapidly, pushing the patient into overt thiamine-deficient crisis. The correct protocol in any patient with suspected thiamine deficiency is thiamine first, glucose second. The nurse who starts a glucose drip on an undiagnosed malnourished patient may be the proximate cause of irreversible neurological damage.

The clinical test for thiamine deficiency is erythrocyte transketolase activity, measured with and without added TPP. In thiamine-deficient patients, activity rises substantially when TPP is added (because the enzyme is present but cofactor-starved), while in replete patients there is no response. This assay directly measures the functional capacity of the non-oxidative PPP in a clinically accessible cell type.

---

## A Note on NADPH Oxidase and Chronic Granulomatous Disease

One useful comparison point for understanding NADPH's role in immune function: while G6PD deficiency impairs the antioxidant use of NADPH in red cells, a different inherited disease illustrates what happens when phagocytes cannot use NADPH for its oxidative purpose.

**Chronic granulomatous disease (CGD)** is caused by mutations in the genes encoding NADPH oxidase (NOX2 and its accessory subunits). Normally, when a neutrophil engulfs a bacterium, it triggers a respiratory burst: a rapid spike of NADPH consumption that reduces $\text{O}_2$ to superoxide ($\text{O}_2^{\bullet-}$), which dismutates to $\text{H}_2\text{O}_2$ and further generates microbicidal reactive oxygen species. This burst kills catalase-negative organisms efficiently. In CGD, the burst cannot happen. Catalase-positive organisms (Staphylococcus aureus, Aspergillus, Serratia, Nocardia, and Burkholderia among others) survive inside phagosomes and spread. The result is recurrent, severe, and unusual infections along with excessive inflammation as the immune system builds granulomas trying to wall off organisms it cannot kill. These patients need lifelong prophylactic antibiotics and antifungals, and some require bone marrow transplantation.

Note the distinction from G6PD deficiency: G6PD deficiency reduces NADPH availability, which impairs glutathione regeneration and the antioxidant capacity of red cells. CGD eliminates the enzyme that uses NADPH to make reactive oxygen species in phagocytes. Same upstream currency (NADPH), opposite downstream consequences.

---

## The MCAT Angle

The PPP appears on the MCAT in three recurring contexts.

**G6PD deficiency and hemolytic anemia.** The MCAT will present a patient who develops hemolysis after drug exposure, ask you to identify the enzyme and explain the mechanism. The key reasoning chain is: oxidative stress consumed NADPH $\to$ NADPH is needed to regenerate reduced glutathione $\to$ GSH is needed to neutralize $\text{H}_2\text{O}_2$ $\to$ without GSH, hemoglobin oxidizes and forms Heinz bodies $\to$ cells lyse. Red cells are selectively vulnerable because they have no mitochondria and cannot make NADPH any other way.

**NADPH versus NADH.** The MCAT tests whether you understand that NADPH is the reducing agent for biosynthesis and antioxidant defense, while NADH is the reducing agent for oxidative phosphorylation. A question might ask why a cell synthesizing large amounts of fatty acids needs the PPP, or why blocking G6PD specifically impairs antioxidant defense rather than energy metabolism. The distinction is about where the reducing equivalents flow.

**Thiamine and the non-oxidative phase.** The MCAT tests Wernicke's encephalopathy and the rule: thiamine before glucose. Questions may ask which enzymes are impaired (PDH, $\alpha$-KGDH, transketolase) and why glucose loading worsens the condition. You are also expected to recognize that the erythrocyte transketolase assay is the functional test for thiamine status.

**The MCAT will not ask you to trace every carbon through the non-oxidative phase.** Recognizing what the pathway produces (NADPH and ribose-5-phosphate), what triggers it (NADP$^+$ rise), and where it is most important (red cells, liver, adrenal cortex, rapidly dividing cells) is sufficient for almost all questions.

---

## Worked Problems

### Problem A

A 45-year-old man with glucose-6-phosphate dehydrogenase deficiency is prescribed rasburicase for tumor lysis syndrome during induction chemotherapy. His hemoglobin drops from 11 g/dL to 6.5 g/dL over 36 hours. His blood smear shows bite cells and spherocytes.

Rasburicase is a recombinant urate oxidase that converts uric acid to allantoin, producing $\text{H}_2\text{O}_2$ as a byproduct: Urate + $\text{O}_2$ + $\text{H}_2\text{O}$ $\rightarrow$ Allantoin + $\text{H}_2\text{O}_2$.

(a) Trace the biochemical sequence from rasburicase activity to Heinz body formation.

(b) The patient's internist suggests switching to febuxostat, a xanthine oxidase inhibitor that reduces uric acid production rather than converting it. Would this prevent hemolysis? Why or why not?

**Answer:**

(a) Rasburicase generates $\text{H}_2\text{O}_2$ as a direct byproduct of each catalytic cycle. $\text{H}_2\text{O}_2$ in the plasma enters red blood cells and must be neutralized by glutathione peroxidase, which oxidizes two GSH to GSSG. Regenerating GSH from GSSG requires NADPH via glutathione reductase. In a G6PD-deficient red cell, NADPH production from the PPP is severely impaired (the enzyme is present but dysfunctional). NADPH cannot be replenished from TCA cycle sources because mature erythrocytes have no mitochondria. GSSG accumulates, GSH falls, and $\text{H}_2\text{O}_2$ neutralization fails. $\text{H}_2\text{O}_2$ then oxidizes hemoglobin to methemoglobin and ferryl species, which aggregate into Heinz bodies. Heinz body-containing cells are rigid; the spleen's sinusoids strip membrane-enclosed Heinz bodies from passing erythrocytes, producing bite cells. Eventually the cells lyse, dropping the hemoglobin to 6.5 g/dL.

(b) Yes, switching to febuxostat would prevent the hemolysis triggered by rasburicase. Febuxostat reduces uric acid production by inhibiting xanthine oxidase upstream; it does not generate $\text{H}_2\text{O}_2$ as a byproduct. With no $\text{H}_2\text{O}_2$ load, the glutathione cycle is not overwhelmed, and the G6PD deficiency is not clinically relevant. Rasburicase is explicitly contraindicated in G6PD deficiency for exactly this reason; febuxostat is the preferred alternative for uric acid management in these patients.

---

### Problem B

A research group grows two cell lines under identical conditions: a line selected for high NADPH demand (active fatty acid synthesis) and a line with normal biosynthetic activity. Both lines have identical G6PD protein levels. The high-NADPH line shows threefold higher PPP flux.

(a) Without changing enzyme levels, what drives the increased PPP flux in the high-NADPH line?

(b) The researchers add an inhibitor of fatty acid synthase to the high-NADPH line. Within 30 minutes, PPP flux drops back to the level of the control line. What does this tell you about the signal linking biosynthetic demand to PPP activity?

**Answer:**

(a) Fatty acid synthesis consumes NADPH at two steps per elongation cycle. High biosynthetic activity continuously oxidizes NADPH to NADP$^+$, raising the NADP$^+$/NADPH ratio. G6PD is product-inhibited by NADPH and substrate-activated by NADP$^+$. A higher NADP$^+$ concentration relieves product inhibition and provides more substrate, increasing G6PD activity and PPP flux. No change in enzyme levels is required; the activity of existing G6PD molecules is modulated by the local redox ratio.

(b) When fatty acid synthase is inhibited, NADPH consumption stops. NADPH accumulates (it is no longer being consumed by biosynthesis), NADP$^+$ falls, and G6PD activity drops due to product inhibition by the rising NADPH. PPP flux decreases within minutes because the stimulus (high NADP$^+$) is removed. This confirms that the immediate signal coupling PPP activity to biosynthetic demand is the NADP$^+$/NADPH ratio, acting directly on G6PD, not a slower transcriptional response.

---

### Problem C

A poorly nourished 38-year-old man who drinks heavily is admitted with confusion, horizontal nystagmus, and ataxia. The admitting team starts a 5% dextrose IV drip while ordering labs. Over the next two hours, his confusion worsens and he develops bilateral lateral gaze palsies.

(a) What is the diagnosis, and which cofactor is deficient?

(b) Explain mechanistically why glucose administration worsened his condition before thiamine was given.

(c) Which three enzymes share this cofactor, and what metabolic processes do each support?

(d) His nurse notes that his red cell transketolase activity (measured without added TPP) is 22% of normal, but rises to 94% of normal when exogenous TPP is added to the assay. Interpret this result.

**Answer:**

(a) Wernicke's encephalopathy, caused by thiamine (vitamin B1) deficiency. The classic triad of confusion, ophthalmoplegia (abnormal eye movements, including the nystagmus and lateral gaze palsies), and ataxia should trigger immediate thiamine administration without waiting for confirmatory labs.

(b) Glucose administration in a thiamine-depleted patient increased glycolytic flux, producing more pyruvate. Pyruvate dehydrogenase (PDH) is a thiamine pyrophosphate (TPP)-dependent enzyme that converts pyruvate to acetyl-CoA. With TPP severely depleted, PDH cannot keep pace with the surge of pyruvate from accelerated glycolysis. Pyruvate accumulates and is shunted to lactate (lactic acidosis) or crosses into the brain. The neurons in high-metabolic demand regions already operating near their reserve capacity lose the ability to sustain oxidative phosphorylation, and their residual TPP is depleted further by the glucose-driven demand. The neurons most vulnerable (in the mammillary bodies, periaqueductal gray, and thalamus) begin to die. The principle: never give glucose to a malnourished or potentially thiamine-deficient patient before giving thiamine.

(c) The three TPP-dependent enzymes are:
- **Pyruvate dehydrogenase:** converts pyruvate to acetyl-CoA, linking glycolysis to the TCA cycle and fatty acid synthesis.
- **$\alpha$-Ketoglutarate dehydrogenase:** catalyzes step 4 of the TCA cycle (oxidative decarboxylation of $\alpha$-ketoglutarate to succinyl-CoA), a key ATP-generating step.
- **Transketolase:** transfers two-carbon units in the non-oxidative phase of the PPP, enabling interconversion between pentose phosphates and glycolytic intermediates.

All three are impaired simultaneously in thiamine deficiency, compounding the metabolic disruption.

(d) The assay result shows that transketolase protein is present and structurally normal, but functionally impaired due to cofactor insufficiency, not enzyme destruction. At 22% of normal activity without TPP, the enzyme is starved for cofactor: only a small fraction of enzyme molecules have TPP bound. When TPP is added back, activity restores to 94% of normal, confirming the enzyme itself is intact and that the limitation was cofactor availability. This is the expected pattern in thiamine deficiency: enzymes are synthesized and folded correctly, but cannot function because the body cannot supply sufficient TPP. The result also demonstrates why this assay is a more reliable index of functional thiamine status than plasma thiamine levels, which fluctuate with recent dietary intake rather than reflecting cofactor saturation of target enzymes.

---

## Opener Questions Revisited

**1. Young man with hemolysis after primaquine. Why red cells? Why males predominantly?**

The patient has G6PD deficiency. The G6PD gene is X-linked; males have one copy and a single defective allele is sufficient to cause enzyme deficiency. Females with one defective copy are usually protected by the functional allele on their second X chromosome, though severely skewed X-inactivation can produce clinical disease in carrier females.

Primaquine (and its metabolites) is an oxidizing compound. In most cells, the oxidative insult from primaquine metabolites is neutralized by the glutathione system, which is continuously replenished using NADPH from multiple sources. Mature red blood cells have no mitochondria and no nucleus. They cannot synthesize new enzymes, cannot run the TCA cycle, and cannot generate NADPH from any source other than G6PD in the PPP. When primaquine depletes their glutathione, there is no backup. Hemoglobin oxidizes, Heinz bodies form, and the spleen destroys the damaged cells.

Other nucleated cells in the same patient survive primaquine exposure because they have alternative NADPH sources and can upregulate antioxidant enzyme expression in response to stress. The red cell cannot do either.

The family history (maternal uncle affected, female cousin unaffected) fits X-linked recessive inheritance perfectly: males express the phenotype, females are protected by the second allele.

**2. Tumor cells divert glucose to the PPP despite adequate ATP. Why?**

Rapidly proliferating cells have two metabolic needs that glycolysis and oxidative phosphorylation do not meet: ribose-5-phosphate for DNA and RNA synthesis, and NADPH for biosynthesis of fatty acids and cholesterol needed to make membranes, and for managing the oxidative stress of rapid proliferation. A tumor doubling its cell mass every few hours must synthesize vast quantities of nucleotides, lipids, and proteins. These processes are NADPH-intensive and ribose-intensive.

The Warburg effect describes the observation that cancer cells preferentially perform aerobic glycolysis (high glucose consumption, lactate secretion) even when oxygen is available. Part of the explanation is that glycolytic intermediates and PPP products feed biosynthesis. ATP is not the scarce resource in a proliferating tumor; building materials are. Diverting glucose to the PPP trades ATP production potential for NADPH and ribose-5-phosphate, which the cell needs more urgently than more ATP. The PPP flux in proliferating tumor cells is a readout of biosynthetic demand, not a sign of metabolic dysfunction.

---

*Chapter 14: Now that we have the major oxidative pathways in place, we can turn to the metabolic logic of fuel storage and mobilization. Glycogen is the cell's short-term glucose buffer, and $\beta$-oxidation is the route that turns stored fat back into acetyl-CoA. Both pathways feed into intermediates we have already seen, which means the accounting is now straightforward.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*

---

## References

1. Cappellini MD, Fiorelli G. Glucose-6-phosphate dehydrogenase deficiency. Lancet. 2008;371(9606):64-74.

2. Luzzatto L, Ally M, Notaro R. Glucose-6-phosphate dehydrogenase deficiency. Blood. 2020;136(11):1225-1240.

3. Ruwende C, Hill A. Glucose-6-phosphate dehydrogenase deficiency and malaria. J Mol Med. 1998;76(8):581-588.

4. Harper C. Thiamine (vitamin B1) deficiency and associated brain damage is still common throughout the world and prevention is simple and safe! Eur J Neurol. 2006;13(10):1078-1082.

5. Stincone A, Prigione A, Cramer T, et al. The return of metabolism: biochemistry and physiology of the pentose phosphate pathway. Biol Rev Camb Philos Soc. 2015;90(3):927-963.

6. Ciccarese F, Ciminale V. Escaping death: mitochondrial redox homeostasis in cancer cells. Front Oncol. 2017;7:117.

7. Segal AW. How neutrophils kill microbes. Annu Rev Immunol. 2005;23:197-223.
