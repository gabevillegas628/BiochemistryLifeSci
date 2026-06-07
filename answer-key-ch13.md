# Answer Key — Chapter 13: The Pentose Phosphate Pathway

---

## Problem 1

**(a) The structural difference between NADPH and NADH:**

The only structural difference is a phosphate group on the 2' hydroxyl of the adenosine ribose in NADPH. NADH has a free hydroxyl at that position; NADPH has a phosphate ester. This difference is small enough to seem cosmetic, but enzymes read it with high specificity. The 2'-phosphate in NADPH is recognized by anabolic enzymes (fatty acid synthase, glutathione reductase, cytochrome P450 reductase), which evolved binding pockets complementary to it. Catabolic enzymes that use NADH (lactate dehydrogenase, malate dehydrogenase, the ETC complexes) evolved pockets that fit the unphosphorylated adenosine and exclude the phosphate. Because the two pools are handled by separate enzyme families, the cell can maintain them at opposite redox states: NADH mostly oxidized (NAD⁺ predominates) and NADPH mostly reduced (NADPH predominates at roughly 100:1).

**(b) Why NADH cannot substitute for NADPH in fatty acid synthesis:**

The chemistry of hydride donation is the same, but the enzymes are not. Fatty acid synthase requires NADPH at its enoyl reductase and ketoreductase active sites; those sites are shaped to bind NADPH and exclude NADH. No amount of surplus NADH allows fatty acid synthesis to proceed because the enzyme simply does not bind it. Beyond the binding problem, there is a thermodynamic reason the substitution would fail even in principle: NADH is a catabolic cofactor that cells keep mostly oxidized. If fatty acid synthesis consumed NADH, it would compete directly with the ETC for the same pool, creating futile competition between anabolism and energy generation. Maintaining two structurally distinct pools allows the cell to use NADH for ATP production and NADPH for biosynthesis simultaneously, without one draining the other.

**(c) NADPH cost of palmitate synthesis:**

Each two-carbon elongation cycle of fatty acid synthesis consumes 2 NADPH (one at the ketoreductase step, one at the enoyl reductase step). Synthesizing palmitate (16 carbons) from acetyl-CoA requires 7 elongation cycles:

$$7 \text{ cycles} \times 2 \text{ NADPH/cycle} = \mathbf{14 \text{ NADPH per palmitate}}$$

The liver obtains the bulk of its cytoplasmic NADPH from the PPP, specifically from the two oxidative-phase reactions catalyzed by G6PD and 6-phosphogluconate dehydrogenase. The malic enzyme reaction (malate → pyruvate + CO₂, coupled to NADP⁺ reduction) is a secondary source in hepatocytes, but the PPP is quantitatively dominant for the large NADPH demand of active lipogenesis.

---

## Problem 2

**(a) Net reaction for the oxidative phase:**

$$\text{Glucose-6-phosphate} + 2\text{NADP}^+ + \text{H}_2\text{O} \rightarrow \text{Ribulose-5-phosphate} + \text{CO}_2 + 2\text{NADPH} + 2\text{H}^+$$

One G6P enters. One ribulose-5-phosphate and one CO₂ exit. Two NADPH are produced. One carbon (C1 of G6P) is irreversibly lost as CO₂.

**(b) Why regulation at the committed step rather than at a later step:**

Once G6PD has oxidized G6P to 6-phosphoglucono-δ-lactone, the substrate is committed: the lactone has no metabolic fate other than proceeding through lactonase and 6-phosphogluconate dehydrogenase. If the regulated step were instead the second NADPH-generating reaction (6-phosphogluconate dehydrogenase), then a spike in NADPH could slow that step, but 6-phosphogluconate would have already accumulated — it would sit in the cell as a dead-end intermediate, representing G6P that has been pulled away from glycolysis and partially oxidized to no productive end. Regulating the first irreversible step (G6PD) prevents this waste: G6P is only diverted to the PPP when NADPH is actually needed, and if NADPH rises, the diversion stops before any G6P is consumed unnecessarily. The general principle is that metabolic pathways are most efficiently controlled at their first committed step, not downstream of it.

