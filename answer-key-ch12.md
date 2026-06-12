# Answer Key — Chapter 12: Electron Transport Chain and Oxidative Phosphorylation

---

## Problem 1

**The path of NADH electrons:**

$\text{NADH}$ is oxidized at Complex I, which transfers the two electrons through a chain of iron-sulfur clusters to ubiquinone, reducing it to $\text{QH}_2$ ($\text{CoQ}$ in the membrane). The energy released drives pumping of **4 protons** from matrix to IMS. $\text{QH}_2$ then carries electrons to Complex III, which runs the Q cycle: for every two electrons that exit toward cytochrome c, **4 protons** are released into the IMS. Cytochrome c delivers electrons one at a time to Complex IV, which reduces $\text{O}_2$ to $\text{H}_2\text{O}$ and pumps **4 protons** per $\text{O}_2$ reduced (2 per electron pair). Total protons per NADH: $4 + 4 + 2 = \mathbf{10 \text{ H}^+}$.

**The path of $\text{FADH}_2$ electrons:**

$\text{FADH}_2$ (from succinate oxidation at Complex II, or from other FAD-linked reactions) donates electrons directly to the CoQ pool via Complex II. Complex II does not pump any protons; it is simply a conduit from $\text{FADH}_2$ to $\text{QH}_2$. The $\text{QH}_2$ produced is identical to the $\text{QH}_2$ produced by Complex I, and from this point the path is the same: Complex III (4 $\text{H}^+$), Complex IV (2 $\text{H}^+$). Total protons per $\text{FADH}_2$: $0 + 4 + 2 = \mathbf{6 \text{ H}^+}$.

**Why the yields differ:**

$\text{FADH}_2$ electrons enter the chain at CoQ, after Complex I, and therefore skip Complex I's 4-proton contribution entirely. With approximately 4 $\text{H}^+$ required per $\text{ATP}$ (including transport costs via ANT and PiC):

$$\text{NADH: } \frac{10 \text{ H}^+}{4 \text{ H}^+/\text{ATP}} = 2.5 \text{ ATP}$$

$$\text{FADH}_2\text{: } \frac{6 \text{ H}^+}{4 \text{ H}^+/\text{ATP}} = 1.5 \text{ ATP}$$

The 1 $\text{ATP}$ difference per molecule reflects the bypass of Complex I's 4-proton pump: 4 fewer $\text{H}^+$ pumped ÷ 4 $\text{H}^+$ per $\text{ATP}$ = exactly 1 fewer $\text{ATP}$. This is not a consequence of $\text{FADH}_2$ being a weaker reductant (though it is, with $E^{\circ'} \approx 0$ V vs. $-0.32$ V for $\text{NADH}$); it is a consequence of where its electrons enter the chain. All $\text{QH}_2$ molecules are equivalent once they are in the membrane, regardless of which dehydrogenase produced them.

---

## Problem 2

**(a) CoQ pool oxidation state:**

Qblock at the Qi site prevents the second electron from each Q cycle from being used to reduce semiquinone ($\text{Q}^{\bullet-}$) back to $\text{QH}_2$ in the matrix. Complex III still accepts $\text{QH}_2$ at the Qo site (the drug is at the Qi site, not the Qo site), but it cannot complete the Q cycle. Over time, the cycle stalls because semiquinone radicals accumulate at the Qo site (they cannot be resolved). The ability of Complex III to oxidize $\text{QH}_2$ is severely impaired. Meanwhile, Complex II continues to produce $\text{QH}_2$ from succinate. With input continuing and output blocked, the CoQ pool becomes **more reduced** (shifts toward $\text{QH}_2$).

**(b) Downstream effects:**

- **Cytochrome c reduction state:** Since Complex III cannot efficiently transfer electrons to cytochrome c when the Q cycle is blocked, cytochrome c will remain mostly **oxidized** ($\text{Fe}^{3+}$). Electrons are backed up at the CoQ level; they are not reaching cytochrome c at normal rates.
- **PMF:** With electron flow through Complex III stalled, Complexes III and IV stop (or greatly reduce) proton pumping. Complex I is also backed up because $\text{QH}_2$ cannot be reoxidized (in a NADH-supplied preparation; here succinate/Complex II still feeds $\text{QH}_2$). Proton pumping slows dramatically. The PMF will **fall** as existing gradient drains through ATP synthase without being replenished.
- **ATP production:** The falling PMF means ATP synthase has less driving force. ATP production **drops substantially**, approaching zero as the gradient collapses.

