# Chapter 9: Thermodynamic Principles II — The Cell's Energy Currency

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. NAD+ gains electrons during glycolysis to become NADH. Why does that matter? Where do those electrons go eventually, and what does the cell get out of it?

2. ATP sits in the middle of the cell's phosphate energy hierarchy, not at the top. Why is it the universal currency if there are more energetically favorable compounds available?

---

## The Big Picture

Chapter 1 gave you the thermodynamic framework. You know that cells run on free energy, that reactions couple together through shared intermediates, and that ATP hydrolysis drives an enormous amount of cellular work. 

Now we need to get more specific, because "the cell uses free energy" is about as useful as "the economy runs on money." True, but not actionable. 

What we're building in this chapter is a working picture of *how* the cell actually handles energy at the molecular level: which molecules carry it, how it gets transferred, and what kinds of reactions move it around. Once you have this toolkit, metabolic pathways stop looking like lists of reactions to memorize and start looking like what they actually are: carefully engineered sequences of energy transfers with a clear thermodynamic logic.

Three things to walk away with:

1. Electron transfer is another form of energy transfer, and the cell exploits it constantly.
2. A small set of carrier molecules handles almost all energy transactions in the cell.
3. Every reaction in a metabolic pathway fits into one of a handful of types, and once you recognize the type, you can reason about the energetics.

> **Clinical preview:** Metformin, the most commonly prescribed drug for type 2 diabetes, works at least partly by interfering with Complex I of the mitochondrial electron transport chain. That changes the cell's NADH/NAD+ ratio, which ripples through glucose metabolism and ultimately lowers blood glucose. We'll come back to this mechanism once you know what NADH actually does and why its ratio to NAD+ matters.

---

## Part I: Redox Chemistry

### What Oxidation and Reduction Actually Mean

You've probably heard "OIL RIG" — oxidation is loss, reduction is gain (of electrons). That's correct as far as it goes, but it's worth slowing down and understanding why electron transfer matters in a biological context, because it's not immediately obvious why moving electrons around should release useful energy.

Here's the key insight: electrons don't all have the same energy. An electron sitting on a carbon atom in glucose has more potential energy than an electron sitting on an oxygen atom in water. This isn't arbitrary; it reflects how strongly different atoms hold onto electrons. Oxygen is extremely electronegative, meaning it attracts electrons strongly. Carbon is much less so. When you oxidize glucose completely to CO₂ and H₂O, you're essentially moving electrons from a low-affinity environment (carbon) to a high-affinity environment (oxygen). Electrons move to where they're held more tightly, and the energy difference is released.

This is exactly analogous to gravitational potential energy. A ball at the top of a hill has more potential energy than at the bottom; it rolls downhill and releases energy. Electrons "roll" from atoms that hold them loosely to atoms that hold them tightly, and the energy difference is what the cell captures.

In biological systems, oxidation and reduction almost always involve the transfer of both electrons and protons together, because carbon-hydrogen bonds are what actually get broken. When you oxidize a carbon compound, you remove H atoms from it. Each H atom is one proton and one electron. The carrier molecules that accept them — primarily NAD+ and FAD — receive both. So in practice you'll see reactions written as:

$$\text{substrate} + \text{NAD}^+ \rightarrow \text{oxidized substrate} + \text{NADH} + \text{H}^+$$

The NADH picks up a hydride ion (H⁻, one proton plus two electrons), and a proton is released to solution. This is a reduction of NAD+. The substrate loses the equivalent and is oxidized. Two sides of the same transaction.

### Reduction Potentials

