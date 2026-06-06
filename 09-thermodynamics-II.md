# Chapter 9: Thermodynamic Principles II: The Cell's Energy Currency

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. $\text{NAD}^+$ gains electrons during glycolysis to become NADH. Why does that matter? Where do those electrons go eventually, and what does the cell get out of it?

2. ATP sits in the middle of the cell's phosphate energy hierarchy, not at the top. Why is it the universal currency if there are more energetically favorable compounds available?

---

## The Big Picture

Chapter 1 gave you the thermodynamic framework. You know that cells run on free energy, that reactions couple together through shared intermediates, and that ATP hydrolysis drives an enormous amount of cellular work. 

Now we need to get more specific, because "the cell uses free energy" is about as useful as "the economy runs on money." True, but not actionable. 

What we're building in this chapter is a working picture of *how* the cell actually handles energy at the molecular level: which molecules carry it, how it gets transferred, and what kinds of reactions move it around. Once you have this toolkit, metabolic pathways stop looking like lists of reactions to memorize and start looking like what they actually are: sequences of energy transfers with a clear thermodynamic logic.

Three things to walk away with:

1. Electron transfer ***is*** energy transfer. The cell moves energy by moving electrons, and it does it constantly.
2. A small set of carrier molecules handles almost all energy transactions in the cell.
3. Every reaction in a metabolic pathway fits into one of a handful of types, and once you recognize the type, you can reason about the energetics.

> **Clinical preview:** Metformin, the most commonly prescribed drug for type 2 diabetes, works at least partly by interfering with Complex I (the first of four protein complexes that form the mitochondrial electron transport chain, and the entry point for electrons from NADH) of the electron transport chain. That changes the cell's NADH/$\text{NAD}^+$ ratio, which ripples through glucose metabolism and ultimately lowers blood glucose. We'll come back to this mechanism once you know what NADH actually does and why its ratio to $\text{NAD}^+$ matters.

---

## Part I: Redox Chemistry

### What Oxidation and Reduction Actually Mean

You've probably heard "OIL RIG": oxidation is loss, reduction is gain (of electrons). That's correct as far as it goes, but it's worth slowing down and understanding why electron transfer matters in a biological context, because it's not immediately obvious why moving electrons around should release useful energy.

Here's the key insight: electrons don't all have the same energy. An electron sitting on a carbon atom in glucose has more potential energy than an electron sitting on an oxygen atom in water. This isn't arbitrary; it reflects how strongly different atoms hold onto electrons. Oxygen is extremely electronegative, meaning it attracts electrons strongly. Carbon is much less so. When you oxidize glucose completely to $\text{CO}_2$ and $\text{H}_2\text{O}$, you're essentially moving electrons from a low-affinity environment (carbon) to a high-affinity environment (oxygen). Electrons move to where they're held more tightly, and the energy *difference* is released.

This is exactly analogous to gravitational potential energy. A ball at the top of a hill has more potential energy than at the bottom; it rolls downhill and releases energy. Electrons "roll" from atoms that hold them loosely to atoms that hold them tightly, and the energy difference is released. Whether the cell captures that energy or loses it as heat depends on the machinery in between.

In biological systems, oxidation and reduction almost always involve the transfer of both electrons and protons together, because carbon-hydrogen bonds are what actually get broken. When you oxidize a carbon compound, you remove H atoms from it. Each H atom is one proton and one electron. The carrier molecules that accept them, primarily $\text{NAD}^+$ and FAD, receive both. So in practice you'll see reactions written as:

$$\text{substrateH}_2 + \text{NAD}^+ \rightarrow \text{oxidized substrate} + \text{NADH} + \text{H}^+$$

$$\text{substrateH}_2 + \text{FAD} \rightarrow \text{oxidized substrate} + \text{FADH}_2$$

The difference in how the protons are handled is worth noticing. $\text{NAD}^+$ accepts a hydride ion ($\text{H}^-$: one proton plus two electrons) from the substrate and releases the second proton to solution, hence the free $\text{H}^+$ on the right. FAD accepts both protons and both electrons directly, so both end up on the carrier and nothing is released. Same two electrons transferred, different proton accounting.

### Reduction Potentials