**(c) Two-step mechanism shared by 6-phosphogluconate dehydrogenase and isocitrate dehydrogenase:**

Both enzymes accomplish **oxidative decarboxylation** in a single active-site sequence. The mechanism proceeds in two stages:

1. **Oxidation:** The substrate is oxidized by NADP⁺ at a hydroxyl adjacent to a carboxylate, generating a β-keto acid intermediate (3-keto-6-phosphogluconate in the PPP; oxalosuccinate in the TCA cycle) and NADPH.

2. **Decarboxylation:** The β-keto acid is inherently unstable and decarboxylates spontaneously (or enzyme-assisted), releasing CO₂ and producing the final product (ribulose-5-phosphate or α-ketoglutarate).

In both cases the β-keto acid intermediate is not released from the enzyme — it decarboxylates while still bound. The analogy extends to cofactor requirement (NADP⁺ in both), reaction irreversibility, and regulatory significance: both are control points in their respective pathways.

---

## Problem 3

**(a) Chain of events from cholesterol synthesis to increased PPP flux:**

Cholesterol synthesis runs a sustained demand for NADPH: each molecule synthesized consumes approximately 18 NADPH. As NADPH is consumed, it is oxidized to NADP⁺. The NADP⁺/NADPH ratio in the cytoplasm rises. G6PD is product-inhibited by NADPH: high NADPH keeps the enzyme in a partially inhibited state. As NADPH falls and NADP⁺ rises, product inhibition is relieved and the substrate concentration at the active site increases. G6PD activity rises in proportion to the NADP⁺/NADPH ratio, channeling more G6P through the oxidative phase, generating more NADPH, and replenishing the pool consumed by cholesterol synthesis. The entire response occurs within the timescale of enzyme kinetics — seconds to minutes — with no change in gene expression required. Depending on the energy state of the cell, the PPP may be running in mode 2, 3 or 4 or a combination of them.

**(b) Effect of statin inhibition on NADP⁺/NADPH ratio and PPP flux:**

Inhibiting HMG-CoA reductase slows cholesterol synthesis, reducing NADPH consumption. NADPH is no longer being drawn down; it accumulates as NADP⁺ is converted back to NADPH faster than it is consumed. The NADP⁺/NADPH ratio falls. G6PD, which is product-inhibited by NADPH, experiences rising NADPH and slows down. PPP flux decreases within minutes, not because any enzyme is directly drug-targeted, but because the metabolic signal driving it (elevated NADP⁺) has been removed. This is the same feedback mechanism in reverse: biosynthetic demand sets the pace of NADPH production, and reducing demand automatically reduces supply.

**(c) Why controlling G6PD alone is sufficient:**

G6PD is the committed step: once G6P is oxidized to 6-phosphoglucono-δ-lactone, the molecule has no pathway other than proceeding through lactonase and 6-phosphogluconate dehydrogenase to ribulose-5-phosphate. The downstream steps have no branch points and no alternative substrates. Therefore, the rate at which G6PD commits G6P to the oxidative phase is the rate of the entire phase. Adding regulation at step 3 would be redundant: if G6PD is inhibited, there is no 6-phosphogluconate for step 3 to act on anyway. The cell achieves full regulatory control with a single feedback point, which is parsimonious and robust.

---

## Problem 4

**(a) Mode for a resting red blood cell under background oxidative stress:**