**(c) Effect of adding FCCP:**

FCCP collapses the PMF by providing an alternate proton path back into the matrix. However, the primary problem here is not back-pressure from the PMF; it is that Complex III is blocked and cannot reoxidize $\text{QH}_2$ to regenerate CoQ. Even after FCCP removes the gradient (eliminating back-pressure), Complex III still cannot complete the Q cycle. Complex II continues feeding $\text{QH}_2$ but there is nowhere for the electrons to go. $\text{O}_2$ consumption will therefore rise **only modestly or minimally**, because the bottleneck is not the PMF — it is the blocked Complex III. This distinguishes a chain block from an ATP synthase block: adding FCCP to oligomycin-treated mitochondria restores O₂ consumption fully, because the chain itself is intact. Adding FCCP to Qblock-treated mitochondria does not, because the electron carrier pathway is severed.

**(d) ROS production:**

Yes, Qblock would substantially increase ROS production at Complex III. When the Qi site is blocked, the semiquinone radical ($\text{Q}^{\bullet-}$) that forms at the Qo site from the first electron of each $\text{QH}_2$ oxidation cannot be resolved by the Q cycle. This semiquinone accumulates at the Qo site. Semiquinone is a highly reactive radical that donates its electron directly to dissolved $\text{O}_2$ rather than continuing down the cytochrome b chain:

$$\text{Q}^{\bullet-} + \text{O}_2 \rightarrow \text{CoQ} + \text{O}_2^{\bullet-}$$

The product, superoxide ($\text{O}_2^{\bullet-}$), is the primary reactive oxygen species. This is the same mechanism by which antimycin A converts Complex III from an electron transport enzyme into a superoxide generator. The Qi block does not just impair ATP synthesis; it converts a fraction of the electron flow into oxidative stress.

---

## Problem 3

**(a) Calculating the PMF:**

At $T = 310 \text{ K}$:

$$\frac{2.303 RT}{F} = \frac{2.303 \times 8.314 \text{ J mol}^{-1}\text{K}^{-1} \times 310 \text{ K}}{96{,}485 \text{ C/mol}}$$

$$= \frac{2.303 \times 2577.3 \text{ J/mol}}{96{,}485 \text{ C/mol}} = \frac{5935 \text{ J/mol}}{96{,}485 \text{ C/mol}} \approx 0.06151 \text{ V} = 61.5 \text{ mV}$$

Note: the sign convention in the PMF equation uses $\Delta V$ as the electrical potential across the membrane (with matrix-negative convention). The chapter states $\Delta V \approx -180 \text{ mV}$ (matrix negative). Here $\Delta V = -150 \text{ mV}$ and $\Delta\text{pH} = +1.0$ (matrix more basic, so $\text{pH}_\text{mat} - \text{pH}_\text{ims} = +1.0$). Substituting:

$$\Delta p = \Delta V - \frac{2.303 RT}{F}\Delta\text{pH} = -150 \text{ mV} - (61.5 \text{ mV})(1.0)$$

$$\Delta p = -150 - 61.5 = \mathbf{-211.5 \text{ mV}} \approx -212 \text{ mV}$$

The negative sign indicates that proton transit from IMS to matrix is thermodynamically favorable (downhill for positive charges moving from positive to negative side).

**(b) Free energy per mole of protons:**

$$\Delta G = F \cdot |\Delta p| = 96{,}485 \text{ C/mol} \times 0.2115 \text{ V} = 20{,}407 \text{ J/mol} \approx \mathbf{20.4 \text{ kJ/mol}}$$

Each mole of protons flowing down this gradient releases approximately 20.4 kJ.

**(c) Energy available per ATP vs. the cost of synthesis:**