How do we quantify how much an atom or molecule "wants" electrons? Through the **standard reduction potential**, written $E^{\circ'}$ (in volts), measured at biochemical standard conditions (pH 7, 25°C, 1 M concentrations).

These aren't theoretical values; they're measured. The basic setup is to take your half-reaction and run it in competition against a universal reference: the **standard hydrogen electrode** (SHE), which is defined as 0 V by convention. You let electrons flow between the two half-reactions and measure the voltage. If your molecule pulls electrons away from the SHE, the voltage is positive; if the SHE pulls electrons away from your molecule, the voltage is negative. Do this for every half-reaction of interest, and you end up with a table of values that are all on the same scale, all comparable to each other, because they were all measured against the same reference point.

Why volts? Because a volt measures electrical potential difference, which is energy per unit charge (joules per coulomb, J/C). Think of it like a battery: a 9V battery "pushes" electrons harder than a 1.5V battery, and that higher voltage means more energy is released per electron moved. Reduction potential works the same way: a higher $E^{\circ'}$ means a stronger *pull* on electrons and more energy released when they flow. This is also exactly why $\Delta G^{\circ'} = -nF\Delta E^{\circ'}$ works out so cleanly: $n$ is moles of electrons, $F$ converts that to coulombs ($96,485 \frac{\text{C}}{\text{mol}}$ or $96.5 \frac{\text{kJ}}{\text{mol}\cdot\text{V}}$), and $\Delta E^{\circ'}$ is the voltage. Multiply charge by voltage and you get joules per mole. The equation isn't a biochemistry invention; it's just unit analysis on the definition of a volt.

The convention: a high (more positive) $E^{\circ'}$ means a molecule has a strong tendency to *grab* electrons, to be reduced. A low (more negative) $E^{\circ'}$ means a molecule tends to *donate* electrons, to be oxidized.

Electrons flow spontaneously from lower $E^{\circ'}$ to higher $E^{\circ'}$, for the same reason water flows downhill. Here are some biologically important values:

| Half-reaction | $n$ | $E^{\circ'}$ (V) |
|---|---|---|
| $\frac{1}{2}O_2 + 2H^+ + 2e^- \rightarrow H_2O$ | 2 | +0.82 |
| $\text{Fumarate} + 2\text{H}^+ + 2e^- \rightarrow \text{Succinate}$ | 2 | +0.03 |
| $\text{NAD}^+ + \text{H}^+ + 2e^- \rightarrow \text{NADH}$ | 2 | −0.32 |
| $\text{NADP}^+ + \text{H}^+ + 2e^- \rightarrow \text{NADPH}$ | 2 | −0.32 |

But let's not just assert that electrons flow from low to high $E^{\circ'}$, let's prove it thermodynamically using the equation connecting reduction potential to free energy:

$$\Delta G^{\circ'} = -nF\Delta E^{\circ'}$$

where:
- $n$ = number of electrons transferred
- $F$ = Faraday's constant = 96.5 kJ/V·mol (sometimes written 96,485 J/V·mol)
- $\Delta E^{\circ'} = E^{\circ'}_{\text{acceptor}} - E^{\circ'}_{\text{donor}}$

Take the reaction that will matter most in the coming chapters: NADH passing its electrons to oxygen.

$$\text{NADH} + \frac{1}{2}\text{O}_2 + \text{H}^+ \rightarrow \text{NAD}^+ + \text{H}_2\text{O}$$

NADH is the donor ($E^{\circ'} = -0.32$ V), oxygen is the acceptor ($E^{\circ'} = +0.82$ V):

$$\Delta E^{\circ'} = +0.82 - (-0.32) = +1.14 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(1.14) = -220 \text{ kJ/mol}$$

That's enormously negative, roughly seven times the $\Delta G^{\circ '}$ of ATP hydrolysis. And this is where the direction rule comes from: $\Delta E^{\circ'}$ is positive because the acceptor has a higher reduction potential than the donor, which makes $\Delta G^{\circ'}$ negative, which means the reaction is spontaneous. Run it the other way (oxygen donating to NADH), and $\Delta E^{\circ'}$ flips negative, $\Delta G^{\circ'}$ goes positive, and the reaction doesn't go. Electrons flow from low to high $E^{\circ'}$ for exactly the same reason any reaction runs in the direction of negative $\Delta G$: thermodynamics ***requires*** it to do so.

### Where Redox Fits in Metabolism

So the oxidation of NADH by oxygen releases −220 kJ/mol and is thermodynamically mandatory. The problem is that you can't actually use that energy if it's released all at once. A single uncontrolled transfer of electrons from NADH directly to oxygen would just generate heat. You can't build ATP from an explosion.

This is the whole point of what is called the **electron transport chain (ETC)**: it's the cell's way of doing this in a controlled, stepwise fashion. Instead of one enormous drop, the electrons pass through a series of protein complexes in the inner mitochondrial membrane, each with a slightly higher reduction potential than the last, releasing free energy incrementally at each step. That energy release is *captured* and used to pump protons across the membrane, building a proton gradient (a very specific electrochemical gradient with its own name: called $\Delta \text{p}$). The gradient then drives ATP synthesis through a molecular turbine called ATP synthase. It's a Rube Goldberg machine of spectacular elegance: electrons fall down an electrochemical staircase, the energy released is used to pump protons uphill, and the protons flowing back downhill spin a rotor that makes ATP.

So when you see a step in glycolysis or the TCA cycle labeled "oxidation," here's what's actually happening: a carbon compound loses electrons and protons to $\text{NAD}^+$ or FAD, converting them to NADH or $\text{FADH}_2$. The carbon compound is done; it moves on to the next reaction. But the electrons aren't done. They ride NADH or $\text{FADH}_2$ to the inner mitochondrial membrane, enter the electron transport chain, and begin their stepwise descent toward oxygen. The free energy released along the way becomes the proton gradient that makes most of the cell's ATP.

The pathway is essentially a wire connecting fuel molecules to oxygen, with the cell tapping the energy at controlled points along the wire.

It's worth pausing on how physical this is. ATP synthase is a literal rotary motor, a protein that spins. The proton gradient drives rotation of this rotor at around 130 revolutions per ***second***, and each full turn synthesizes 3 ATP molecules. This is happening right now, thousands of times simultaneously in every mitochondria, in every one of your trillions of cells, continuously, every second of your life. A resting adult produces roughly their own body weight in ATP every day, virtually all of it from ATP synthase. The reason that number is even achievable is the controlled stepwise architecture of the ETC: by breaking the −220 kJ/mol drop into smaller increments and coupling each increment to proton pumping, the cell can run ATP synthase fast enough to keep up with demand. A single uncontrolled drop from NADH to oxygen couldn't do that, only a controlled thermodynamic balancing act could accomplish this reliably for decades (or longer if you're a lobster).

---

## Part II: The Activated Carrier Toolkit

Before diving in, it's worth defining two terms that will organize everything from here on out. **Catabolism** is the set of pathways that break molecules down, releasing free energy in the process (glycolysis, the TCA cycle, fatty acid oxidation). **Anabolism** is the set of pathways that build molecules up, consuming free energy to do so (fatty acid synthesis, gluconeogenesis, protein synthesis). Metabolism is the sum of both. The reason the distinction matters here is that the cell uses different carrier molecules for the two directions: catabolic pathways generate energy-carrying molecules, anabolic pathways spend them. Keeping those pools separate is how the cell avoids short-circuiting itself.

The cell handles energy in the form of specific molecular carriers. There are only a handful of them, but they carry almost all of the cell's energy transactions. Think of them as denominations of cellular currency, each useful for different kinds of transactions.

### ATP: The Universal Phosphoryl Donor

You already know ATP from Chapter 1. The quick recap for this context: $\text{ATP}$ hydrolysis to $\text{ADP} + \text{P}_i$ releases about −30.5 kJ/mol under standard conditions ($\Delta G^{\circ '}$) and about −50 to −60 kJ/mol under cellular conditions ($\Delta G$). This free energy is used to drive reactions that wouldn't otherwise go.

The mechanism is almost always direct phosphoryl transfer: the enzyme moves the phosphate group from ATP to the substrate rather than hydrolyzing ATP in solution first and hoping the energy somehow carries over. Chapter 1 covered why the shared intermediate (the phosphorylated substrate) is what makes the coupling thermodynamically legitimate.

One thing to add here: there are two kinds of ATP hydrolysis worth distinguishing. Sometimes ATP loses just the terminal phosphate (producing ADP + $\text{P}_\text{i}$). Other times ATP loses a pyrophosphate group (the two terminal phosphates together), producing AMP + $\text{PP}_\text{i}$. The pyrophosphate ($\text{PP}_\text{i}$) is then rapidly hydrolyzed by pyrophosphatase to 2 $\text{P}_\text{i}$. Because pyrophosphatase essentially makes the $\text{PP}_\text{i}$ hydrolysis irreversible, this gives an even larger thermodynamic driving force than the ADP pathway. Fatty acid activation (attaching a fatty acid to CoA before oxidation) uses this trick.

### $\text{NAD}^+$/NADH: The Catabolic Electron Carrier

$\text{NAD}^+$ (nicotinamide adenine dinucleotide) is the primary electron carrier in catabolic (energy-releasing) reactions. When a substrate is oxidized, $\text{NAD}^+$ accepts a hydride ion ($\text{H}^-$) from the substrate and becomes $\text{NADH}$. A hydride contains 2 electrons, effectively $\text{NADH}$ is a carrier of electron *pairs*. The reaction is reversible, and that reversibility is the whole point: $\text{NAD}^+$ can pick up electrons in the cytoplasm or mitochondria and deliver them to the electron transport chain, where the electrons are offloaded to oxygen, releasing energy and regenerating $\text{NAD}^+$.

The key ratio to care about is $\text{NAD}^+/\text{NADH}$. Catabolic pathways need $\text{NAD}^+$ as an electron acceptor. If the cell runs out of $\text{NAD}^+$ (if NADH accumulates faster than it's oxidized), those pathways stall. This is why oxygen deprivation is so immediately devastating to aerobic metabolism: without oxygen to accept electrons at the end of the transport chain, NADH can't be reoxidized to $\text{NAD}^+$, $\text{NAD}^+$ runs out, and glycolysis, the Krebs cycle, fatty-acid oxidation, protein catabolism (all of which require $\text{NAD}^+$) grind to a halt. The cell's short-term solution under anaerobic conditions is to dump electrons onto pyruvate to make lactate, which regenerates $\text{NAD}^+$ and keeps glycolysis running. That's lactic acid fermentation, and we'll cover it fully in the glycolysis chapter.

### FAD/$\text{FADH}_2$: The Other Electron Carrier

FAD (flavin adenine dinucleotide) is another electron carrier; it gets reduced to $\text{FADH}_2$ during oxidation reactions. Unlike $\text{NAD}^+$, which accepts a hydride ion, FAD accepts two hydrogen atoms directly, one from each carbon being oxidized; it picks up two protons and two electrons in the process, so still an electron *pair* carrier. It is regenerated at the electron transport chain.

Why does the cell use FAD at all when it already has $\text{NAD}^+$? Because they have different reduction potentials, and that difference determines which substrates each can oxidize. $\text{NAD}^+/\text{NADH}$ has an $E^{\circ'}$ of −0.32 V. $\text{FAD}/\text{FADH}_2$ varies by enzyme context, but in succinate dehydrogenase it's approximately 0 V.

The succinate-to-fumarate oxidation is the clearest example. Fumarate/succinate is already in the table above: $E^{\circ'} = +0.03$ V. In this reaction, succinate is the electron donor. Let's try both carriers:

**With $\text{NAD}^+$ as acceptor** ($E^{\circ'} = -0.32$ V):

$$\Delta E^{\circ'} = -0.32 - (+0.03) = -0.35 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(-0.35) = +67.6 \text{ kJ/mol}$$

Strongly unfavorable. $\text{NAD}^+$ cannot oxidize succinate; the electrons would have to flow uphill by 0.35 V. No cellular concentration adjustment is large enough to overcome a +67.6 kJ/mol penalty.

**With FAD as acceptor** ($E^{\circ'} \approx 0$ V in this enzyme):

$$\Delta E^{\circ'} = 0 - (+0.03) = -0.03 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(-0.03) = +5.8 \text{ kJ/mol}$$

Slightly unfavorable under standard conditions, but only barely. Under cellular conditions, fumarate is immediately consumed by the next enzyme in the TCA cycle and $\text{FADH}_2$ is rapidly reoxidized by the electron transport chain, keeping both product concentrations low and pulling the reaction forward. A +5.8 kJ/mol standard penalty is easily overcome by concentration effects; a +67.6 kJ/mol penalty is not. This is why the cell uses $\text{FAD}$ here and not $\text{NAD}^+$: it's the only carrier with a reduction potential close enough to succinate's to make the reaction thermodynamically workable.

The trade-off is that $\text{FADH}_2$ delivers electrons to the transport chain at a lower energy point than NADH, and we can show exactly why with the same calculation we've been doing. Both carriers ultimately pass their electrons to oxygen; the question is how much free energy is released when they do.

**NADH oxidation by $\text{O}_2$** (donor $E^{\circ'} = -0.32$ V, acceptor $E^{\circ'} = +0.82$ V):

$$\Delta E^{\circ'} = +0.82 - (-0.32) = +1.14 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(1.14) = -220 \text{ kJ/mol}$$

**$\text{FADH}_2$ oxidation by $\text{O}_2$** (donor $E^{\circ'} \approx 0$ V, acceptor $E^{\circ'} = +0.82$ V):

$$\Delta E^{\circ'} = +0.82 - 0 = +0.82 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(0.82) = -158 \text{ kJ/mol}$$

$\text{FADH}_2$ releases about 62 kJ/mol less than NADH when oxidized by oxygen. That's roughly 28% less free energy available to pump protons and drive ATP synthesis, which is exactly why the ATP yields differ: each NADH drives synthesis of about 2.5 ATP, each $\text{FADH}_2$ about 1.5 ATP. The numbers come directly from the reduction potentials, not from a table someone memorized.

FAD is unique in another way: it's always covalently or tightly non-covalently bound to its enzyme (it's a *prosthetic group* (a non-amino-acid cofactor permanently bound to its enzyme), like the heme in hemoglobin). It doesn't float free the way $\text{NAD}^+$ does. This means FAD is functionally part of the enzyme and is recycled right there at the enzyme's active site by the electron transport chain (we'll see how exactly when we examine the ETC more carefully). 

### NADPH: The Anabolic Electron Carrier

NADPH (nicotinamide adenine dinucleotide phosphate) looks almost identical to NADH; the only structural difference is a phosphate group on the adenosine ribose. But that one phosphate makes it recognizable to completely different enzymes, and it serves a completely different function: NADPH is the electron donor for biosynthetic reactions.

When we break down fuels, much like a car engine, that fuel is being *oxidized*, the oxidizers are $\text{NAD}^+$ or $\text{FAD}$. Conversely, whenever the cell *builds* something (fatty acids, cholesterol, amino acids, nucleotides), it needs reducing power, meaning electrons to reduce oxidized carbon precursors into reduced carbon products. $\text{NADPH}$ provides those electrons. The cell keeps its $\text{NADPH}$ pool separate from its $\text{NADH}$ pool precisely because anabolic and catabolic demands have to be managed independently.

The primary source of NADPH is the pentose phosphate pathway, which runs alongside glycolysis. It oxidizes glucose-6-phosphate to generate NADPH and ribose-5-phosphate (the sugar backbone of nucleotides); the full pathway is covered in a later chapter.

**The short rule:** NADH is for catabolism and energy generation. NADPH is for biosynthesis and managing oxidative stress (glutathione reductase, for example, uses NADPH). Same chemistry, completely different cellular role.


### Coenzyme A: The Acyl Carrier

Coenzyme A (CoA) is the cell's acyl group carrier. The business end of CoA is a thiol group (–SH), and it forms a **thioester bond** with acyl groups (carbon chains with a carbonyl at the end):

$$\text{CoA-SH} + \text{RCOO}^- + \text{H}^+ \rightarrow \text{R}{-}\overset{\overset{\displaystyle\mathrm{O}}{\|}}{\text{C}}{-}\text{S-CoA} + \text{H}_2\text{O}$$

The most important example is acetyl-CoA, where the acyl group is a two-carbon acetyl unit ($\text{CH}_3\text{CO}$–). Acetyl-CoA is the central junction of carbon metabolism: it's the form in which the cell packages the carbon from glucose (via pyruvate), from fatty acids (via beta-oxidation, the stepwise two-carbon cleavage of fatty acyl chains, covered in a later chapter), and from certain amino acids, before feeding them into the TCA cycle.

Why does thioester formation matter? Thioester bonds are thermodynamically similar to phosphoanhydride bonds in ATP. They're high-energy in the same sense that ATP is: not because the bond itself is energetic, but because the thioester is in a more reactive, less stable configuration than its hydrolysis products. Hydrolysis of a thioester releases about −31 kJ/mol, right in the range of ATP hydrolysis. This means CoA thioesters can drive reactions in the same way ATP phosphoryl transfer can, and the two systems are interchangeable in some reactions. The first step of the TCA cycle, citrate synthase, works by exploiting the reactivity of the acetyl-CoA thioester to drive condensation with oxaloacetate (a 4-carbon TCA cycle intermediate, introduced in Ch11).

### A Few Others Worth Knowing

These come up in later chapters, so a heads-up now saves confusion later:

**SAM (S-adenosylmethionine)** is the cell's methyl group donor. Methylation of DNA, histones, neurotransmitters, and many other molecules all go through SAM. When SAM donates its methyl group, it becomes S-adenosylhomocysteine, which is eventually recycled back to methionine. 

**UDPG (UDP-glucose)** is how the cell activates glucose for glycogen synthesis and other glycosylation reactions. Direct glucosyl transfer from glucose itself isn't favorable enough; attaching glucose to UDP (via the high-energy UDP-glucose bond) makes the transfer thermodynamically driven.

**Biotin** carries $\text{CO}_2$ groups. Carboxylation reactions (adding $\text{CO}_2$ to a carbon chain) are used in both fatty acid synthesis and gluconeogenesis (the synthesis of glucose from non-sugar precursors, covered fully in Ch10), and biotin is the prosthetic group that carries the $\text{CO}_2$ from ATP-driven carboxylation to the acceptor molecule.

**THF (tetrahydrofolate)** carries one-carbon units at various oxidation states (from methyl all the way up to formyl) and is essential for synthesizing purines, thymidine, and several amino acids. Unlike SAM, which donates only methyl groups, THF handles the full range of one-carbon chemistry. It's also the target of some of the most widely used drugs in medicine: methotrexate (used in cancer and rheumatoid arthritis) and trimethoprim (a common antibiotic) both work by blocking THF synthesis or recycling, starving rapidly dividing cells of the one-carbon units they need to make DNA.

---

## Part III: The Phosphate Compound Energy Hierarchy

ATP has a standard free energy of hydrolysis of −30.5 kJ/mol. That's not the highest in the cell; there are phosphorylated compounds with more negative values, and there are compounds with less negative values. This hierarchy matters because it determines which direction phosphoryl groups spontaneously transfer.

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

A concrete example makes this click. PEP (phosphoenolpyruvate) sits well above ATP in the hierarchy. So PEP can phosphorylate ADP. That's the pyruvate kinase reaction, the last step of glycolysis. Stack PEP hydrolysis against the reverse of ATP hydrolysis (i.e., ADP phosphorylation) and sum:

$$
\begin{array}{rcll}
\text{PEP} + \cancel{H_2O} & \rightarrow & \text{Pyruvate} + \cancel{P_i} & \Delta G^{\circ'} = -61.9 \text{ kJ/mol} \\
ADP + \cancel{P_i} & \rightarrow & ATP + \cancel{H_2O} & \Delta G^{\circ'} = +30.5 \text{ kJ/mol} \\
\hline
\text{PEP} + ADP & \rightarrow & \text{Pyruvate} + ATP & \Delta G^{\circ'} = -31.4 \text{ kJ/mol}
\end{array}
$$

Favorable. Phosphate flows downhill from PEP to ADP, and ATP is synthesized.

Now try the reverse: can ATP phosphorylate pyruvate back to PEP? Stack ATP hydrolysis against the reverse of PEP hydrolysis:

$$
\begin{array}{rcll}
ATP + \cancel{H_2O} & \rightarrow & ADP + \cancel{P_i} & \Delta G^{\circ'} = -30.5 \text{ kJ/mol} \\
\text{Pyruvate} + \cancel{P_i} & \rightarrow & \text{PEP} + \cancel{H_2O} & \Delta G^{\circ'} = +61.9 \text{ kJ/mol} \\
\hline
ATP + \text{Pyruvate} & \rightarrow & ADP + \text{PEP} & \Delta G^{\circ'} = +31.4 \text{ kJ/mol}
\end{array}
$$

Not favorable. The math simply doesn't work in this direction. This is why pyruvate kinase is irreversible under cellular conditions, and why gluconeogenesis (which needs to go from pyruvate back toward PEP) can't just run pyruvate kinase in reverse as we'll see in the glycolysis chapter. It has to use a completely different two-enzyme workaround that costs two ATP equivalents to get the job done. The hierarchy forces that detour.

---

## Part IV: Types of Metabolic Reactions

Every step in every metabolic pathway is a chemical reaction, and every chemical reaction falls into one of a small number of categories. Learning to recognize the categories means you can reason about a reaction's energetics and mechanism even when you've never seen it before.

Here are the six types you'll encounter repeatedly:

### 1. Oxidation-Reduction

Already covered above. One molecule loses electrons (and usually protons), another gains them. $\text{NAD}^+$, FAD, and $\text{NADP}^+$ are the electron acceptors in catabolic oxidations; NADPH is the electron donor in biosynthetic reductions. The $\Delta G$ is determined by the difference in reduction potentials.

*Example:* Isocitrate + $\text{NAD}^+$ → α-ketoglutarate + $\text{NADH}$ + $\text{CO}_2$ (TCA cycle step 3, introduced in Ch11; isocitrate and α-ketoglutarate are TCA cycle intermediates you will meet there)

### 2. Group Transfer

One molecule donates a chemical group to another. The group can be a phosphoryl group (from ATP), an acyl group (from CoA), a methyl group (from SAM), or others. The key is that a fragment of one molecule is transferred to another, usually with hydrolysis of a high-energy bond driving the reaction.

*Example:* Glucose + ATP → Glucose-6-phosphate + ADP (hexokinase; phosphoryl transfer from ATP to glucose)

### 3. Hydrolysis

A bond is cleaved by the addition of water. Hydrolysis reactions are thermodynamically favorable for high-energy bonds (phosphoanhydride bonds, thioester bonds) and are often used to drive reactions to completion or to break down macromolecules.

*Example:* ATP + $\text{H}_2\text{O}$ → ADP + $\text{P}_\text{i}$ (used to drive endergonic reactions by coupling)

*Example:* Proteins hydrolyzed to amino acids during digestion

### 4. Addition and Elimination

A group is added to a double bond (addition), or a double bond is formed by removing a group (elimination). These reactions often involve water being added across a C=C double bond (hydration) or being removed (dehydration).

*Example:* Fumarate + $\text{H}_2\text{O}$ → Malate (hydration; fumarase, step 7 of the TCA cycle, Ch11)

*Example:* Malate → Fumarate + $\text{H}_2\text{O}$ (dehydration, in the reverse direction; used in fatty acid synthesis)

### 5. Isomerization

The molecule's formula doesn't change, just its structure. A functional group moves to a different position, a chiral center is inverted, or one constitutional isomer is converted to another. Isomerization reactions are often near-equilibrium and are used to set up more favorable downstream reactions.

*Example:* Glucose-6-phosphate → Fructose-6-phosphate (phosphoglucose isomerase, step 2 of glycolysis; moves the carbonyl from C1 to C2)

*Example:* Citrate → Isocitrate (aconitase, step 2 of the TCA cycle, Ch11; repositions the hydroxyl group for subsequent oxidation)

### 6. Ligation (Carbon-Carbon Bond Formation)

ATP-driven formation of a covalent bond, often a carbon-carbon bond. This is how the cell builds carbon skeletons. Ligases use ATP (or sometimes GTP) hydrolysis to drive bond formation that would otherwise be thermodynamically unfavorable.

*Example:* Pyruvate + $\text{CO}_2$ + ATP → Oxaloacetate + ADP + $\text{P}_\text{i}$ (pyruvate carboxylase; used in gluconeogenesis, introduced in Ch10)

*Example:* The first step of fatty acid synthesis: acetyl-CoA + $\text{CO}_2$ + ATP → malonyl-CoA (a 3-carbon acyl-CoA used as the building block in fatty acid synthesis) + ADP + $\text{P}_\text{i}$ (acetyl-CoA carboxylase)

---

## Part V: The Thermodynamic Logic of Metabolic Pathways

### Near-Equilibrium vs. Irreversible Steps

Not all steps in a pathway are created equal. Some have $\Delta G^{\circ'}$ values close to zero and operate near equilibrium under cellular conditions, meaning the reaction runs easily in both directions, and the actual direction depends on which side the concentrations are pushing. Other steps have large negative $\Delta G$ values under cellular conditions and are essentially irreversible.

These irreversible steps are the important ones. They're the **committed steps** of a pathway: once you've gone through them, you're committed to that branch of metabolism. They're also the steps where cells place their regulatory machinery, because it makes much more sense to put a throttle at a point of no return than somewhere reversible.

In glycolysis, three reactions are irreversible: the hexokinase step (glucose → glucose-6-phosphate), the phosphofructokinase step (fructose-6-phosphate → fructose-1,6-bisphosphate), and the pyruvate kinase step (PEP → pyruvate). The middle one, phosphofructokinase, is the primary regulatory step. When the cell has plenty of ATP, phosphofructokinase is inhibited, and glycolysis slows. When AMP accumulates (signaling energy deprivation), it's activated, and glycolysis speeds up. The allosteric regulation of this single irreversible enzyme controls the flux through the entire pathway.

### Product Removal Keeps Pathways Running

Here's a point that connects back to Chapter 1: the actual $\Delta G$ of any step depends on the concentrations of reactants and products via:

$$\Delta G = \Delta G^{\circ'} + RT\ln\frac{[\text{products}]}{[\text{reactants}]}$$

If product concentrations are kept low, $\frac{\text{products}}{\text{reactants}}<1$ its logarithm is negative, and $\Delta G$ is pulled below $\Delta G^{\circ'}$. This is how cells keep near-equilibrium steps running in the forward direction even when $\Delta G^{\circ'}$ is slightly positive: if the product is immediately consumed by the next enzyme in the pathway, it never accumulates, the concentration ratio stays small, and the actual $\Delta G$ stays negative.

This is also why metabolic pathways run as coordinated sequences rather than isolated reactions. The product of each step is the substrate for the next. Each enzyme in the chain is, in a sense, pulling on the one before it. Disrupt any step and you get product accumulation upstream and substrate starvation downstream, both of which shift $\Delta G$ values in ways that can stall the whole pathway.

### Coupling Across the Whole Pathway

Chapter 1 showed coupling between two reactions. The same logic extends to an entire pathway. Glycolysis consists of ten sequential reactions. Thermodynamically, you can treat the whole pathway as a single coupled system, summing all ten $\Delta G$ values to get the net driving force for converting glucose to pyruvate. The intermediate steps don't have to be individually favorable as long as the overall sequence is. The thermodynamics of the whole pathway is what matters, and the pathway is held together by the chain of shared intermediates running from glucose all the way to pyruvate.

This is worth sitting with for a moment, because it changes how you think about metabolic regulation. The question isn't "is step 4 favorable?" The question is "is the flux through the whole pathway appropriate for what the cell needs right now?" Regulation works at the level of pathway flux, not individual reaction favorability, and the key regulatory points are almost always the irreversible steps.

---

## When It Breaks

### Metformin and Complex I

Metformin is the first-line drug for type 2 diabetes, taken by hundreds of millions of people. Its mechanism is still not completely understood, but a major component involves inhibiting Complex I of the mitochondrial electron transport chain.

Complex I is where NADH enters the electron transport chain; it accepts electrons from NADH and passes them down the chain toward oxygen. When metformin partially inhibits Complex I, NADH can't be reoxidized as efficiently. NADH accumulates, and the NADH/$\text{NAD}^+$ ratio rises.

Here's why that matters: glycolysis, pyruvate dehydrogenase, and the TCA cycle all require $\text{NAD}^+$ as an electron acceptor. When $\text{NAD}^+$ becomes scarce, these pathways slow down. Glucose is metabolized less efficiently, which reduces the ATP/AMP ratio. Low ATP/AMP activates AMPK (AMP-activated protein kinase), a master metabolic sensor that, among many other effects, suppresses hepatic gluconeogenesis (glucose synthesis in the liver); AMPK's full regulatory role is covered in Ch10. Less glucose output from the liver means lower blood glucose.

The downstream effects of partially tweaking a single electron transport complex ripple through NADH/$\text{NAD}^+$ balance, glycolysis, gluconeogenesis, and whole-body glucose homeostasis. You couldn't follow this chain of events without understanding what $\text{NAD}^+$ does, why its ratio to NADH matters, and how the thermodynamics of electron transfer connect to pathway flux. This is the chapter that makes that story readable.

### Thiamine Deficiency and the TCA Cycle

Thiamine (vitamin B₁) is a cofactor for three critical enzymes in oxidative metabolism: pyruvate dehydrogenase (which converts pyruvate to acetyl-CoA), alpha-ketoglutarate dehydrogenase (a TCA cycle enzyme), and transketolase (pentose phosphate pathway). All three are oxidative decarboxylation steps: they oxidize a substrate, release $\text{CO}_2$, and transfer electrons to $\text{NAD}^+$.

Thiamine deficiency shuts down all three. The result is a bottleneck at pyruvate: glucose can still be converted to pyruvate by glycolysis, but pyruvate can't be converted to acetyl-CoA and enter the TCA cycle. Pyruvate accumulates and is converted to lactate, producing lactic acidosis.

The neurological consequences, including Wernicke encephalopathy (confusion, eye movement abnormalities, and ataxia), reflect the fact that neurons are particularly dependent on aerobic glucose metabolism and have essentially no other fuel option. Thiamine deficiency is classic in chronic alcoholism and severe malnutrition. Treatment with IV thiamine can be dramatically effective if given early.

The mechanism is an $\text{NAD}^+$-dependent oxidation step that gets knocked out by losing a cofactor. Without it, the electrons that should move from pyruvate through NADH to the electron transport chain have nowhere to go, the redox cycle stalls, and the cell's aerobic energy metabolism collapses at the entry point to the TCA cycle.

---

## The MCAT Angle

**Reduction potential and spontaneity:** If $\Delta E^{\circ'}$ is positive (acceptor has higher $E^{\circ'}$ than donor), the reaction is spontaneous and $\Delta G^{\circ'}$ is negative. Electrons flow from low to high reduction potential. The equation $\Delta G^{\circ'} = -nF\Delta E^{\circ'}$ ties this directly to free energy.

**$\text{NAD}^+$ vs. NADPH:** They look similar but serve opposite metabolic roles. NADH carries electrons from catabolism to the electron transport chain. NADPH donates electrons for biosynthesis. Questions that confuse the two are common; always ask whether the context is breaking things down (catabolism, NADH) or building things up (anabolism, NADPH).

**The phosphate hierarchy:** Compounds above ATP in the hydrolysis hierarchy can phosphorylate ADP. Compounds below ATP get phosphorylated by ATP. PEP and 1,3-BPG are both above ATP, which is why they can drive substrate-level phosphorylation. Glucose-6-phosphate is below ATP, which is why hexokinase runs in the direction ATP → glucose-6-phosphate, not the other way.

**Coenzyme A and thioesters:** When you see acetyl-CoA or any acyl-CoA in a pathway, the thioester bond is what makes the subsequent reaction thermodynamically favorable. The "high-energy" thioester drives condensation, acyl transfer, and similar reactions much like ATP phosphoryl transfer drives phosphorylation.

**Irreversible steps as regulatory nodes:** If a question asks where in a metabolic pathway regulation is most likely to occur, look for the step with the largest negative $\Delta G$ under cellular conditions. That's the irreversible step, and irreversible steps are where cells put their throttles.

**Pathway $\Delta G$ is additive:** The total $\Delta G^{\circ'}$ for a multi-step pathway is the sum of the $\Delta G^{\circ'}$ values for all steps. A pathway can include steps with positive $\Delta G^{\circ'}$ as long as the sum is negative. The coupling is achieved through shared intermediates running the length of the pathway.

---

## Worked Problems

### Problem 1: Reduction Potential and Free Energy

The succinate dehydrogenase reaction in the TCA cycle oxidizes succinate to fumarate, passing electrons to FAD:

$$\text{Succinate} + \text{FAD} \rightarrow \text{Fumarate} + \text{FADH}_2$$

The $E^{\circ'}$ for the fumarate/succinate half-reaction is +0.03 V. The $E^{\circ'}$ for FAD/$\text{FADH}_2$ is 0 V (approximately, in this enzyme context).

(a) Which molecule is oxidized and which is reduced?

(b) Calculate $\Delta G^{\circ'}$ for the reaction (n = 2).

(c) In the electron transport chain, $\text{FADH}_2$ passes electrons to ubiquinone (coenzyme Q, a lipid-soluble electron carrier embedded in the inner mitochondrial membrane), which has an $E^{\circ'}$ of +0.045 V. Is this step thermodynamically favorable? Calculate $\Delta G^{\circ'}$.

**Solution:**

(a) Succinate loses electrons (gets oxidized to fumarate). FAD gains electrons (gets reduced to $\text{FADH}_2$). Fumarate is the oxidized form; succinate is the reduced form.

(b) The electron donor is succinate/fumarate ($E^{\circ'} = +0.03$ V). The acceptor is FAD/$\text{FADH}_2$ ($E^{\circ'} = 0$ V). Wait: we need to be careful about the direction. In the reaction as written, FAD is being reduced and succinate is being oxidized. So:

$$\Delta E^{\circ'} = E^{\circ'}_{\text{acceptor}} - E^{\circ'}_{\text{donor}} = 0 - (+0.03) = -0.03 \text{ V}$$

$$\Delta G^{\circ'} = -nF\Delta E^{\circ'} = -(2)(96.5)(-0.03) = +5.8 \text{ kJ/mol}$$

This is slightly endergonic under standard conditions. In the intact enzyme and under cellular conditions, the reaction is pulled forward by the subsequent reoxidation of $\text{FADH}_2$ at the electron transport chain.

(c) $\text{FADH}_2$ donates to ubiquinone (Q):

$$\Delta E^{\circ'} = E^{\circ'}_{Q} - E^{\circ'}_{\text{FADH}_2} = +0.045 - 0 = +0.045 \text{ V}$$

$$\Delta G^{\circ'} = -(2)(96.5)(+0.045) = -8.7 \text{ kJ/mol}$$

Negative: favorable. $\text{FADH}_2$ spontaneously reduces ubiquinone. This step releases free energy and contributes (modestly) to the proton gradient that drives ATP synthesis.

---

### Problem 2: The Phosphate Hierarchy

A student proposes the following reaction as an energy source:

$$\text{Glucose-6-phosphate} + \text{ADP} \rightarrow \text{Glucose} + \text{ATP}$$

$\Delta G^{\circ'}$ for glucose-6-phosphate hydrolysis = −13.8 kJ/mol
$\Delta G^{\circ'}$ for ATP hydrolysis = −30.5 kJ/mol

(a) Is this reaction thermodynamically favorable in the direction written?

(b) Explain this using the phosphate energy hierarchy.

(c) The reverse reaction (hexokinase phosphorylating glucose using ATP) is spontaneous. What is its $\Delta G^{\circ'}$?

**Solution:**

(a) To evaluate the reaction as written, calculate $\Delta G^{\circ'}$ for the net reaction. The reaction as written is the reverse of ATP hydrolysis plus the hydrolysis of glucose-6-phosphate:

$$\Delta G^{\circ'} = \Delta G^{\circ'}_{\text{G6P hydrolysis}} + \Delta G^{\circ'}_{\text{ADP phosphorylation}}$$

ADP phosphorylation is the reverse of ATP hydrolysis: $\Delta G^{\circ'} = +30.5$ kJ/mol.

$$\Delta G^{\circ'} = -13.8 + 30.5 = +16.7 \text{ kJ/mol}$$

Not favorable. This reaction doesn't go in the direction written.

(b) Glucose-6-phosphate sits below ATP in the phosphate energy hierarchy ($\Delta G^{\circ'}$ of hydrolysis −13.8 vs. −30.5 kJ/mol). Phosphate spontaneously transfers from higher-energy to lower-energy compounds, meaning from ATP down to glucose, not the other way. You can't use glucose-6-phosphate to make ATP because that would be moving phosphate uphill thermodynamically.

(c) The reverse reaction, ATP phosphorylating glucose to glucose-6-phosphate, simply has the opposite sign:

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

**1. $\text{NAD}^+$ gains electrons during glycolysis to become NADH. Why does that matter?**

Those electrons represent free energy that the cell hasn't captured yet. NADH carries them from the cytoplasm to the inner mitochondrial membrane, where the electron transport chain accepts them and passes them through a series of carriers of increasing reduction potential, ultimately to oxygen. The free energy released as electrons fall down this electrochemical gradient is used to pump protons across the inner membrane, creating a proton gradient. That gradient drives ATP synthase. The electrons that $\text{NAD}^+$ picks up from glycolysis are ultimately responsible for most of the ATP the cell makes from glucose oxidation. Without $\text{NAD}^+$, those electrons would have nowhere to go, glycolysis would stall, and the cell would be limited to the two net ATPs from substrate-level phosphorylation.

**2. If there are higher-energy phosphate compounds than ATP, why is ATP the universal currency?**

Because ATP sits in the middle of the phosphate energy hierarchy. High-energy phosphate compounds like PEP and 1,3-BPG, generated by catabolism, can donate their phosphate groups to ADP, recharging ATP. ATP then donates phosphate to low-energy acceptors, driving biosynthetic reactions and ion transport and mechanical work. A compound at the top of the hierarchy could only receive phosphate, never donate it to anything. A compound at the bottom could only receive ATP's phosphate, never generate ATP from catabolism. The middle position allows ATP to shuttle phosphate from producers (catabolism) to consumers (everything else). It's the universal currency precisely because it can be both spent and replenished.

---

*Chapter 10 (Glycolysis & Gluconeogenesis): This is where the toolkit gets used. Glycolysis is ten reactions: a mix of phosphoryl transfers, isomerizations, oxidation-reduction, and substrate-level phosphorylation, all linked by shared intermediates into a single thermodynamic unit. Every reaction type from Part IV shows up.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*

---

## Problem Set

**Problem 1.**
The following half-reactions are relevant to a hypothetical metabolic pathway:

| Half-reaction | $E^{\circ'}$ (V) |
|---|---|
| Compound A (oxidized) + $2\text{H}^+$ + $2e^-$ → Compound A (reduced) | −0.19 |
| Compound B (oxidized) + $2\text{H}^+$ + $2e^-$ → Compound B (reduced) | +0.12 |

(a) In the spontaneous direction, which compound is oxidized and which is reduced?

(b) Calculate $\Delta G^{\circ'}$ for the reaction (n = 2). Use $F = 96.5$ kJ/V·mol.

(c) If compound B (reduced) passes its electrons directly to oxygen ($E^{\circ'} = +0.82$ V), calculate $\Delta G^{\circ'}$ for that transfer. Compare the magnitude to the NADH-to-oxygen transfer calculated in the chapter, and explain why the values differ.

---

**Problem 2.**
$\text{NAD}^+$ and FAD both accept electrons from carbon substrates, but they are not interchangeable. For each scenario below, identify which carrier is used and explain why the other would not work. Use reduction potentials ($E^{\circ'}_{\text{NAD}^+/\text{NADH}} = -0.32$ V; $E^{\circ'}_{\text{FAD/FADH}_2} \approx 0$ V for the enzyme-bound form) to support your reasoning.

(a) Oxidation of a substrate whose half-reaction has $E^{\circ'} = -0.18$ V.

(b) Oxidation of a substrate whose half-reaction has $E^{\circ'} = +0.05$ V.

---

**Problem 3.** *(Synthesis)*
A newly characterized enzyme catalyzes the following reaction:

$$\text{Glucose-1-phosphate} + \text{ADP} \rightarrow \text{Glucose} + \text{ATP}$$

$\Delta G^{\circ'}$ for glucose-1-phosphate hydrolysis = −20.9 kJ/mol; $\Delta G^{\circ'}$ for ATP hydrolysis = −30.5 kJ/mol.

(a) Calculate $\Delta G^{\circ'}$ for this reaction as written. Is it spontaneous in the direction written?

(b) Now consider the reverse reaction: glucose + ATP → glucose-1-phosphate + ADP. Calculate $\Delta G^{\circ'}$. Is this spontaneous?

(c) The textbook's phosphate hierarchy lists PEP at −61.9 kJ/mol, ATP at −30.5 kJ/mol, and glucose-6-phosphate at −13.8 kJ/mol. Based only on hierarchy logic, predict whether each of the following transfers is spontaneous without calculation: (i) PEP → ADP, (ii) ATP → glycerol-3-phosphate, (iii) glucose-6-phosphate → ADP.

---

**Problem 4.** *(Synthesis)*
An enzyme in an obscure bacterium oxidizes succinate ($E^{\circ'} = +0.03$ V) using $\text{NAD}^+$ as the electron acceptor instead of FAD.

(a) Calculate $\Delta G^{\circ'}$ for this reaction.

(b) Explain why mammalian cells use FAD rather than $\text{NAD}^+$ for this oxidation, and what constraint on the reduction potential this imposes.

(c) Even granting that the bacterial enzyme actually does catalyze this reaction, what would be the energetic consequence at the level of ATP production if the $\text{FADH}_2$ that would normally be produced were replaced by NADH? Is this a benefit or a cost, and why?

---

**Problem 5.**
For each of the six metabolic reaction types listed in the chapter, identify one example from outside glycolysis or the TCA cycle (draw from the broader context of cell biology, digestion, nucleotide metabolism, or biosynthesis that is mentioned anywhere in the textbook). State which type it represents and explain in one sentence what the reaction accomplishes.

---

**Problem 6.** *(Synthesis)*
An enzyme catalyzes the reaction $X \rightarrow Y$ with $\Delta G^{\circ'} = +8.1$ kJ/mol. Under cellular conditions, [X] = 0.4 mM and [Y] = 0.01 mM. Temperature is 37°C (310 K, $R = 8.314$ J/mol·K).

(a) Calculate the actual $\Delta G$ under these cellular conditions.

(b) Is the reaction spontaneous? Justify your answer.

(c) A student argues: "Since $\Delta G^{\circ'}$ is positive, this reaction cannot be coupled to anything useful — you'd just be wasting energy trying to run it." Explain the flaw in this reasoning, using the relationship between $\Delta G^{\circ'}$ and actual $\Delta G$.

(d) A downstream enzyme in the same pathway is inhibited by a drug, causing [Y] to rise to 2.0 mM while [X] stays at 0.4 mM. Recalculate $\Delta G$ and describe what happens to flux through the $X \rightarrow Y$ step.

---

**Problem 7.**
Coenzyme A forms a thioester bond with acyl groups. The $\Delta G^{\circ'}$ for thioester hydrolysis is approximately −31 kJ/mol.

(a) How does thioester hydrolysis compare energetically to ATP hydrolysis? What does this mean for the types of reactions thioesters can drive?

(b) Acetyl-CoA is the substrate for the first step of the TCA cycle (citrate synthase). The reaction releases CoA. Using the concept of "high-energy bonds," explain why citrate synthase does not require ATP as an additional energy input.

(c) Fatty acid activation before beta-oxidation uses the reaction: fatty acid + CoA + ATP → fatty acyl-CoA + AMP + $\text{PP}_\text{i}$. The pyrophosphate ($\text{PP}_\text{i}$) is immediately hydrolyzed by pyrophosphatase. How many ATP equivalents are consumed in total, and why does this route provide a greater thermodynamic driving force than a reaction that would produce ADP + $\text{P}_\text{i}$?

---

**Problem 8.** *(Synthesis)*
Metformin partially inhibits Complex I of the electron transport chain, which accepts electrons from NADH and passes them down the chain.

(a) When Complex I is partially inhibited, what happens to the $\text{NADH}$/$\text{NAD}^+$ ratio?

(b) The chapter describes three metabolic pathways that require $\text{NAD}^+$ as an electron acceptor. Name them and explain how each is affected when $\text{NAD}^+$ becomes scarce.

(c) A patient takes a standard dose of metformin. A different patient takes an overdose. The first patient has controlled blood glucose; the second develops lactic acidosis. Using the reaction types and carrier functions from this chapter, trace the mechanism by which an extreme rise in $\text{NADH}$/$\text{NAD}^+$ leads to lactate accumulation.

---

## References

1. Berg JM, Tymoczko JL, Gatto GJ, Stryer L. *Biochemistry*, 9th ed. W.H. Freeman; 2019.
2. Nelson DL, Cox MM. *Lehninger Principles of Biochemistry*, 8th ed. W.H. Freeman; 2021.
3. Hinkle PC. P/O ratios of mitochondrial oxidative phosphorylation. *Biochim Biophys Acta*. 2005;1706(1-2):1-11. doi:10.1016/j.bbabio.2004.09.004
4. Owen MR, Doran E, Halestrap AP. Evidence that metformin exerts its anti-diabetic effects through inhibition of complex 1 of the mitochondrial respiratory chain. *Biochem J*. 2000;348(Pt 3):607-614. doi:10.1042/0264-6021:3480607
5. Zhou G, Myers R, Li Y, et al. Role of AMP-activated protein kinase in mechanism of metformin action. *J Clin Invest*. 2001;108(8):1167-1174. doi:10.1172/JCI13505
6. Rui L. Energy metabolism in the liver. *Compr Physiol*. 2014;4(1):177-197. doi:10.1002/cphy.c130024
7. Liesa M, Palacín M, Zorzano A. Mitochondrial dynamics in mammalian health and disease. *Physiol Rev*. 2009;89(3):799-845. doi:10.1152/physrev.00030.2008
8. Knowles JR, Albery WJ. Perfection in enzyme catalysis: the energetics of triosephosphate isomerase. *Acc Chem Res*. 1977;10(4):105-111. doi:10.1021/ar50112a001
9. Jitrapakdee S, Wallace JC. Structure, function and regulation of pyruvate carboxylase. *Biochem J*. 1999;340(Pt 1):1-16. doi:10.1042/bj3400001
10. Victor M, Adams RD, Collins GH. The Wernicke-Korsakoff Syndrome and Related Neurologic Disorders Due to Alcoholism and Malnutrition, 2nd ed. F.A. Davis; 1989.
11. Fattal-Valevski A. Thiamine (vitamin B1). *J Evid Based Complementary Altern Med*. 2011;16(1):12-20. doi:10.1177/1533210110392941
12. Kraut JA, Madias NE. Metabolic acidosis: pathophysiology, diagnosis and management. *Nat Rev Nephrol*. 2010;6(5):274-285. doi:10.1038/nrneph.2010.33