The resting red cell is running **Mode 4**: it needs NADPH and also needs to generate ATP. The oxidative phase runs to produce NADPH for glutathione regeneration and antioxidant defense. Ribulose-5-phosphate is not directed toward nucleotide synthesis (the cell has no nucleus and no active DNA replication); instead it passes through the non-oxidative phase, which converts it to fructose-6-phosphate and glyceraldehyde-3-phosphate. Those intermediates reenter glycolysis and are oxidized to pyruvate and then lactate (the red cell has no mitochondria, so all ATP generation is anaerobic), producing the ATP the cell needs to run Na⁺/K⁺-ATPase and maintain membrane integrity. Mode 4 layers NADPH generation on top of normal glucose catabolism: the same carbons that eventually yield ATP also generate NADPH on their way through the oxidative phase.

Mode 3, by contrast, is more appropriate under acute or severe oxidative stress, where NADPH demand is high enough that the cell intentionally recycles carbon back through gluconeogenesis to regenerate G6P and run the oxidative phase repeatedly, trading ATP production for maximal NADPH output.

**(b) Why Mode 1 requires the oxidative phase to be off:**

In Mode 1, the cell has abundant NADPH: the NADPH/NADP⁺ ratio is already high, meaning NADP⁺ is scarce. G6PD is product-inhibited by NADPH, so at high NADPH/NADP⁺ the enzyme is essentially off. It is not a matter of running the oxidative phase "at a lower rate" — product inhibition closes the valve. Even if a tiny amount of G6PD activity persisted, the high NADPH would immediately inhibit it further, making the oxidative phase a negligible source of Ru5P. The cell therefore cannot rely on the oxidative phase to supply pentoses and must make ribose-5-phosphate through the non-oxidative phase running in reverse, starting from glycolytic intermediates (F6P and G3P), which are available regardless of NADPH status.

**(c) Carbon flow in Mode 4:**

In Mode 4, the oxidative phase generates NADPH while the non-oxidative phase recycles the carbon skeletons back into glycolysis. Specifically: G6P enters the oxidative phase, loses one carbon as CO₂, and exits as ribulose-5-phosphate with two NADPH generated. Ribulose-5-phosphate passes through the non-oxidative phase and is converted to fructose-6-phosphate and glyceraldehyde-3-phosphate. Both intermediates reenter glycolysis directly and are oxidized through pyruvate, acetyl-CoA, the TCA cycle, and oxidative phosphorylation to produce ATP.

Compared to running glycolysis alone: Mode 4 produces 2 NADPH per G6P diverted through the oxidative phase, at the cost of one carbon lost as CO₂ (which can no longer contribute to ATP via the TCA cycle). The same glucose carbons that eventually produce ATP also generate NADPH on the way through. This is why Mode 4 is described as metabolically integrated: the PPP is not competing with glycolysis for G6P — it is prefixing a NADPH-generating step onto what is otherwise normal glucose catabolism.

---

## Problem 5

**(a) Biochemical sequence from divicine to Heinz body formation:**

Divicine and isouramil are direct oxidants that oxidize reduced glutathione (GSH) to oxidized glutathione (GSSG), consuming the cell's GSH pool directly. To regenerate GSH from GSSG, glutathione reductase must transfer two electrons from NADPH. In a G6PD-deficient red cell, NADPH cannot be replenished because G6PD, the only NADPH source in a mature erythrocyte, is functionally defective. GSSG accumulates, GSH falls, and the glutathione cycle cannot continue. Without GSH, glutathione peroxidase cannot neutralize the H₂O₂ that accumulates from normal metabolic oxygen exposure. H₂O₂ oxidizes hemoglobin: the ferrous iron in heme is oxidized to the ferric state (methemoglobin), and further oxidation generates ferryl hemoglobin, which denatures and precipitates inside the red cell. The precipitated hemoglobin aggregates form visible inclusions called Heinz bodies. Heinz body-containing cells are rigid and cannot deform to pass through the splenic sinusoids. The spleen physically strips the Heinz body-containing membrane segments from passing erythrocytes, producing the characteristic bite cell morphology. Eventually the cell membrane can no longer sustain integrity and lyses.