How do we quantify how much an atom or molecule "wants" electrons? Through the **standard reduction potential**, written $E^{\circ'}$ (in volts), measured at biochemical standard conditions (pH 7, 25°C, 1 M concentrations).

The convention: a high (more positive) $E^{\circ'}$ means a molecule has a strong tendency to *accept* electrons, to be reduced. A low (more negative) $E^{\circ'}$ means a molecule tends to *donate* electrons, to be oxidized.

Electrons flow spontaneously from low $E^{\circ'}$ to high $E^{\circ'}$, for the same reason water flows downhill. Here are some biologically important values:

| Half-reaction | $E^{\circ'}$ (V) |
|---|---|
| $\frac{1}{2}O_2 + 2H^+ + 2e^- \rightarrow H_2O$ | +0.82 |
| Fumarate + 2H⁺ + 2e⁻ → Succinate | +0.03 |
| $\text{NAD}^+ + \text{H}^+ + 2e^- \rightarrow \text{NADH}$ | −0.32 |
| $\text{NADP}^+ + \text{H}^+ + 2e^- \rightarrow \text{NADPH}$ | −0.32 |

Oxygen has the highest reduction potential in this list — it strongly wants electrons. NADH has a low (negative) reduction potential — it's a good electron donor. So when NADH eventually passes its electrons to oxygen via the electron transport chain, those electrons fall from −0.32 V all the way to +0.82 V. That's a big drop, and the energy released is substantial.

We can calculate exactly how substantial using the relationship between reduction potential and free energy:

$$\Delta G^{\circ'} = -nF\Delta E^{\circ'}$$

where:
- $n$ = number of electrons transferred
- $F$ = Faraday's constant = 96.5 kJ/V·mol (sometimes written 96,485 J/V·mol)
- $\Delta E^{\circ'} = E^{\circ'}_{\text{acceptor}} - E^{\circ'}_{\text{donor}}$

For NADH passing two electrons to oxygen:

$$\Delta E^{\circ'} = +0.82 - (-0.32) = +1.14 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(1.14) = -220 \text{ kJ/mol}$$

That's a lot of free energy released per NADH oxidized — about seven times the free energy of ATP hydrolysis. The electron transport chain captures a fraction of this energy to synthesize ATP. The rest is released as heat, which is part of how you maintain body temperature.

The sign of $\Delta G^{\circ'}$ follows directly from the sign of $\Delta E^{\circ'}$: if $\Delta E^{\circ'}$ is positive (electrons flow from lower to higher reduction potential), $\Delta G^{\circ'}$ is negative and the reaction is spontaneous. If $\Delta E^{\circ'}$ is negative (electrons would have to flow "uphill"), $\Delta G^{\circ'}$ is positive and you'd need to drive the reaction with an input of energy. Just like with any other coupled reaction.

### Where Redox Fits in Metabolism

Nearly every catabolic pathway involves oxidation of carbon compounds, and the electrons from that oxidation have to go somewhere. In aerobic metabolism, they ultimately go to oxygen. But cells don't transfer electrons directly from glucose to oxygen in one step; that would release all the energy as heat at once, uncontrollable and uncapturable. Instead, the electrons are picked up by carrier molecules (NADH, FADH₂) and delivered to the electron transport chain in a controlled sequence that allows the energy to be captured incrementally as ATP.

So when you see a step in glycolysis or the TCA cycle labeled "oxidation," what's actually happening is: a carbon compound loses electrons and protons to NAD+ or FAD, converting them to NADH or FADH₂. Those carriers then carry the electrons to the inner mitochondrial membrane, where the electron transport chain passes them through a series of protein complexes and ultimately to oxygen. The free energy released along the way drives the synthesis of ATP.

The pathway is essentially a wire connecting fuel molecules to oxygen, with the cell tapping the energy at controlled points along the wire.

---

## Part II: The Activated Carrier Toolkit

The cell handles energy in the form of specific molecular carriers. There are only a handful of them, but they carry almost all of the cell's energy transactions. Think of them as denominations of cellular currency, each useful for different kinds of purchases.

### ATP: The Universal Phosphoryl Donor

You already know ATP from Chapter 1. The quick recap for this context: ATP hydrolysis to ADP + Pᵢ releases about −30.5 kJ/mol under standard conditions and about −50 to −60 kJ/mol under cellular conditions. This free energy is used to drive reactions that wouldn't otherwise go.

The mechanism is almost always direct phosphoryl transfer: the enzyme moves the phosphate group from ATP to the substrate rather than hydrolyzing ATP in solution first and hoping the energy somehow carries over. Chapter 1 covered why the shared intermediate (the phosphorylated substrate) is what makes the coupling thermodynamically legitimate.

One thing to add here: there are two kinds of ATP hydrolysis worth distinguishing. Sometimes ATP loses just the terminal phosphate (producing ADP + Pᵢ). Other times ATP loses a pyrophosphate group — the two terminal phosphates together — producing AMP + PPᵢ. The pyrophosphate (PPᵢ) is then rapidly hydrolyzed by pyrophosphatase to 2 Pᵢ. Because pyrophosphatase essentially makes the PPᵢ hydrolysis irreversible, this gives an even larger thermodynamic driving force than the ADP pathway. Fatty acid activation (attaching a fatty acid to CoA before oxidation) uses this trick.

### NAD+/NADH: The Catabolic Electron Carrier

NAD+ (nicotinamide adenine dinucleotide) is the primary electron carrier in catabolic (energy-releasing) reactions. When a substrate is oxidized, NAD+ accepts a hydride ion (H⁻) from the substrate and becomes NADH. The reaction is reversible, and that reversibility is the whole point: NAD+ can pick up electrons in the cytoplasm or mitochondria and deliver them to the electron transport chain, where the electrons are offloaded to oxygen, releasing energy and regenerating NAD+.

The key ratio to care about is NAD+/NADH. Catabolic pathways need NAD+ as an electron acceptor. If the cell runs out of NAD+ (if NADH accumulates faster than it's reoxidized), those pathways stall. This is why oxygen deprivation is so immediately devastating to aerobic metabolism: without oxygen to accept electrons at the end of the transport chain, NADH can't be reoxidized to NAD+, NAD+ runs out, and glycolysis (which requires NAD+) grinds to a halt. The cell's short-term solution under anaerobic conditions is to dump electrons onto pyruvate to make lactate, which regenerates NAD+ and keeps glycolysis running — that's lactic acid fermentation, and we'll cover it fully in the glycolysis chapter.

### NADPH: The Anabolic Electron Carrier

NADPH (nicotinamide adenine dinucleotide phosphate) looks almost identical to NADH; the only structural difference is a phosphate group on the adenosine ribose. But that one phosphate makes it recognizable to completely different enzymes, and it serves a completely different function: NADPH is the electron donor for biosynthetic reactions.

Whenever the cell builds something — fatty acids, cholesterol, amino acids, nucleotides — it needs reducing power, meaning electrons to reduce oxidized carbon precursors into reduced carbon products. NADPH provides those electrons. The cell keeps its NADPH pool separate from its NADH pool precisely because anabolic and catabolic demands have to be managed independently.

The primary source of NADPH is the pentose phosphate pathway, which runs alongside glycolysis and is essentially a glucose-oxidizing machine dedicated to generating NADPH rather than ATP.

**The short rule:** NADH is for catabolism and energy generation. NADPH is for biosynthesis and managing oxidative stress (glutathione reductase, for example, uses NADPH). Same chemistry, completely different cellular role.

### FAD/FADH₂: The Other Electron Carrier

FAD (flavin adenine dinucleotide) is another electron carrier that gets reduced to FADH₂ during oxidation reactions. Like NAD+, it accepts a hydride and is regenerated at the electron transport chain.

Why does the cell use FAD at all when it already has NAD+? Because they have different reduction potentials. NAD+/NADH has a $E^{\circ'}$ of −0.32 V. FAD/FADH₂ has an $E^{\circ'}$ around 0 V (it varies by enzyme context). This means FAD can accept electrons from substrates that NAD+ cannot — specifically substrates that aren't quite oxidized enough to donate electrons to NAD+. The succinate-to-fumarate step in the TCA cycle uses FAD rather than NAD+ for exactly this reason: the $\Delta G^{\circ'}$ for NAD+-linked oxidation of succinate would be slightly positive, but FAD-linked oxidation is favorable.

The trade-off is that FADH₂ delivers electrons to the transport chain at a lower energy point than NADH, so it generates less ATP per molecule. Each NADH ultimately drives the synthesis of about 2.5 ATP; each FADH₂ drives about 1.5 ATP. This difference matters when you're accounting for the total ATP yield of glucose oxidation.

FAD is unique in another way: it's always covalently or tightly non-covalently bound to its enzyme (it's a *prosthetic group*). It doesn't float free the way NAD+ does. This means FAD is functionally part of the enzyme and is recycled right there at the enzyme's active site by the electron transport chain. 

### Coenzyme A: The Acyl Carrier

Coenzyme A (CoA) is the cell's acyl group carrier. The business end of CoA is a thiol group (–SH), and it forms a **thioester bond** with acyl groups (carbon chains with a carbonyl at the end):

$$\text{CoA-SH} + \text{R-COOH} \rightarrow \text{R-CO-S-CoA} + \text{H}_2\text{O}$$

The most important example is acetyl-CoA, where the acyl group is a two-carbon acetyl unit (CH₃CO–). Acetyl-CoA is the central junction of carbon metabolism: it's the form in which the cell packages the carbon from glucose (via pyruvate), from fatty acids (via beta-oxidation), and from certain amino acids, before feeding them into the TCA cycle.

Why does thioester formation matter? Thioester bonds are thermodynamically similar to phosphoanhydride bonds in ATP — they're high-energy in the same sense that ATP is: not because the bond itself is energetic, but because the thioester is in a more reactive, less stable configuration than its hydrolysis products. Hydrolysis of a thioester releases about −31 kJ/mol, right in the range of ATP hydrolysis. This means CoA esters can drive reactions in the same way ATP phosphoryl transfer can, and the two systems are interchangeable in some reactions. The first step of the TCA cycle — citrate synthase — works by exploiting the reactivity of the acetyl-CoA thioester to drive condensation with oxaloacetate.

### A Few Others Worth Knowing

These come up in later chapters, so a heads-up now saves confusion later:

**SAM (S-adenosylmethionine)** is the cell's methyl group donor. Methylation of DNA, histones, neurotransmitters, and many other molecules all go through SAM. When SAM donates its methyl group, it becomes S-adenosylhomocysteine, which is eventually recycled back to methionine. 

**UDPG (UDP-glucose)** is how the cell activates glucose for glycogen synthesis and other glycosylation reactions. Direct glucosyl transfer from glucose itself isn't favorable enough; attaching glucose to UDP (via the high-energy UDP-glucose bond) makes the transfer thermodynamically driven.

**Biotin** carries CO₂ groups. Carboxylation reactions — adding CO₂ to a carbon chain — are used in both fatty acid synthesis and gluconeogenesis, and biotin is the prosthetic group that carries the CO₂ from ATP-driven carboxylation to the acceptor molecule.

---

## Part III: The Phosphate Compound Energy Hierarchy

ATP has a standard free energy of hydrolysis of −30.5 kJ/mol. That's not the highest in the cell — there are phosphorylated compounds with more negative values, and there are compounds with less negative values. This hierarchy matters because it determines which direction phosphoryl groups spontaneously transfer.

Here are representative values:

| Compound | $\Delta G^{\circ'}$ of hydrolysis (kJ/mol) |
|---|---|
| Phosphoenolpyruvate (PEP) | −61.9 |
| 1,3-Bisphosphoglycerate (1,3-BPG) | −49.4 |
| Creatine phosphate | −43.1 |
| **ATP** | **−30.5** |
| Glucose-1-phosphate | −20.9 |
| Glucose-6-phosphate | −13.8 |
| Glycerol-3-phosphate | −9.2 |

ATP sits in the middle. That's intentional.

Compounds above ATP in the hierarchy (PEP, 1,3-BPG, creatine phosphate) can spontaneously phosphorylate ADP to make ATP. This is exactly what happens at the end of glycolysis: PEP donates its phosphate to ADP (catalyzed by pyruvate kinase), and the large favorable $\Delta G^{\circ'}$ drives ATP synthesis even without the electron transport chain. This is called **substrate-level phosphorylation**. Similarly, 1,3-BPG phosphorylates ADP via phosphoglycerate kinase, another substrate-level phosphorylation step.

Compounds below ATP in the hierarchy (glucose-6-phosphate, glycerol-3-phosphate) can't phosphorylate ADP; the energetics go the wrong way. Instead, ATP phosphorylates *them*. This is why hexokinase uses ATP to phosphorylate glucose to glucose-6-phosphate at the start of glycolysis: glucose-6-phosphate is lower in the hierarchy, so the phosphate flows downhill from ATP to glucose.

The position of ATP in the middle of the hierarchy is what makes it work as a universal currency. It can accept phosphate from high-energy donors (capturing energy from catabolism) and donate phosphate to low-energy acceptors (spending that energy on cellular work). If ATP sat at the top, it couldn't be recharged from catabolism. If it sat at the bottom, it couldn't drive anything. The middle position is the whole point.

---

## Part IV: Types of Metabolic Reactions

Every step in every metabolic pathway is a chemical reaction, and every chemical reaction falls into one of a small number of categories. Learning to recognize the categories means you can reason about a reaction's energetics and mechanism even when you've never seen it before.

Here are the six types you'll encounter repeatedly:

### 1. Oxidation-Reduction

Already covered above. One molecule loses electrons (and usually protons), another gains them. NAD+, FAD, and NADP+ are the electron acceptors in catabolic oxidations; NADPH is the electron donor in biosynthetic reductions. The $\Delta G$ is determined by the difference in reduction potentials.

*Example:* Isocitrate + NAD+ → α-ketoglutarate + NADH + CO₂ (TCA cycle, isocitrate dehydrogenase step)

### 2. Group Transfer

One molecule donates a chemical group to another. The group can be a phosphoryl group (from ATP), an acyl group (from CoA), a methyl group (from SAM), or others. The key is that a fragment of one molecule is transferred to another, usually with hydrolysis of a high-energy bond driving the reaction.

*Example:* Glucose + ATP → Glucose-6-phosphate + ADP (hexokinase; phosphoryl transfer from ATP to glucose)

### 3. Hydrolysis

A bond is cleaved by the addition of water. Hydrolysis reactions are thermodynamically favorable for high-energy bonds (phosphoanhydride bonds, thioester bonds) and are often used to drive reactions to completion or to break down macromolecules.

*Example:* ATP + H₂O → ADP + Pᵢ (used to drive endergonic reactions by coupling)

*Example:* Proteins hydrolyzed to amino acids during digestion

### 4. Addition and Elimination

A group is added to a double bond (addition), or a double bond is formed by removing a group (elimination). These reactions often involve water being added across a C=C double bond (hydration) or being removed (dehydration).

*Example:* Fumarate + H₂O → Malate (hydration; fumarase in TCA cycle)

*Example:* Malate → Fumarate + H₂O (dehydration, in the reverse direction; used in fatty acid synthesis)

### 5. Isomerization

The molecule's formula doesn't change, just its structure. A functional group moves to a different position, a chiral center is inverted, or one constitutional isomer is converted to another. Isomerization reactions are often near-equilibrium and are used to set up more favorable downstream reactions.

*Example:* Glucose-6-phosphate → Fructose-6-phosphate (phosphoglucose isomerase, step 2 of glycolysis; moves the carbonyl from C1 to C2)

*Example:* Citrate → Isocitrate (aconitase in TCA cycle; repositions the hydroxyl group for subsequent oxidation)

### 6. Ligation (Carbon-Carbon Bond Formation)

ATP-driven formation of a covalent bond, often a carbon-carbon bond. This is how the cell builds carbon skeletons. Ligases use ATP (or sometimes GTP) hydrolysis to drive bond formation that would otherwise be thermodynamically unfavorable.

*Example:* Pyruvate + CO₂ + ATP → Oxaloacetate + ADP + Pᵢ (pyruvate carboxylase; used in gluconeogenesis)

*Example:* The first step of fatty acid synthesis: acetyl-CoA + CO₂ + ATP → malonyl-CoA + ADP + Pᵢ (acetyl-CoA carboxylase)

---

## Part V: The Thermodynamic Logic of Metabolic Pathways

### Near-Equilibrium vs. Irreversible Steps

Not all steps in a pathway are created equal. Some have $\Delta G^{\circ'}$ values close to zero and operate near equilibrium under cellular conditions — the reaction runs easily in both directions, and the actual direction depends on which side the concentrations are pushing. Other steps have large negative $\Delta G$ values under cellular conditions and are essentially irreversible.

These irreversible steps are the important ones. They're the **committed steps** of a pathway: once you've gone through them, you're committed to that branch of metabolism. They're also the steps where cells place their regulatory machinery, because it makes much more sense to put a throttle at a point of no return than somewhere reversible.

In glycolysis, three reactions are irreversible: the hexokinase step (glucose → glucose-6-phosphate), the phosphofructokinase step (fructose-6-phosphate → fructose-1,6-bisphosphate), and the pyruvate kinase step (PEP → pyruvate). The middle one, phosphofructokinase, is the primary regulated step. When the cell has plenty of ATP, phosphofructokinase is inhibited, and glycolysis slows. When AMP accumulates (signaling energy deprivation), it's activated, and glycolysis speeds up. The allosteric regulation of this single irreversible enzyme controls the flux through the entire pathway.

### Product Removal Keeps Pathways Running

Here's a point that connects back to Chapter 1: the actual $\Delta G$ of any step depends on the concentrations of reactants and products via:

$$\Delta G = \Delta G^{\circ'} + RT\ln\frac{[\text{products}]}{[\text{reactants}]}$$

If product concentrations are kept low, the concentration term is negative, which makes the actual $\Delta G$ more negative than $\Delta G^{\circ'}$ alone. This is how cells keep near-equilibrium steps running in the forward direction even when $\Delta G^{\circ'}$ is slightly positive: if the product is immediately consumed by the next enzyme in the pathway, it never accumulates, the concentration ratio stays small, and the actual $\Delta G$ stays negative.

This is also why metabolic pathways run as coordinated sequences rather than isolated reactions. The product of each step is the substrate for the next. Each enzyme in the chain is, in a sense, pulling on the one before it. Disrupt any step and you get product accumulation upstream and substrate starvation downstream, both of which shift $\Delta G$ values in ways that can stall the whole pathway.

### Coupling Across the Whole Pathway

Chapter 1 showed coupling between two reactions. The same logic extends to an entire pathway. Glycolysis consists of ten sequential reactions. Thermodynamically, you can treat the whole pathway as a single coupled system, summing all ten $\Delta G$ values to get the net driving force for converting glucose to pyruvate. The intermediate steps don't have to be individually favorable as long as the overall sequence is. The thermodynamics of the whole pathway is what matters, and the pathway is held together by the chain of shared intermediates running from glucose all the way to pyruvate.

This is worth sitting with for a moment, because it changes how you think about metabolic regulation. The question isn't "is step 4 favorable?" The question is "is the flux through the whole pathway appropriate for what the cell needs right now?" Regulation works at the level of pathway flux, not individual reaction favorability, and the key regulatory points are almost always the irreversible steps.

---

## When It Breaks

### Metformin and Complex I

Metformin is the first-line drug for type 2 diabetes, taken by hundreds of millions of people. Its mechanism is still not completely understood, but a major component involves inhibiting Complex I of the mitochondrial electron transport chain.

Complex I is where NADH enters the electron transport chain; it accepts electrons from NADH and passes them down the chain toward oxygen. When metformin partially inhibits Complex I, NADH can't be reoxidized as efficiently. NADH accumulates, and the NADH/NAD+ ratio rises.

Here's why that matters: glycolysis, pyruvate dehydrogenase, and the TCA cycle all require NAD+ as an electron acceptor. When NAD+ becomes scarce, these pathways slow down. Glucose is metabolized less efficiently, which reduces the ATP/AMP ratio. Low ATP/AMP activates AMPK (AMP-activated protein kinase), a master metabolic sensor that, among many other effects, suppresses hepatic gluconeogenesis (glucose synthesis in the liver). Less glucose output from the liver means lower blood glucose.

The downstream effects of partially tweaking a single electron transport complex ripple through NADH/NAD+ balance, glycolysis, gluconeogenesis, and whole-body glucose homeostasis. You couldn't follow this chain of events without understanding what NAD+ does, why its ratio to NADH matters, and how the thermodynamics of electron transfer connect to pathway flux. This is the chapter that makes that story readable.

### Thiamine Deficiency and the TCA Cycle

Thiamine (vitamin B₁) is a cofactor for three critical enzymes in oxidative metabolism: pyruvate dehydrogenase (which converts pyruvate to acetyl-CoA), alpha-ketoglutarate dehydrogenase (a TCA cycle enzyme), and transketolase (pentose phosphate pathway). All three are oxidative decarboxylation steps — they oxidize a substrate, release CO₂, and transfer electrons to NAD+.

Thiamine deficiency shuts down all three. The result is a bottleneck at pyruvate: glucose can still be converted to pyruvate by glycolysis, but pyruvate can't be converted to acetyl-CoA and enter the TCA cycle. Pyruvate accumulates and is converted to lactate, producing lactic acidosis.

The neurological consequences — Wernicke encephalopathy, which causes confusion, eye movement abnormalities, and ataxia — reflect the fact that neurons are particularly dependent on aerobic glucose metabolism and have essentially no other fuel option. Thiamine deficiency is classic in chronic alcoholism and severe malnutrition. Treatment with IV thiamine can be dramatically effective if given early.

The mechanism is an NAD+-dependent oxidation step that gets knocked out by losing a cofactor. Without it, the electrons that should move from pyruvate through NADH to the electron transport chain have nowhere to go, the redox cycle stalls, and the cell's aerobic energy metabolism collapses at the entry point to the TCA cycle.

---

## The MCAT Angle

**Reduction potential and spontaneity:** If $\Delta E^{\circ'}$ is positive (acceptor has higher $E^{\circ'}$ than donor), the reaction is spontaneous and $\Delta G^{\circ'}$ is negative. Electrons flow from low to high reduction potential. The equation $\Delta G^{\circ'} = -nF\Delta E^{\circ'}$ ties this directly to free energy.

**NAD+ vs. NADPH:** They look similar but serve opposite metabolic roles. NADH carries electrons from catabolism to the electron transport chain. NADPH donates electrons for biosynthesis. Questions that confuse the two are common — always ask whether the context is breaking things down (catabolism, NADH) or building things up (anabolism, NADPH).

**The phosphate hierarchy:** Compounds above ATP in the hydrolysis hierarchy can phosphorylate ADP. Compounds below ATP get phosphorylated by ATP. PEP and 1,3-BPG are both above ATP, which is why they can drive substrate-level phosphorylation. Glucose-6-phosphate is below ATP, which is why hexokinase runs in the direction ATP → glucose-6-phosphate, not the other way.

**Coenzyme A and thioesters:** When you see acetyl-CoA or any acyl-CoA in a pathway, the thioester bond is what makes the subsequent reaction thermodynamically favorable. The "high-energy" thioester drives condensation, acyl transfer, and similar reactions much like ATP phosphoryl transfer drives phosphorylation.

**Irreversible steps as regulatory nodes:** If a question asks where in a metabolic pathway regulation is most likely to occur, look for the step with the largest negative $\Delta G$ under cellular conditions. That's the irreversible step, and irreversible steps are where cells put their throttles.

**Pathway $\Delta G$ is additive:** The total $\Delta G^{\circ'}$ for a multi-step pathway is the sum of the $\Delta G^{\circ'}$ values for all steps. A pathway can include steps with positive $\Delta G^{\circ'}$ as long as the sum is negative. The coupling is achieved through shared intermediates running the length of the pathway.

---

## Worked Problems

### Problem 1: Reduction Potential and Free Energy

The succinate dehydrogenase reaction in the TCA cycle oxidizes succinate to fumarate, passing electrons to FAD:

$$\text{Succinate} + \text{FAD} \rightarrow \text{Fumarate} + \text{FADH}_2$$

The $E^{\circ'}$ for the fumarate/succinate half-reaction is +0.03 V. The $E^{\circ'}$ for FAD/FADH₂ is 0 V (approximately, in this enzyme context).

(a) Which molecule is oxidized and which is reduced?

(b) Calculate $\Delta G^{\circ'}$ for the reaction (n = 2).

(c) In the electron transport chain, FADH₂ passes electrons to ubiquinone (coenzyme Q), which has an $E^{\circ'}$ of +0.045 V. Is this step thermodynamically favorable? Calculate $\Delta G^{\circ'}$.

**Solution:**

(a) Succinate loses electrons (gets oxidized to fumarate). FAD gains electrons (gets reduced to FADH₂). Fumarate is the oxidized form; succinate is the reduced form.

(b) The electron donor is succinate/fumarate ($E^{\circ'} = +0.03$ V). The acceptor is FAD/FADH₂ ($E^{\circ'} = 0$ V). Wait: we need to be careful about the direction. In the reaction as written, FAD is being reduced and succinate is being oxidized. So:

$$\Delta E^{\circ'} = E^{\circ'}_{\text{acceptor}} - E^{\circ'}_{\text{donor}} = 0 - (+0.03) = -0.03 \text{ V}$$

$$\Delta G^{\circ'} = -nF\Delta E^{\circ'} = -(2)(96.5)(-0.03) = +5.8 \text{ kJ/mol}$$

This is slightly endergonic under standard conditions. In the intact enzyme and under cellular conditions, the reaction is pulled forward by the subsequent reoxidation of FADH₂ at the electron transport chain.

(c) FADH₂ donates to ubiquinone (Q):

$$\Delta E^{\circ'} = E^{\circ'}_{Q} - E^{\circ'}_{\text{FADH}_2} = +0.045 - 0 = +0.045 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(+0.045) = -8.7 \text{ kJ/mol}$$

Negative: favorable. FADH₂ spontaneously reduces ubiquinone. This step releases free energy and contributes (modestly) to the proton gradient that drives ATP synthesis.

---

### Problem 2: The Phosphate Hierarchy

A student proposes the following reaction as an energy source:

$$\text{Glucose-6-phosphate} + \text{ADP} \rightarrow \text{Glucose} + \text{ATP}$$

$\Delta G^{\circ'}$ for glucose-6-phosphate hydrolysis = −13.8 kJ/mol
$\Delta G^{\circ'}$ for ATP hydrolysis = −30.5 kJ/mol

(a) Is this reaction thermodynamically favorable in the direction written?

(b) Explain this using the phosphate energy hierarchy.

(c) The reverse reaction — hexokinase phosphorylating glucose using ATP — is spontaneous. What is its $\Delta G^{\circ'}$?

**Solution:**

(a) To evaluate the reaction as written, calculate $\Delta G^{\circ'}$ for the net reaction. The reaction as written is the reverse of ATP hydrolysis plus the hydrolysis of glucose-6-phosphate:

$$\Delta G^{\circ'} = \Delta G^{\circ'}_{\text{G6P hydrolysis}} + \Delta G^{\circ'}_{\text{ADP phosphorylation}}$$

ADP phosphorylation is the reverse of ATP hydrolysis: $\Delta G^{\circ'} = +30.5$ kJ/mol.

$$\Delta G^{\circ'} = -13.8 + 30.5 = +16.7 \text{ kJ/mol}$$

Not favorable. This reaction doesn't go in the direction written.

(b) Glucose-6-phosphate sits below ATP in the phosphate energy hierarchy ($\Delta G^{\circ'}$ of hydrolysis −13.8 vs. −30.5 kJ/mol). Phosphate spontaneously transfers from higher-energy to lower-energy compounds, meaning from ATP down to glucose — not the other way. You can't use glucose-6-phosphate to make ATP because that would be moving phosphate uphill thermodynamically.

(c) The reverse reaction — ATP phosphorylating glucose to glucose-6-phosphate — simply has the opposite sign:

$$\text{Glucose} + \text{ATP} \rightarrow \text{Glucose-6-phosphate} + \text{ADP} \qquad \Delta G^{\circ'} = -16.7 \text{ kJ/mol}$$

Spontaneous. This is why hexokinase runs in this direction: ATP is higher in the hierarchy, so phosphoryl transfer flows from ATP to glucose.

---

### Problem 3: Pathway Flux and Product Removal

An enzyme catalyzes the reaction:

$$A \rightarrow B \qquad \Delta G^{\circ'} = +4.2 \text{ kJ/mol}$$

Under standard conditions, this reaction is not favorable. But inside a cell, [A] = 2.0 mM and [B] = 0.05 mM. The temperature is 37°C (310 K).

(a) Calculate the actual $\Delta G$ inside the cell.

(b) Is the reaction spontaneous under cellular conditions?

(c) A downstream enzyme rapidly converts B to C. How does this change the analysis?

**Solution:**

(a) Use:

$$\Delta G = \Delta G^{\circ'} + RT\ln\frac{[B]}{[A]}$$

$$\Delta G = +4200 + (8.314)(310)\ln\frac{0.05 \times 10^{-3}}{2.0 \times 10^{-3}}$$

$$= +4200 + (2577)\ln(0.025)$$

$$= +4200 + (2577)(-3.69)$$

$$= +4200 - 9510 = -5310 \text{ J/mol} = -5.3 \text{ kJ/mol}$$

(b) Yes. Even though $\Delta G^{\circ'} > 0$, the actual $\Delta G$ is negative under cellular conditions because the product B is kept at a very low concentration relative to A. The reaction is spontaneous.

(c) If a downstream enzyme converts B to C, [B] stays low or drops even further. This keeps the concentration ratio $[B]/[A]$ small and the logarithm term large and negative. Product removal by the downstream enzyme is what maintains the thermodynamic driving force for this step, and for many near-equilibrium steps in metabolic pathways. The pathway enzymes are not independent: they cooperate thermodynamically through the metabolite concentrations they set for each other.

---

## Opener Questions Revisited

**1. NAD+ gains electrons during glycolysis to become NADH. Why does that matter?**

Those electrons represent free energy that the cell hasn't captured yet. NADH carries them from the cytoplasm to the inner mitochondrial membrane, where the electron transport chain accepts them and passes them through a series of carriers of increasing reduction potential, ultimately to oxygen. The free energy released as electrons fall down this electrochemical gradient is used to pump protons across the inner membrane, creating a proton gradient. That gradient drives ATP synthase. The electrons that NAD+ picks up from glycolysis are ultimately responsible for most of the ATP the cell makes from glucose oxidation. Without NAD+, those electrons would have nowhere to go, glycolysis would stall, and the cell would be limited to the two net ATPs from substrate-level phosphorylation.

**2. If there are higher-energy phosphate compounds than ATP, why is ATP the universal currency?**

Because ATP sits in the middle of the phosphate energy hierarchy. High-energy phosphate compounds like PEP and 1,3-BPG, generated by catabolism, can donate their phosphate groups to ADP, recharging ATP. ATP then donates phosphate to low-energy acceptors, driving biosynthetic reactions and ion transport and mechanical work. A compound at the top of the hierarchy could only receive phosphate, never donate it to anything. A compound at the bottom could only receive ATP's phosphate, never generate ATP from catabolism. The middle position allows ATP to shuttle phosphate from producers (catabolism) to consumers (everything else). It's the universal currency precisely because it can be both spent and replenished.

---

*Chapter 10 (Glycolysis & Gluconeogenesis): This is where the toolkit gets used. Glycolysis is ten reactions: a mix of phosphoryl transfers, isomerizations, oxidation-reduction, and substrate-level phosphorylation, all linked by shared intermediates into a single thermodynamic unit. Every reaction type from Part IV shows up.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*