With an 8-subunit c-ring and 3 ATP per rotation:
- Protons per rotation: 8
- Energy per proton: 20.4 kJ/mol
- Total energy per rotation: $8 \times 20.4 = 163.2 \text{ kJ/mol}$
- Energy per ATP: $\frac{163.2}{3} \approx \mathbf{54.4 \text{ kJ/mol per ATP}}$

The standard free energy of ATP synthesis ($\Delta G^{\circ'}$ for the reverse of hydrolysis) is $+30.5 \text{ kJ/mol}$. The 54.4 kJ/mol available from proton transit — even at this lower-than-typical PMF — substantially exceeds the thermodynamic cost of ATP synthesis. The surplus is the thermodynamic driving force: the system does not run near the edge of equilibrium; the PMF provides a comfortable free energy excess that makes synthesis highly favorable. Under physiological conditions where the actual cellular $\Delta G$ for ATP synthesis is closer to $+50 \text{ kJ/mol}$ (due to far-from-standard $\text{ATP}$/$\text{ADP}$/$P_i$ concentrations), the margin is tighter, which is why the PMF must be maintained well above minimum levels to drive synthesis efficiently.

---

## Problem 4

**(a) Why is the L:P ratio elevated in Complex I deficiency?**

Complex I is the entry point for $\text{NADH}$ into the electron transport chain. With 90% of Complex I non-functional, the matrix's capacity to reoxidize $\text{NADH}$ to $\text{NAD}^+$ is severely curtailed. $\text{NADH}$ accumulates in the mitochondrial matrix, driving up the $\text{NADH}/\text{NAD}^+$ ratio.

This matters for pyruvate in two ways. First, pyruvate dehydrogenase (PDH) is inhibited by the high $\text{NADH}/\text{NAD}^+$ ratio (PDH kinase is activated by elevated NADH and acetyl-CoA, phosphorylating and inactivating PDH). Pyruvate cannot be converted to acetyl-CoA efficiently. Second, and more directly: the high cytoplasmic $\text{NADH}/\text{NAD}^+$ ratio (which reflects the mitochondrial state via shuttle exchange) drives the lactate dehydrogenase equilibrium far toward lactate formation:

$$\text{Pyruvate} + \text{NADH} + \text{H}^+ \rightleftharpoons \text{Lactate} + \text{NAD}^+$$

Because lactate dehydrogenase is near equilibrium in the cell, the ratio $[\text{Lactate}]/[\text{Pyruvate}]$ is directly proportional to $[\text{NADH}]/[\text{NAD}^+]$. A very high L:P ratio (>25 is considered consistent with ETC defects; >30–35 is strongly suggestive) reflects a severely elevated $\text{NADH}/\text{NAD}^+$ ratio, which in turn indicates impaired ETC reoxidation of $\text{NADH}$ — exactly what Complex I deficiency causes.

**(b) Why are the basal ganglia and brainstem selectively vulnerable?**

Neurons in the basal ganglia and brainstem share two properties that make them exquisitely sensitive to ETC failure:

1. **High and continuous ATP demand.** These structures are tonically active, require sustained ion gradients ($\text{Na}^+$/$\text{K}^+$-ATPase, $\text{Ca}^{2+}$ pumps), and have no ability to downregulate their activity to conserve energy the way less-critical tissues can.

2. **Near-exclusive dependence on oxidative phosphorylation.** Neurons store essentially no glycogen and have a high respiratory quotient approaching 1.0 for glucose oxidation. They rely on the ETC to reoxidize the $\text{NADH}$ produced from both glycolysis and the TCA cycle. When ETC capacity is 90% reduced, glycolysis can proceed only as fast as its limited anaerobic capacity allows ($\text{NADH} \rightarrow \text{Lactate}$), which is orders of magnitude less ATP than these neurons require.

The bilateral symmetry of the lesions reflects the fact that both structures receive equivalent metabolic stress — it is a global ETC defect, not a focal one.

**(c) Normal at birth, deteriorating later: heteroplasmy and threshold effects:**

The child has 90% mutant mtDNA in most tissues. The key is the concept of a **threshold**: below a certain fraction of mutant mtDNA, the remaining wild-type copies produce enough functional Complex I to sustain normal ATP output. Above the threshold, function falls below the minimum required for cell survival, and disease appears.

At birth, multiple additional factors compensate temporarily. Cells can have thousands of mitochondria, and early in development mitochondrial turnover (fission, fusion, mitophagy) may partially redistribute wild-type copies. The metabolic demands of a newborn's brain, while high, are somewhat lower than those of an 18-month-old who is actively myelinating, wiring synaptic connections, and sustaining increasing neurological activity. As metabolic demands ramp up with development, the partially compensated ETC can no longer keep pace, and cells cross below the ATP-generation threshold needed for survival. The heteroplasmy fraction can also shift over time through replication drift, potentially increasing the mutant burden in high-demand tissues and accelerating disease onset.

**(d) Prognosis for the 5-year-old sibling:**

The most accurate answer is: **uncertain, but the risk is real.** The key concepts are threshold effects and heteroplasmy drift.

At 55% mutant mtDNA, the sibling may currently be below the threshold in most critical tissues, which explains the absence of symptoms. However, heteroplasmy is not stable — the mutant fraction can increase or decrease over time through stochastic segregation of mitochondria during cell division. If the mutant fraction drifts upward in neurons, cardiomyocytes, or other high-demand cells, the sibling could eventually cross the disease threshold. Alternatively, the fraction could drift downward, reducing risk further. The concept illustrated is the **threshold effect of heteroplasmy**: disease severity and timing are not determined by genotype alone but by the dynamic balance of mutant versus wild-type mitochondrial genomes within each cell, which can change throughout life.

---

## Problem 5

**(a) Mechanism of action:**

The compound is an **uncoupler** — specifically, a lipid-soluble weak acid that acts as a proton shuttle across the inner mitochondrial membrane, bypassing ATP synthase. The classical compound it resembles is **2,4-dinitrophenol (DNP)**, used disastrously as a weight-loss drug in the 1930s. (FCCP is another well-known pharmacological uncoupler of the same class.)

**(b) Why does $\text{O}_2$ consumption double?**

Under normal coupled conditions, the proton gradient acts as **back-pressure** on the respiratory complexes. As the PMF builds, it becomes thermodynamically harder for Complexes I, III, and IV to pump more protons against it — so the chain slows. This is respiratory control: the rate of electron transport is governed by how quickly ATP synthase drains the gradient.

When the uncoupler collapses the PMF by ferrying protons back into the matrix, that back-pressure is eliminated. The respiratory complexes can now pump protons downhill at their maximum kinetic rate, because there is no gradient resisting them. $\text{NADH}$ is consumed rapidly, the TCA cycle and other upstream pathways are stimulated to replenish it, and $\text{O}_2$ (the terminal electron acceptor at Complex IV) is consumed correspondingly faster. The doubling of $\text{O}_2$ consumption reflects the chain running near its maximum uninhibited rate.

**(c) Why titrating the dose cannot make this safe:**

The critical difference is **regulatory control**. UCP1 in brown adipose tissue is subject to tight allosteric regulation: free fatty acids activate it, and purine nucleotides (ATP, ADP, GTP) inhibit it. The sympathetic nervous system controls UCP1 activity through norepinephrine, cAMP, and PKA. When thermogenesis is no longer needed, signaling terminates, UCP1 is inhibited, and the gradient is allowed to rebuild. The system has a thermostat.

A small-molecule lipid-soluble proton shuttle like DNP has **no thermostat**. Its rate of proton shuttling depends only on its membrane concentration and the PMF magnitude; higher PMF drives faster proton shuttling, which generates more heat, which raises the metabolic rate further. There is no molecular mechanism for the body to tell the compound to stop. Even at a "safe" initial dose, as the compound drives up metabolic rate and heat production, any residual drug in the membrane continues to act. Core body temperature rises, metabolic demand increases, more fuel is burned to meet ATP needs (which are never fully met, since ATP synthesis is impaired), generating more heat still. This is a positive feedback loop with no intrinsic limit. There is no dose at which the effect becomes self-limiting in the way that UCP1 is self-limiting.

**(d) Fate of free energy in coupled vs. uncoupled cells:**

In normally coupled cells: the free energy from $\text{NADH}$ oxidation ($\Delta G^{\circ'} \approx -220 \text{ kJ/mol}$ from $\text{NADH}$ to $\text{O}_2$) is stored as a proton electrochemical gradient, and approximately 60–70% of that energy is captured as ATP (the remainder is dissipated as heat, as no energy conversion is 100% efficient).

In uncoupler-treated cells: the same electron transport chemistry occurs, and the same protons are pumped across the membrane, but those protons immediately return through the uncoupler without doing work. The free energy of the proton gradient that would have driven ATP synthesis is **dissipated entirely as heat**. The cell burns fuel at an accelerated rate and produces only heat, not chemical potential energy. ATP levels fall because consumption (all the normal ATPase reactions) continues while synthesis stops, and the cell eventually dies from a combination of energy failure and hyperthermia.

---

## Problem 6

**(a) Shuttle system in each tissue:**

- **Hepatocytes (liver):** The **malate-aspartate shuttle** is the primary route. The liver expresses high levels of the required transaminases (GOT1 and GOT2), the malate-dehydrogenase isoforms, and the necessary membrane carriers (malate-α-ketoglutarate antiporter, glutamate-aspartate carrier). The liver does not experience the extreme NADH surges that fast-twitch muscle does, so the reversibility of the shuttle is not a practical problem.

- **Fast-twitch skeletal muscle:** The **glycerol-3-phosphate shuttle** is used. Fast-twitch muscle can generate NADH from glycolysis far faster than any other tissue — during a sprint, glycolytic flux is enormous. The glycerol-3-phosphate shuttle is irreversible (the membrane-associated FAD-linked glycerol-3-phosphate dehydrogenase on the outer face of the IMM is a one-way reaction) and can therefore handle NADH surges without running backward. It is also mechanistically simpler, requiring only two enzymes.

**(b) GOT2 mutation: which shuttle fails and which takes over:**

Aspartate aminotransferase (GOT2) is the mitochondrial matrix isoform of the enzyme that interconverts aspartate and oxaloacetate (OAA) using glutamate and α-ketoglutarate. It is essential for the malate-aspartate shuttle: inside the matrix, OAA cannot be transported directly across the membrane, so it is transaminated to aspartate (by GOT2) for export. Without GOT2, OAA cannot be converted to aspartate in the matrix, the cycle cannot complete, and the **malate-aspartate shuttle fails**.

The liver would be forced to rely on the **glycerol-3-phosphate shuttle** instead. Each cytoplasmic NADH would then yield only 1.5 ATP (entering as $\text{FADH}_2$ equivalents) rather than 2.5 ATP. Per glucose, the two cytoplasmic NADH from glycolysis would yield: $2 \times 1.5 = 3 \text{ ATP}$ instead of $2 \times 2.5 = 5 \text{ ATP}$.

**(c) ATP yield comparison:**

Recall the full per-glucose accounting (using only the mitochondrial $\text{NADH}$ and $\text{FADH}_2$ for this comparison):

| Component | Normal (MA shuttle) | GOT2-deficient (G3P shuttle) |
|---|---|---|
| 8 mitochondrial NADH | $8 \times 2.5 = 20$ ATP | $8 \times 2.5 = 20$ ATP |
| 2 $\text{FADH}_2$ | $2 \times 1.5 = 3$ ATP | $2 \times 1.5 = 3$ ATP |
| 4 direct ATP/GTP | 4 ATP | 4 ATP |
| 2 cytoplasmic NADH | $2 \times 2.5 = 5$ ATP | $2 \times 1.5 = 3$ ATP |
| **Total** | **32 ATP** | **30 ATP** |

The ATP cost of the GOT2 mutation is **2 ATP per glucose** — exactly the penalty for using the lower-yield shuttle for the 2 cytoplasmic NADH.

**(d) Why the glycerol-3-phosphate shuttle is preferred under burst conditions:**

The glycerol-3-phosphate shuttle is **irreversible**. Once glycerol-3-phosphate is oxidized by the FAD-linked glycerol-3-phosphate dehydrogenase on the outer face of the IMM, the electrons enter the CoQ pool and cannot come back. This means the shuttle always moves reducing equivalents into the mitochondria regardless of the concentration gradients of its intermediates.

The malate-aspartate shuttle, by contrast, runs on the gradients of malate, aspartate, glutamate, and OAA. Under extreme glycolytic flux, cytoplasmic NADH rises sharply and the amino acid intermediate gradients can reverse, causing the shuttle to run backward and export reducing equivalents from the mitochondria — the opposite of what is needed. For fast-twitch muscle that needs to sustain glycolytic bursts without the shuttle working against it, the guaranteed unidirectionality of the glycerol-3-phosphate shuttle is worth the 1 ATP per cytoplasmic NADH penalty.

---

## Problem 7

**(a) Which preparation drops $\text{O}_2$ consumption more sharply?**

**Preparation B (cyanide)** drops more sharply.

- In **Preparation A (oligomycin):** ATP synthase is blocked, so protons cannot return through $\text{F}_0$. The PMF rises as pumping continues without any proton outlet. As the gradient builds, it exerts increasing back-pressure on Complexes I, III, and IV, progressively slowing them. $\text{O}_2$ consumption falls, but not to zero immediately — the chain slows to the rate at which the gradient equilibrates with the maximum pumping capacity. A small, residual electron flow may continue.

- In **Preparation B (cyanide):** Complex IV is directly blocked; electrons cannot be transferred to $\text{O}_2$ at all. Since $\text{O}_2$ is the terminal acceptor and its reduction is the step where electrons actually leave the chain, blocking it stops all electron flow. $\text{O}_2$ consumption drops essentially to zero immediately. There is no electron "seepage" around a blocked terminal acceptor.

**(b) PMF: which rises, which falls?**

- **Preparation A (oligomycin):** PMF **rises**. Proton pumping continues (electrons still flow briefly; even as the chain slows, it still pumps against a gradient that has not yet reached equilibrium), while proton re-entry through ATP synthase is blocked. Protons accumulate in the IMS. The gradient grows until it equilibrates with pumping capacity.

- **Preparation B (cyanide):** PMF **falls**. With the chain stopped, no new protons are pumped. ATP synthase continues to consume the existing gradient (as long as ADP is present), draining it. Over time, the PMF collapses toward zero as protons return through synthase without being replenished.

**(c) Evaluating the student's reasoning:**

The conclusion — that $\text{ATP}$ synthesis requires electron transport — is **correct**. The logic used to reach it is **flawed**.

The student argues from the observation that blocking either intervention abolishes ATP. But this does not establish that electron transport is required for ATP synthesis in a mechanistic sense. The real mechanistic connection is indirect: electron transport builds the PMF, and ATP synthase uses the PMF to synthesize ATP. Neither result in isolation proves this linkage. What the two experiments together actually demonstrate is that the chain and the synthase are connected through the proton gradient. The better conclusion from these experiments is: ATP synthesis requires a proton gradient, and the chain is the device that builds it. Blocking the chain (Preparation B) eliminates the source of the gradient; blocking the synthase (Preparation A) builds the gradient without converting it to ATP. The student's conclusion is right but arrived at with reasoning that does not account for the intermediate role of the PMF — and that matters, because it leaves open the erroneous interpretation that the chain directly phosphorylates ADP (the pre-Mitchell view).

**(d) Adding FCCP to each preparation:**

- **Preparation A (oligomycin + FCCP):** $\text{O}_2$ consumption **rises sharply**. FCCP collapses the PMF that had been building due to the oligomycin block. With the back-pressure eliminated, the respiratory complexes (which are structurally intact) can now pump protons downhill at their maximum rate. Electron transport accelerates, and O₂ consumption rises substantially — to near-maximal rates. ATP production remains near zero (oligomycin still blocks the $\text{F}_0$ channel, and the PMF is continuously drained by FCCP before it can drive synthesis).

- **Preparation B (cyanide + FCCP):** $\text{O}_2$ consumption **does not rise** (remains near zero). FCCP provides an alternate proton path, but the constraint here is not back-pressure — it is that Complex IV is blocked and electrons cannot reach $\text{O}_2$ at all. Collapsing the PMF cannot restore electron flow to a chain whose terminal step is irreversibly blocked. The two responses differ because the underlying bottlenecks differ: Preparation A is constrained thermodynamically (back-pressure), while Preparation B is constrained kinetically/mechanistically (no functional terminal acceptor).