**(b) Why red cells are selectively vulnerable:**

Mature erythrocytes are uniquely defenseless because they have shed the equipment every other cell uses for backup NADPH production and antioxidant upregulation:

1. **No mitochondria.** Most nucleated cells can generate some NADPH in the mitochondrial matrix via isocitrate dehydrogenase (NADP⁺-linked) and the nicotinamide nucleotide transhydrogenase. Red cells have neither of these. They cannot run the TCA cycle at all.

2. **No nucleus.** Nucleated cells under oxidative stress upregulate the expression of antioxidant enzymes (catalase, superoxide dismutase, glutathione peroxidase, and G6PD itself via Nrf2 signaling) as a transcriptional response. Red cells cannot synthesize any new proteins. Whatever G6PD activity they have at maturation is all they will ever have — and if it is deficient, no stress response can correct it.

The G6PD-deficient person's nucleated cells tolerate fava bean exposure because they have these backup mechanisms. The red cell has no backup.

**(c) Why the sister has higher enzyme activity:**

G6PD is encoded on the X chromosome. The brother is hemizygous (one X, one defective G6PD allele): every cell he has expresses only the mutant enzyme, giving ~7% activity across all red cells. The sister is heterozygous (one functional allele, one defective allele on her two X chromosomes). In each somatic cell, X-inactivation silences one X chromosome randomly during early development. The result is that approximately half of her red cell precursors silenced the X carrying the defective allele and express only functional G6PD; the other half silenced the normal allele and express only defective G6PD. Her total population averages to roughly 50% activity (with individual variation depending on whether X-inactivation was exactly 50:50). Her 52% activity reflects a nearly equal split, consistent with heterozygosity and random inactivation. The cells with functional G6PD in her population provide enough total NADPH to prevent hemolysis at the oxidative dose from fava bean consumption.

---

## Problem 6

**(a) Balanced polymorphism:**

When a harmful allele persists at high frequency in a population over generations, it means the allele is not being purged by natural selection — or more precisely, it is being purged in carriers who express the disease, but simultaneously being enriched by selection in some other context. This is called **balanced polymorphism** (or heterozygote advantage). The necessary condition is that the fitness gain in the selective context (malaria survival) must equal or exceed the fitness loss from the disease state (hemolytic risk and occasional mortality), integrated across all individuals carrying the allele. Where malaria mortality before reproductive age is high — historically 20–25% childhood mortality in hyperendemic regions — even partial protection from malaria can exert strong enough selection to maintain an otherwise harmful allele at high equilibrium frequency.

**(b) Biochemical basis for parasite vulnerability:**

*Plasmodium falciparum* digests hemoglobin in a specialized acidic digestive vacuole and generates heme as a toxic byproduct, which it polymerizes into hemozoin for detoxification. This process generates significant oxidative stress within the parasite. The parasite manages that stress using the host red cell's reducing capacity: it imports glutathione and depends on the cell's NADPH supply to keep the oxidative environment manageable. In a G6PD-deficient red cell, the NADPH pool is low, GSH is partially oxidized, and the baseline oxidative environment is elevated. The parasite, which has evolved to inhabit cells with normal reducing capacity, is exposed to an oxidative stress it cannot fully compensate for. The parasite either fails to complete its erythrocytic developmental cycle or produces fewer merozoites, reducing the efficiency of infection.

**(c) Hypothesis for why heterozygous females are more protected than hemizygous males:**

X-inactivation in heterozygous females produces a mosaic red cell population: roughly half the cells have normal G6PD activity and half are G6PD-deficient. When *Plasmodium* infects red cells at random, it enters both normal and deficient cells. Parasites in the G6PD-deficient cells encounter high oxidative stress and are selectively impaired. The spleen preferentially destroys oxidatively damaged cells — including infected G6PD-deficient cells with parasites inside — clearing the infection more efficiently. Meanwhile, the cells with normal G6PD activity maintain systemic antioxidant capacity and prevent clinical hemolysis. The two populations work in concert: deficient cells are a trap for the parasite, and normal cells prevent the red cell population from collapsing.

In hemizygous males, all red cells are deficient. The parasite trap is still there, but when oxidative stress is high (from infection itself, immune response, or concomitant illness), there are no normal cells to maintain glutathione defense systemwide. The protection is real, but the accompanying vulnerability to hemolytic crises is also real. The heterozygous female's mosaic creates a more favorable balance: strong parasite clearance from deficient cells, systemic stability from normal cells. This hypothesis is consistent with the epidemiological observation that heterozygous females have the strongest survival advantage — not because they have more protection, but because they have the right combination of protection and stability.

---

## Problem 7

**(a) Three TPP-dependent enzymes:**

- **Pyruvate dehydrogenase (PDH):** Converts pyruvate to acetyl-CoA by oxidative decarboxylation, linking glycolysis to the TCA cycle and fatty acid synthesis. PDH is the gateway from glycolytic carbon into aerobic oxidative metabolism.

- **α-Ketoglutarate dehydrogenase (α-KGDH):** Catalyzes the oxidative decarboxylation of α-ketoglutarate to succinyl-CoA in step 4 of the TCA cycle, one of the key energy-yielding steps of the cycle. This is mechanistically analogous to PDH; both are multi-enzyme complexes with TPP as the decarboxylase cofactor.

- **Transketolase:** Transfers two-carbon units between sugar phosphates in the non-oxidative phase of the PPP, enabling interconversion of three-, four-, five-, six-, and seven-carbon intermediates. Without transketolase, the non-oxidative phase cannot run and the PPP cannot supply ribose-5-phosphate via Mode 1 or recycle ribulose-5-phosphate in Modes 3 and 4.

All three are impaired simultaneously in thiamine deficiency, blocking aerobic glucose catabolism at the glycolysis-TCA junction, inside the TCA cycle, and in the non-oxidative PPP.

**(b) Mechanistic explanation for why glucose worsens Wernicke's:**

Glucose administration increases glycolytic flux, generating more pyruvate. Pyruvate is normally converted to acetyl-CoA by PDH, which requires TPP. In a thiamine-depleted patient, the total TPP stores in all tissues are critically low; PDH has little TPP bound and is operating at residual capacity. The glucose-driven surge of pyruvate increases the demand on PDH at a moment when the cofactor supply cannot meet it. The residual TPP that was barely maintaining neuronal PDH activity is consumed rapidly as the enzyme is overwhelmed. Pyruvate accumulates and is shunted to lactate (producing lactic acidosis) or enters neurons where it cannot be processed. Neurons in the metabolically active regions of the mammillary bodies, thalamus, and periaqueductal gray are particularly affected because they operate at near-maximal aerobic metabolic rates with essentially no reserve. When PDH fails in these neurons, ATP production drops toward zero and cell death begins. The intervention that was intended to provide energy instead depletes the last cofactor protecting the neurons from energy failure. The correct protocol — thiamine before glucose in any malnourished or potentially thiamine-depleted patient — exists precisely to prevent this sequence.

**(c) Interpreting the transketolase assay results:**

**Patient A (19% without TPP → 91% with TPP):** Transketolase protein is present and structurally intact. The very low baseline activity reflects cofactor starvation: the enzyme exists in the cell, but most of its active-site TPP binding sites are empty because the cell lacks thiamine to synthesize sufficient TPP. When TPP is added directly to the assay, it saturates the empty binding sites and restores activity to near-normal levels. This pattern — low baseline activity with large restoration on TPP addition — is the diagnostic signature of thiamine deficiency. The "TPP effect" (the percent increase in activity on adding TPP) is the clinically used metric, and a substantial TPP effect confirms that the limitation is cofactor availability, not enzyme absence or structural damage.

**Patient B (58% without TPP → 61% with TPP):** Baseline activity is reduced, but adding TPP does not rescue it. The 3-point increase is within assay noise, not a significant TPP effect. This pattern suggests the enzyme is already as TPP-saturated as it is going to be, and the limitation is something other than cofactor supply: the enzyme protein may be reduced in amount (low expression, accelerated degradation), or there may be a mutation or post-translational modification reducing catalytic efficiency. This is not a pattern of thiamine deficiency. Treating this patient with thiamine would not correct the enzyme deficit.

---

## Problem 8

**(a) Normal function of NADPH in red blood cells versus neutrophils:**

These are opposite functions.

In **red blood cells**, NADPH is used for **antioxidant defense**. NADPH donates electrons to glutathione reductase, regenerating reduced glutathione (GSH) from GSSG. GSH is the substrate for glutathione peroxidase, which neutralizes H₂O₂ and lipid peroxides. NADPH also reduces thioredoxin and other antioxidant intermediates. The purpose is to protect the cell from oxidative damage — NADPH is a reducing agent deployed against reactive oxygen species.

In **neutrophils**, NADPH is used for **intentional ROS generation**. NADPH oxidase (NOX2) catalyzes the reaction:

$$\text{NADPH} + 2\text{O}_2 \rightarrow \text{NADP}^+ + \text{H}^+ + 2\text{O}_2^{\bullet-}$$

The superoxide produced dismutates to H₂O₂ and generates further reactive species (hypochlorous acid via myeloperoxidase) in the phagolysosome, killing ingested bacteria. NADPH is a pro-oxidant substrate here — the cell uses it to make the very reactive oxygen species that red cells use NADPH to neutralize.

**(b) Vulnerability of each patient:**

**Patient A (G6PD deficiency):** G6PD is the sole NADPH source in mature red cells. When oxidative stress (drug, infection, fava beans) demands accelerated GSH regeneration, NADPH cannot be resupplied. GSH falls, GSSG accumulates, H₂O₂ and lipid peroxides accumulate, hemoglobin denatures into Heinz bodies, and cells are destroyed by the spleen. The vulnerability is hemolytic anemia because the antioxidant function of NADPH is lost in the one cell type that has no backup.

**Patient B (CGD):** NADPH is produced normally from the PPP, but NOX2 cannot use it to reduce O₂. When a neutrophil engulfs a bacterium, the respiratory burst — the primary microbicidal mechanism — cannot fire. Bacteria survive inside phagolysosomes. Catalase-positive organisms are especially dangerous because they destroy H₂O₂ from the small amounts produced by other mechanisms, removing even the limited residual microbicidal activity. The patient suffers recurrent, deep-seated infections with organisms like *S. aureus*, *Aspergillus*, *Serratia*, and *Burkholderia* that catalase-negative organisms could not sustain.

**(c) Why antioxidant supplementation is misguided for CGD:**

The researcher has diagnosed a problem in the antioxidant arm of NADPH metabolism and proposed an antioxidant solution. But CGD is not an antioxidant deficiency. The neutrophil's problem is that it cannot generate enough superoxide in the phagosome. Providing N-acetylcysteine boosts glutathione levels, which would help a cell struggling to neutralize reactive oxygen species — this is relevant to G6PD deficiency in red cells, not to CGD.

In CGD neutrophils, boosting glutathione would either do nothing (if NOX2 produces no ROS to neutralize) or actively worsen the situation (if trace ROS from other sources in the phagosome are being further quenched by the additional antioxidant, removing any residual microbicidal activity). The intervention treats the correct molecule (NADPH-linked chemistry) but in the wrong direction. G6PD deficiency needs more antioxidant capacity in red cells; CGD needs more pro-oxidant capacity in phagosomes. Confusing these reflects the error of treating "NADPH biology" as monolithic rather than recognizing that NADPH's downstream consequences depend entirely on which enzyme uses it.
