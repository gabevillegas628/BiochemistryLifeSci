# Chapter 4: Enzymes and Catalysis

---

## Opener Questions

Think about these before you read. Come back to them at the end and see if your answer changed.

1. A farmer is brought to the emergency department by his family after collapsing in the field. He is drooling, his pupils are pinpoint, he is bradycardic, and he has fasciculations across his chest and arms. His family says he was spraying pesticides. The attending gives him atropine and calls the poison control center, which recommends adding pralidoxime (2-PAM) immediately. The toxicologist on the phone says: "If it has been more than a few hours, the 2-PAM won't do anything. Give it now or don't bother." What is happening at the molecular level, and why does timing matter for one of the antidotes but not the other?

2. Methotrexate is a drug used to treat rheumatoid arthritis, certain cancers, and ectopic pregnancies. It works by binding to an enzyme called dihydrofolate reductase (DHFR) roughly 1000 times more tightly than the enzyme's natural substrate does. Yet despite this enormous affinity advantage, giving more substrate can partially overcome methotrexate's effect. How is this possible? What does it tell you about the mechanism of drug action?

---

## The Big Picture

Chapter 3 established that proteins are binding machines. A protein has a binding site with a geometry and chemistry complementary to some target molecule, a ligand. The tightness of that interaction is captured by a single number, the $K_d$, and the fraction of sites occupied at any given ligand concentration follows a predictable curve. The chapter ended with hemoglobin, a protein that has taken the binding problem and added a layer of sophistication: cooperative binding, allostery, and the ability to integrate information from multiple ligands simultaneously.

But in Chapter 3, the protein and ligand separated unchanged. Hemoglobin binds oxygen, releases oxygen, and is identical before and after. This is only half the story of what proteins do.

The other half is **chemistry**. The same principles that govern binding, complementary shape, non-covalent interactions, the thermodynamics of association, also govern a more powerful class of event: the protein grabs a molecule, does something to it, and releases a chemically altered product. These proteins are **enzymes**, and the molecules they transform are **substrates**.

Enzymes are the reason biochemistry is not just thermodynamics. Thermodynamics tells you which reactions are possible ($\Delta G < 0$ means the reaction *must* proceed). But thermodynamics says nothing about how fast those reactions proceed. At body temperature, without enzymes, almost every metabolic reaction would proceed so slowly that life is impossible. The conversion of $\text{CO}_2$ and water to bicarbonate in red blood cells takes over 100 seconds without a catalyst, but the enzyme carbonic anhydrase completes it in under a millisecond. Life runs on enzyme-catalyzed timescales.

The through-line for this chapter is organophosphate poisoning. Organophosphates are a class of compounds that includes both agricultural pesticides (malathion, parathion) and nerve agents (sarin, VX). They work by permanently disabling a single enzyme: acetylcholinesterase. Understanding why that matters, and why the antidote works only within a narrow time window, requires a complete picture of how enzymes work, how fast they work, and how they can be blocked. By the end of this chapter, you will be able to explain the farmer's symptoms, the treatment, and the reason the toxicologist was so insistent about timing.

---

## Why Life Needs Catalysts

### Thermodynamics vs. Kinetics

Recall from Chapter 1 the distinction between thermodynamics and kinetics. Thermodynamics tells you about the final state: whether a reaction releases or requires free energy, and thus whether the equilibrium favors products or reactants. A reaction with a large negative $\Delta G$ is thermodynamically favorable: the products are much more stable than the reactants.

Kinetics tells you something entirely different: how fast the reaction proceeds. A reaction can be thermodynamically favorable and yet proceed imperceptibly slowly. The burning of glucose in air is enormously exergonic ($\Delta G$ is about $-2850$ kJ/mol), yet a glucose solution at room temperature is stable for years. No spontaneous combustion. The thermodynamics say it should burn; the kinetics say it will not, not without activation.

This distinction is not an academic subtlety. It is the central operating principle of metabolism. The cell maintains large thermodynamic gradients across many reactions simultaneously, and controls which ones actually proceed by deploying or withdrawing the enzymes that catalyze them. Metabolism is not just a set of favorable reactions running to completion; it is a carefully orchestrated network where enzyme activity, not thermodynamics, determines which pathways are active at any moment.

### The Activation Energy Problem

Why do thermodynamically favorable reactions often not proceed spontaneously? The answer is the **activation energy** ($E_a$), the energy that must be added to the system to get the reaction started.

Consider any chemical reaction converting substrate $S$ to product $P$. Even if $P$ is much lower in free energy than $S$ (so the reaction is thermodynamically favorable), the molecule must pass through an intermediate state before it can become $P$. This intermediate state, the **transition state** $X^{\ddagger}$, is not a stable species. It exists at the top of the free energy barrier between $S$ and $P$. Getting from $S$ to the transition state requires adding energy, $E_a$, even though the overall reaction releases energy.

Think of a boulder on a hillside. The boulder wants to roll to the valley (thermodynamically favorable), but it will not move unless you push it over the lip of the hill first (activation energy). Once over the lip, it rolls down on its own.

At physiological temperatures, molecules have thermal energy distributed across a Boltzmann distribution: a statistical spread in which most molecules have moderate energy but a small fraction have much higher energy. Only that small fraction have enough energy at any moment to surmount the activation energy barrier. This fraction determines the spontaneous rate. If the barrier is high, the reaction is slow regardless of how favorable the overall $\Delta G$ is.

### What a Catalyst Actually Does

A catalyst increases the rate of a reaction without being consumed by it. Critically, a catalyst does **not** change the thermodynamics: $\Delta G$, $\Delta H$, and $\Delta S$ for the overall reaction are identical whether or not a catalyst is present. The equilibrium position is unchanged. What a catalyst changes is the pathway from $S$ to $P$, specifically, it provides an alternative pathway with a **lower activation energy**.


A lower $E_a$ means a larger fraction of molecules have sufficient energy to reach the transition state at any given temperature. More molecules crossing the barrier per unit time means a faster reaction. Enzymes typically lower activation energies by 40 to 100 kJ/mol or more, which corresponds to observed rate enhancements of $10^{6}$ to $10^{17}$ over the uncatalyzed reaction.

Interestingly, because $\Delta G^{\circ'}$ cannot change (it is set by the intrinsic chemical properties of S and P, which the enzyme does not alter) an enzyme also cannot alter the equilibrium position of a reaction. To see why, recall

$$\Delta G = \Delta G^{\circ '} + RT ln\frac{[\text{P}]}{[\text{S}]}$$

At equilibrium the ratio of P to S is defined as $K_{eq}^{'}$ and $\Delta G=0$. Rearranging the equation above produces

$$\Delta G^{\circ '} = -RT ln(K_{eq}^{'})$$

In plain english, if $\Delta G^{\circ '}$ doesn't change, $K_{eq}^{'}$ **can't** change. Enzymes do not alter equilibrium, they **reduce the time required to reach the same equilibrium**.

Because the catalyst is not consumed, it can catalyze the same reaction over and over. One molecule of carbonic anhydrase can convert $10^6$ molecules of $\text{CO}_2$ per second. One molecule of catalase can decompose $4 \times 10^7$ molecules of hydrogen peroxide per second. The catalytic cycle regenerates the enzyme at the end of each turnover, ready for the next substrate molecule.

One more constraint: because catalysts do not change the equilibrium position, an enzyme that speeds up the forward reaction ($S \rightarrow P$) must also, by definition, speed up the reverse reaction ($P \rightarrow S$) to the same degree. The equilibrium constant is unchanged; only the speed of reaching that equilibrium changes. To see why, examine the following hypothetical reaction

$$ S \underset{k_R}{\overset{k_F}{\rightleftharpoons}} \text{P}$$

Recall that at equilibrium, it's not that *nothing* is occuring, but instead that it just *looks* like nothing is occurring. The equilibrium position is determined entirely by defining the concentrations at which the rate of the forward reaction ($V_F=k_F[\text{S}]$) is equal to the rate of the reverse reaction ($V_R=k_R[\text{P}]$). Setting these rates equal to each other and rearranging gives us:

$$\frac{k_F}{k_R} = \frac{[\text{P}]}{[\text{S}]} = K_{eq}^{'}$$

Since we have already established that an enzyme **cannot** change $K_{eq}^{'}$, any increase in the forward rate constant **must** be matched by the same proportional increase in the reverse rate constant.

---

## How Enzymes Work

### The Active Site

Enzymes are proteins. Their catalytic power comes from specific three-dimensional architecture. The part of the enzyme responsible for binding substrate and catalyzing chemistry is the **active site**: a cleft or pocket, usually formed by residues from non-adjacent parts of the polypeptide chain that are brought into proximity by the protein's tertiary structure.

The active site has two functional regions: the **binding site**, which recognizes and holds the substrate, and the **catalytic site**, which actually performs the chemistry. In practice these overlap considerably; the same residues often contribute to both recognition and catalysis.

Binding within the active site relies on the same non-covalent forces covered in Chapter 2: hydrogen bonds, van der Waals contacts, hydrophobic packing, and electrostatic interactions. The active site is exquisitely complementary to the substrate in shape, charge distribution, and hydrogen-bonding capacity. This complementarity is the molecular basis of **enzyme specificity**: why a given enzyme acts on one substrate (or one class of substrates) but not others.

The active site is typically a small fraction of the total enzyme surface. Most of the protein's mass is scaffold: structural architecture that positions the active site residues with the required precision and holds them there. Mutations far from the active site can abolish activity entirely by disrupting this scaffold.

### Transition State Stabilization

The most important insight about enzyme catalysis is that enzymes do not primarily stabilize the substrate. They stabilize the **transition state**.

Here is why this matters. The rate of a reaction depends on how often molecules reach the transition state. If the enzyme binds the transition state more tightly than it binds the substrate, it lowers the energy of the transition state relative to the substrate, which lowers $E_a$, which increases the rate. The tighter the enzyme binds the transition state, the faster the catalysis.

Crucially, the active site is complementary in shape and charge to the transition state, not to the ground-state substrate. The substrate fits reasonably well in the active site but the transition state fits much better. This is why enzymes are such powerful catalysts: they are optimized, by billions of years of evolution, to bind and stabilize the highest-energy point on the reaction coordinate.

This principle has practical consequences. Molecules that resemble the transition state in structure are expected to bind the active site with extremely high affinity because the active site was shaped to fit them. Many potent enzyme inhibitors are transition state analogs: stable molecules that mimic the geometric and electronic features of the transition state without actually being converted to product. They bind so tightly that they effectively shut off the enzyme.

### Induced Fit

Early descriptions of enzyme specificity used the **lock-and-key model**: the substrate fits the active site the way a key fits a lock, rigid complementary shapes. This is an oversimplification.

The more accurate model is **induced fit**: the active site is not rigid. When a substrate binds, it induces a conformational change in the enzyme that closes around the substrate, bringing catalytic residues into precisely the correct positions. The substrate also changes shape slightly to adopt its bound conformation.

The practical consequences of induced fit are significant. First, the enzyme can distinguish between a substrate and a substrate analog that differs by one group: a slightly wrong molecule may bind but not trigger the full conformational change, leaving catalytic residues out of position. Second, water molecules are often excluded from the active site during the closure, creating a microenvironment with very different properties (lower dielectric constant, precise acid/base residue positioning) than bulk solvent. This altered microenvironment is part of what makes the active site so effective at chemistry that would proceed only slowly in water.

### Catalytic Strategies

Enzymes use a relatively small repertoire of chemical mechanisms to accomplish an enormous diversity of reactions. The main strategies are:

**Acid-base catalysis.** Active site residues can donate or accept protons to stabilize charged intermediates or the transition state. Histidine is the most versatile acid-base catalyst in biology: its side chain $pK_a$ is close to 7, so at physiological pH it can exist in both protonated and unprotonated forms simultaneously. Glutamate, aspartate, lysine, and the N-terminal amine also participate in acid-base catalysis.

**Covalent catalysis.** The enzyme forms a transient covalent bond with the substrate, creating a covalent intermediate that is more reactive than the original substrate. This intermediate then breaks down to release product and regenerate the free enzyme. Serine proteases, enzymes that cleave peptide bonds using an active-site serine, include trypsin and chymotrypsin (digestive proteases) and the coagulation factors (blood-clotting enzymes covered in a later chapter). They work this way: a serine residue in the active site attacks the peptide bond, forming an acyl-enzyme intermediate before hydrolysis releases the product.

**Metal ion catalysis.** Many enzymes require metal ions (zinc, magnesium, iron, copper, manganese) at their active sites. Metal ions can stabilize negative charges on transition states, orient substrates for attack, or directly participate in redox chemistry. Carbonic anhydrase uses a zinc ion to activate a water molecule for nucleophilic attack on $\text{CO}_2$. Roughly one-third of all enzymes require a metal ion cofactor for activity.

**Proximity and orientation effects.** Simply bringing two reactant molecules into proximity in the correct orientation can accelerate a reaction dramatically even without any chemistry from the enzyme itself. An enzyme that holds two substrates in the optimal geometry for reaction achieves an effective concentration many orders of magnitude higher than would occur by diffusion alone. Estimates suggest that proximity and orientation effects alone could account for $10^3$ to $10^8$ fold rate enhancements.

In practice, most enzymes use several of these strategies simultaneously, and the combination of effects accounts for their enormous catalytic power.

---

## Enzyme Kinetics

### Setting Up the Problem

How do we measure enzyme activity? The simplest metric would be to observe the rate of the reaction, which at its simplest is just $V=\frac{\Delta [\text{P}]}{\Delta t}$. This, however, presents a bit of a problem because $V=k[\text{S}]$ and as the reaction proceeds $[\text{S}]$ decreases, therefore decreasing the rate. This is *further* complicated by the fact that we must also account for the reverse reaction, which will have an increasing rate as $[\text{P}]$ builds up, until both rates are equal and the system reaches equilibrium. We can remove both of these hurdles by examining the initial velocity $V_0$ at the beginning of the reaction, when product concentration is negligible and the back-reaction can be ignored, though $V_0$ still depends on the initial substrate concentration chosen.

If we measure $V_0$ at a series of starting substrate concentrations, $[\text{S}]$, holding enzyme concentration $[\text{E}]_T$ constant, we observe a characteristic pattern: $V_0$ increases with $[\text{S}]$ but the increase slows at higher concentrations and approaches a maximum, $V_{max}$. This looks like the hyperbolic binding curve from Chapter 3, and that similarity is not a coincidence.

### The Michaelis-Menten Model

How can we explain the shape of this graph? Leonor Michaelis and Maud Menten formalized the kinetic description of enzyme catalysis in 1913. Their model begins with the following reaction scheme:

$$\text{E} + \text{S} \underset{k_{-1}}{\overset{k_1}{\rightleftharpoons}} \text{ES} \overset{k_2}{\longrightarrow} \text{E} + \text{P}$$

The enzyme E binds substrate S to form an enzyme-substrate complex ES (with forward rate constant $k_1$ and reverse rate constant $k_{-1}$). The complex then undergoes catalysis to release product P and regenerate free enzyme (rate constant $k_2$, also called $k_{cat}$ for reasons we will return to shortly). Note that because we are examining only the initial rate, $[\text{P}]=0$ and so the reverse rate given by $V_R=k_{-2}[\text{E}][\text{P}]=0$ so we can ignore the rate constant $k_{-2}$ entirely.

The **steady-state assumption**, introduced by Briggs and Haldane, is the key to deriving the rate equation. In a typical enzyme assay, the enzyme is far less concentrated than the substrate. After a brief transient, the ES complex reaches a steady state where its formation and breakdown are balanced, so $\frac{d[\text{ES}]}{dt} = 0$. This is not an equilibrium; it is a dynamic steady state where the rate of ES formation equals the rate of ES breakdown.

Formation of ES:
$$\text{rate of formation} = k_1[\text{E}][\text{S}]$$

Breakdown of ES (by either reverse binding or catalysis and product release): rate of breakdown = k_{-1}[\text{ES}] + k_2[\text{ES}]$$

Setting formation equal to breakdown:
$$k_1[\text{E}][\text{S}] = (k_{-1} + k_2)[\text{ES}]$$

Grouping together the rate constants and concentrations:

$$\frac{k_{-1} + k_2}{k_1} = \frac{[\text{E}][\text{S}]}{[\text{ES}]}$$

To make our lives easier let's also define that mess of rate constants to be one variable, the **Michaelis constant** $K_M$.

$$K_M = \frac{[\text{E}][\text{S}]}{[\text{ES}]}$$


We cannot measure free enzyme $[\text{E}]$ directly, but we know that total enzyme is partitioned between free and bound forms:
$$[\text{E}]_T = [\text{E}] + [\text{ES}]$$

Substituting $[\text{E}] = [\text{E}]_T - [\text{ES}]$:

$$K_M = \frac{([\text{E}]_T - [\text{ES}])[\text{S}]}{[\text{ES}]}$$

Expanding and collecting $[\text{ES}]$ terms:

$$[\text{ES}](K_M + [\text{S}]) = [\text{E}_T][\text{S}]$$

Solving for $[\text{ES}]$:

$$[\text{ES}] = [\text{E}]_T\frac{[\text{S}]}{K_M + [\text{S}]}$$


The observed velocity $V_0$ is the rate at which ES breaks down to produce P:

$$V_0 = k_2[\text{ES}] = k_2[\text{E}]_T\frac{[\text{S}]}{K_m + [\text{S}]}$$

Define $V_{max} = k_2[\text{E}]_T$ (the maximum velocity when all enzyme is in the ES complex):

$$\boxed{V_0 = V_{max}\frac{[\text{S}]}{K_m + [\text{S}]}}$$

This is the **Michaelis-Menten equation**. It describes a rectangular hyperbola, and it should look familiar: it has exactly the same form as the binding equation $\theta = \frac{[\text{L}]}{K_d + [\text{L}]}$ from Chapter 3.

Note that the units of $K_M$ must be Molar, which of course makes sense given that $K_M = \frac{[\text{E}][\text{S}]}{[\text{ES}]}$ as shown above. So what does this concentration value mean? By setting $[\text{S}]=K_M$ we see that $V_0=\frac{1}{2}V_{max}$. In other words the Michaelis constant is the substrate concentration at which the enzyme operates at half its maximum velocity. This is the kinetic meaning of $K_M$.

### What $K_m$ Means and What It Is Not

$K_m$ is frequently described as the affinity of the enzyme for its substrate. This is approximately true but needs qualification.

If $k_2 \ll k_{-1}$ (the substrate dissociates much faster than it is converted to product), then $K_m \approx \frac{k_{-1}}{k_1} = K_d$, and $K_m$ is a genuine measure of binding affinity. In this limit, the Michaelis-Menten model reduces to a rapid-equilibrium model and $K_m = K_d$.

But in general, $K_m = \frac{k_{-1} + k_2}{k_1}$ includes the catalytic rate constant $k_2$ in the numerator. If $k_2$ is comparable to or greater than $k_{-1}$, $K_m$ overestimates the true $K_d$ for substrate binding. $K_m$ is a kinetic constant, not a true dissociation constant, though it approximates affinity when catalysis is slow relative to dissociation.

What you can say unambiguously: a smaller $K_m$ means the enzyme reaches half-maximal velocity at lower substrate concentration, which effectively means the enzyme is more efficient at low substrate concentrations. Comparing $K_m$ values across enzymes with similar substrates is a reasonable way to compare their apparent substrate affinity.

$K_m$ values in biology span a remarkable range: from nanomolar (for some highly regulated enzymes with tightly bound substrates) to millimolar (for enzymes that must operate at substrate concentrations set by cellular chemistry). Often the $K_m$ of an enzyme is close to the physiological substrate concentration in the cell. This is not coincidental. An enzyme operating near its $K_m$ is in the steepest part of the Michaelis-Menten curve and is most sensitive to changes in substrate concentration, which is exactly where you want an enzyme if you want its activity to respond to changes in metabolic state.

### $V_{max}$, $k_{cat}$, and Catalytic Efficiency

$V_{max}$ is the maximum velocity of the enzyme and is achieved when all enzyme molecules are occupied with substrate ($[\text{ES}] = [\text{E}]_T$). Since $V_{max} = k_2[\text{E}]_T$, $V_{max}$ depends on how much enzyme is present. To compare intrinsic catalytic power across enzymes or across conditions with different enzyme concentrations, we use $k_{cat}$, the **turnover number**:

$$k_{cat} = \frac{V_{max}}{[\text{E}]_T}$$

$k_{cat}$ is the number of substrate molecules converted to product per enzyme molecule per second at saturating substrate. It is an intrinsic property of the enzyme, independent of how much enzyme you have.

For simple one-step mechanisms like the Michaelis-Menten model above, $k_{cat} = k_2$. For more complex mechanisms with multiple steps, $k_{cat}$ reflects the rate-limiting step.

Some representative $k_{cat}$ values:
- Carbonic anhydrase: $\sim 10^6$ s$^{-1}$
- Catalase: $\sim 4 \times 10^7$ s$^{-1}$
- Acetylcholinesterase: $\sim 10^4$ s$^{-1}$
- Typical metabolic enzyme: $10^2$ to $10^3$ s$^{-1}$

Acetylcholinesterase's $k_{cat}$ of roughly 10,000 per second means one enzyme molecule hydrolyzes 10,000 acetylcholine molecules every second. This is exactly fast enough to terminate synaptic transmission and reset the neuromuscular junction after each action potential. This will be directly relevant when we return to organophosphate poisoning.

To compare different enzymes on the same substrate (or the same enzyme on different substrates), the most useful parameter is the **catalytic efficiency** $k_{cat}/K_m$:

$$\text{Catalytic efficiency} = \frac{k_{cat}}{K_m}$$

This ratio has units of $\text{M}^{-1}\text{s}^{-1}$ and represents how efficiently an enzyme converts substrate to product when substrate is dilute (well below $K_m$). When this is the case $K_m + [\text{S}] \approx K_m$ and so the Michaelis-Menten equation simplifies to

$$V_0=V_{max}\frac{[\text{S}]}{K_m}$$

Substituting $V_{max} = k_{cat}[\text{E}]_T$ and rearranging yields

$$V_0 = \frac{k_{cat}}{K_m}[\text{S}][\text{E}]_T$$

We can see then that in this low-substrate regime, $k_{cat}/K_m$ is effectively the second-order rate constant for the productive encounter of enzyme and substrate. The higher the value, the more productive encounters we observe and so the higher the effeciency of that enzyme to that particular substrate.

The upper limit on $k_{cat}/K_m$ is set by the diffusion limit: enzyme and substrate cannot encounter each other faster than diffusion allows, roughly $10^8$ to $10^9 \text{M}^{-1}s^{-1}$. Enzymes that have reached this limit are called **catalytically perfect**: they are so good at catalysis that the only thing limiting their speed is how fast substrate diffuses to the active site. Acetylcholinesterase and catalase are examples of near-perfect enzymes, with $k_{cat}/K_m$ approaching $10^8 \text{M}^{-1}s^{-1}$.

### The Lineweaver-Burk Plot

The Michaelis-Menten equation is a hyperbola. Estimating $K_m$ and $V_{max}$ from a hyperbolic curve by eye is imprecise: $V_{max}$ is an asymptote never actually reached, and the curve around the $K_m$ region is gradual. Hans Lineweaver and Dean Burk proposed a useful transformation in 1934.

Take the reciprocal of both sides of the Michaelis-Menten equation:

$$\frac{1}{V_0} = \frac{K_m + [\text{S}]}{V_{max}[\text{S}]} = \frac{K_m}{V_{max}} \cdot \frac{1}{[\text{S}]} + \frac{1}{V_{max}}$$

This is a linear equation in $\frac{1}{[\text{S}]}$. A plot of $\frac{1}{V_0}$ vs. $\frac{1}{[\text{S}]}$ (the **Lineweaver-Burk plot** or **double-reciprocal plot**) gives a straight line with:

- Slope: $\frac{K_m}{V_{max}}$
- y-intercept: $\frac{1}{V_{max}}$
- x-intercept: $-\frac{1}{K_m}$

From these intercepts, $K_m$ and $V_{max}$ can be read off directly. The Lineweaver-Burk plot also makes enzyme inhibition visually interpretable: different types of inhibitors produce characteristic changes in the slope and intercepts, as we will see next.

*Note: Lineweaver-Burk plots amplify error at low substrate concentrations (large $1/[\text{S}]$ values), where experimental measurements are least reliable. Modern enzyme kinetics uses nonlinear regression on the untransformed Michaelis-Menten data, but the double-reciprocal plot remains valuable conceptually and is heavily tested on the MCAT/DAT.*

---

## Enzyme Inhibition

Enzyme inhibition is not merely an academic topic. Every drug that targets an enzyme, and there are hundreds of them, is an enzyme inhibitor. Understanding how inhibitors work, and how their effects appear in kinetic data, is foundational to understanding pharmacology.

Inhibitors are classified by their mechanism of action and by whether they bind reversibly or irreversibly and can be classified into 3 categories depending on their effects on enzyme kinetics:

1. **Competitive inhibition**: the inhibitor competes with substrate for the active site; increasing $[\text{S}]$ can overcome it
2. **Uncompetitive inhibition**: the inhibitor binds only the ES complex; increasing $[\text{S}]$ makes it worse
3. **Noncompetitive inhibition**: the inhibitor binds a separate site on both free enzyme and ES; increasing $[\text{S}]$ has no effect

### Competitive Inhibition

A **competitive inhibitor** competes directly with the substrate for the active site. Because the inhibitor and substrate compete for the same binding site, increasing substrate concentration can overcome inhibition: flood the active site with substrate and the inhibitor gets outcompeted. This is the defining characteristic of competitive inhibition.

The competitive inhibitor binds free enzyme, not the ES complex. Its binding is described by an inhibitor dissociation constant $K_i$ (effecitvely the $K_a$ of the inhibtor for this enzyme):

$$\text{E} + \text{I} \rightleftharpoons \text{EI} \quad K_i = \frac{[\text{E}][\text{I}]}{[\text{EI}]}$$

With competitive inhibitor present, some enzyme is sequestered as EI and unavailable to bind substrate. The quantitative effect on the Michaelis-Menten equation is:

$$V_0 = \frac{V_{max}[\text{S}]}{\alpha K_m + [\text{S}]}$$

where $\alpha = 1 + \frac{[\text{I}]}{K_i}$. The apparent $K_m$ increases by a factor of $\alpha$; $V_{max}$ is unchanged.

On a Lineweaver-Burk plot, competitive inhibition rotates the line around the y-intercept: the y-intercept ($1/V_{max}$) is unchanged, the slope increases (apparent $K_m$ increases), and the x-intercept moves toward zero (apparent $K_m$ is larger so $-1/K_m$ is smaller in magnitude).

Why does the $K_m$ value increase in competitive inhibition? The answer is somewhat intuitive. Let's say that in the absence of inhibitor we have the nominal $K_m$ and recall that $K_m=[\text{S}]$ when $V_0=V_{max}/2$. In the presence of a competitive inhibitor, $S$ is now competing with $I$ for the active site and so more $S$ is required to achieve the same $V_0$ as without inhibitor. Thus a higher $[\text{S}]$ is required to reach $V_{max}/2$, causing the apparent increase in $K_m$. This new apparent $K_m$ value is referred to as $K_m^{app}$. $V_{max}$ remains unchanged, however: the same maximum velocity is achievable since $[\text{E}]_T$ is unchanged; it simply requires a higher $[\text{S}]$ to get there.

**Clinical example: statins.** HMG-CoA reductase catalyzes the rate-limiting step in cholesterol biosynthesis, the conversion of HMG-CoA to mevalonate. Statins (atorvastatin, rosuvastatin, etc.) are competitive inhibitors of this enzyme. Their molecular structure mimics the transition state of the reaction, giving them higher affinity for the active site than the natural substrate. With the enzyme partially inhibited, the liver produces less cholesterol and upregulates LDL receptors to import cholesterol from the blood, lowering plasma LDL. The key feature: competitive inhibition is in principle reversible and dose-dependent, so the therapeutic effect can be titrated.

**Second example: methotrexate.** Dihydrofolate reductase (DHFR) converts dihydrofolate to tetrahydrofolate, a cofactor required for nucleotide synthesis. Methotrexate is a competitive inhibitor of DHFR with roughly 1000-fold higher affinity than the natural substrate dihydrofolate. At therapeutic doses, the enzyme is largely occupied by methotrexate. Rapidly dividing cells (cancer cells, immune cells) are preferentially affected because they require more nucleotides. Critically: because the inhibition is competitive, very high doses of the substrate analog leucovorin (folinic acid, a downstream product that bypasses the blocked step) can partially rescue normal cells after high-dose methotrexate therapy. This is the basis for "leucovorin rescue" in oncology protocols. The revisiting of the opener question about methotrexate should now be answerable: competitive inhibition is always in principle overcome by enough substrate, which is why adding product analogs can partially rescue cells even when inhibitor affinity is very high.

### Uncompetitive Inhibition

An **uncompetitive inhibitor** binds ONLY the enzyme-substrate complex (ES), not free enzyme. It cannot bind the active site when it is empty. This seems counterintuitive: how can binding away from the substrate binding site depend on whether substrate is present? The answer is induced fit: substrate binding causes a conformational change that creates or exposes a binding site for the inhibitor elsewhere on the enzyme.

The uncompetitive inhibitor traps the ES complex, preventing it from proceeding to product:

$$\text{ES} + \text{I} \rightleftharpoons \text{ESI (inactive)}$$

The quantitative effect:

$$V_0 = \frac{V_{max}/\alpha'}{K_m/\alpha' + [\text{S}]}$$

where $\alpha' = 1 + \frac{[\text{I}]}{K_i'}$. Both $V_{max}$ and $K_m$ are decreased by the same factor $\alpha'$. The ratio $V_{max}/K_m$ is unchanged.

On a Lineweaver-Burk plot, uncompetitive inhibition shifts the line parallel upward: same slope, higher y-intercept, x-intercept moves right. Parallel lines on a double-reciprocal plot are the diagnostic signature of uncompetitive inhibition.

A striking and initially puzzling consequence: uncompetitive inhibition actually decreases the apparent $K_m$ (because the inhibitor traps ES, effectively pulling the equilibrium toward ES and increasing apparent affinity), yet also decreases $V_{max}$. Adding more substrate makes things worse, not better, because more substrate drives more ES formation, which gives the inhibitor more ES to trap. This means, unlike competitive inhibition, uncompetitive inhibition cannot be overcome by adding more substrate.

### Noncompetitive (Mixed) Inhibition

A **noncompetitive inhibitor** binds both free enzyme and the ES complex, typically at a site other than the active site (an allosteric site). If it binds both with equal affinity, it is pure noncompetitive inhibition. If it binds with different affinities for E vs. ES, it is **mixed inhibition**.

For pure noncompetitive inhibition, the inhibitor does not prevent substrate binding (so $K_m$ is unchanged) but reduces the fraction of ES that can proceed to product (so $V_{max}$ is reduced):

$$V_0 = \frac{V_{max}/\alpha}{K_m + [\text{S}]}$$

On a Lineweaver-Burk plot, noncompetitive inhibition rotates the line around the x-intercept: y-intercept increases (lower $V_{max}$), slope increases, but x-intercept is unchanged (same $K_m$). Adding more substrate does not help because the inhibitor does not compete with substrate. $V_{max}$ is simply reduced.

The three reversible inhibition types are summarized:

| Inhibitor Type | Binds | Effect on $K_m$ | Effect on $V_{max}$ | Lineweaver-Burk |
|---|---|---|---|---|
| Competitive | Free E | Increases | Unchanged | Same y-int, higher slope |
| Uncompetitive | ES complex | Decreases | Decreases | Parallel shift up |
| Noncompetitive | E and ES | Unchanged | Decreases | Same x-int, higher y-int |

*Mnemonic: competitive inhibitors increase apparent $K_m$ because the enzyme "thinks" the substrate is less abundant (it has to compete with inhibitor). Noncompetitive inhibitors reduce $V_{max}$ because some fraction of enzyme is permanently unproductive regardless of substrate concentration.*

### Irreversible Inhibition

Reversible inhibitors dissociate from the enzyme and reach a dynamic equilibrium. Irreversible inhibitors form a stable, often covalent, bond with the enzyme that does not break under physiological conditions. Once an enzyme molecule is irreversibly inhibited, it is permanently inactivated.

Irreversible inhibitors reduce the total amount of functional enzyme ($[\text{E}]_T$), which reduces $V_{max}$ proportionally (since $V_{max} = k_{cat}[\text{E}]_T$). $K_m$ is not affected: the remaining uninhibited enzyme molecules still bind substrate with the same affinity and turn it over at the same rate; there are just fewer of them.

Many irreversible inhibitors are **mechanism-based inhibitors** (also called suicide inhibitors or $k_{cat}$ inhibitors): they enter the active site as substrates, are partially processed by the enzyme's catalytic machinery, and then the partially processed intermediate forms a stable covalent bond with an active site residue. The enzyme essentially destroys itself by doing its job. Aspirin (acetylsalicylic acid) is a classic example: it irreversibly acetylates a serine residue in the active sites of cyclooxygenase-1 and cyclooxygenase-2 (COX-1 and COX-2), permanently inactivating the enzyme. Since platelets lack a nucleus and cannot synthesize new COX protein, aspirin's antiplatelet effect lasts for the entire lifespan of the platelet (8 to 10 days).

The organophosphates, our clinical through-line, work through irreversible inhibition of acetylcholinesterase. We will return to the full picture shortly.

---

## Regulation of Enzyme Activity

### Why Enzymes Need to Be Regulated

A cell cannot simply run all metabolic reactions at maximum speed all the time. The rate of any metabolic pathway must be matched to cellular demand: fast enough when the demand is high, slow enough not to waste resources when demand is low. This requires real-time control of enzyme activity.

There are two general strategies: change how much enzyme is present (gene expression, protein synthesis, protein degradation) which effecitvely reduces $[\text{E}]_T$ and thus $V_{max}$; or change the activity of existing enzyme molecules. Gene expression responses are slow, on the scale of minutes to hours. Activity regulation of existing enzymes is fast, on the scale of milliseconds to seconds. For fine-grained real-time control of metabolism, enzymes must be regulatable at the protein level.

### Allosteric Regulation

Recall from Chapter 3 that hemoglobin is an allosteric protein: binding of a ligand (oxygen, 2,3-BPG, $H^+$) at one site changes the binding properties of distant sites. Enzymes are also allosteric, and the same principles apply.

An **allosteric enzyme** has one or more **regulatory sites** distinct from the active site. When a small molecule (**allosteric effector** or **allosteric modulator**) binds the regulatory site, it changes the enzyme's conformation and thus its activity. Allosteric activators increase activity; allosteric inhibitors decrease it.

Allosteric enzymes often display sigmoidal kinetics (like hemoglobin's sigmoidal oxygen binding curve) rather than hyperbolic Michaelis-Menten kinetics. This arises because allosteric enzymes are typically oligomers with cooperativity between subunits: binding of substrate at one subunit increases (or decreases) affinity at other subunits. Sigmoidal kinetics has a steep response in a defined concentration range, which makes the enzyme a highly sensitive switch rather than a gradual responder.

The two-state model (T-state and R-state, as in hemoglobin) applies directly:

- **T-state (tense)**: low affinity, low activity
- **R-state (relaxed)**: high affinity, high activity
- Allosteric activators shift equilibrium toward R-state
- Allosteric inhibitors shift equilibrium toward T-state

A classic example: aspartate transcarbamoylase (ATCase) catalyzes the first committed step in pyrimidine biosynthesis (the pathway that makes the nucleotide building blocks cytosine, uracil, and thymine, required for DNA and RNA synthesis). It is inhibited allosterically by CTP (cytidine triphosphate, one of the end products of this pathway). When CTP builds up, it binds an allosteric site on ATCase and shifts the enzyme toward the T-state, slowing pyrimidine synthesis. When CTP is depleted, the enzyme shifts back to R-state and synthesis accelerates. This is **feedback inhibition**: the product of a pathway inhibits an enzyme early in that pathway, maintaining steady-state concentration.

### Covalent Modification: Phosphorylation

A second major mechanism of real-time enzyme regulation is **covalent modification**. Rather than an allosteric effector molecule binding non-covalently, another enzyme chemically modifies the target enzyme, changing its activity.

The most common covalent modification in signaling is **phosphorylation**: addition of a phosphate group to the hydroxyl group of a serine, threonine, or tyrosine residue, catalyzed by a **protein kinase**, and reversed by a **protein phosphatase**.

Phosphorylation is ideal as a regulatory switch for several reasons:

1. It introduces a large, doubly charged group ($-\text{OPO}_3^{2-}$ at physiological pH) into the local environment of a residue. This can disrupt local hydrogen bonding networks, change the surface charge of the protein, and shift the conformational equilibrium between active and inactive states.
2. It is reversible on timescales of seconds to minutes, controlled by the opposing activities of kinases and phosphatases.
3. It is amplifiable: a single signaling event can activate a kinase, which phosphorylates and activates other kinases, creating a **kinase cascade** that amplifies a small signal into a large cellular response. We will examine several kinase cascades in a later chapter.

Importantly, the same phosphorylation can activate some enzymes and inhibit others, depending on where the phosphorylated residue is and how its modification affects the protein's structure. Glycogen phosphorylase (which breaks down glycogen, the branched glucose polymer used for short-term energy storage in liver and muscle) is activated by phosphorylation; glycogen synthase (which builds glycogen) is inhibited by phosphorylation. Both enzymes are phosphorylated by the same kinase, protein kinase A (a kinase activated by the second messenger cAMP), in response to epinephrine (the "fight-or-flight" hormone released by the adrenal glands, covered in the signal transduction chapter), simultaneously turning on glycogen breakdown and turning off glycogen synthesis, a phenomenon known as **reciprocal regulation**; there would be no point in having both pathways turned on. The cell integrates a single hormonal signal into a coordinated metabolic response through phosphorylation of multiple target enzymes.

### Feedback Inhibition and Metabolic Control

Metabolic pathways are not isolated: they are interconnected networks, and the output of one pathway is often the input of another. **Feedback inhibition** is a general mechanism for maintaining homeostasis in these networks.

In the simplest form, the end product of a pathway inhibits the first committed (irreversible) step. This makes thermodynamic sense: once you have enough of the product, slow down the part of the pathway that committed you to making it. The inhibition is allosteric: the product binds a regulatory site on the first committed enzyme and shifts it toward lower activity.

The first committed step is the logical control point for two reasons. First, it is the step that most directly commits resources to the pathway: everything upstream is reversible and shared with other pathways, but once this step occurs, the molecules are on their way to the endpoint. Inhibiting this step conserves upstream intermediates for other uses. Second, inhibiting a downstream step wastes the intermediate between the inhibited step and the beginning of the pathway, whereas inhibiting the first committed step wastes nothing.

---

## Putting It Together: Organophosphate Poisoning

### Background: The Neuromuscular Junction

To follow the organophosphate story, you need a working model of where acetylcholine matters most.

A **motor neuron** is a nerve cell whose axon terminates at a skeletal muscle fiber at a specialized contact called the **neuromuscular junction (NMJ)**. Signaling across the NMJ is electrical-then-chemical: an **action potential** (a brief voltage spike that propagates along the neuron's membrane) reaches the axon terminal and triggers the release of **acetylcholine (ACh)**, a small-molecule neurotransmitter, into the **synaptic cleft** (the narrow gap between the neuron and the muscle). ACh diffuses across the cleft and binds receptors on the muscle side, called the **motor end plate**, triggering membrane depolarization and muscle contraction.

Acetylcholine receptors come in two families. **Nicotinic receptors** are ion channels: they open directly when ACh binds, allowing ions to flow and depolarizing the membrane. They are found at the neuromuscular junction and at autonomic ganglia. **Muscarinic receptors** are G-protein coupled receptors found on smooth muscle, cardiac muscle, and glands; when activated, they slow the heart, stimulate secretions, and contract smooth muscle. The symptoms of organophosphate poisoning map directly onto which receptor type is being overstimulated in which tissue.

For the muscle to respond to the next signal, ACh must be rapidly cleared from the cleft. That is the job of acetylcholinesterase.

### Acetylcholinesterase and Synaptic Transmission

The neuromuscular junction works on a tight timing cycle. A motor neuron fires an action potential. The action potential triggers release of acetylcholine (ACh) into the synaptic cleft. ACh diffuses to the motor end plate, binds nicotinic acetylcholine receptors, depolarizes the muscle, and triggers contraction. Then ACh must be rapidly removed from the cleft so the receptor can reset before the next action potential.

Removal of ACh is accomplished almost entirely by **acetylcholinesterase (AChE)**, an enzyme embedded in the basement membrane of the synapse. AChE hydrolyzes ACh to choline and acetate, both of which are recycled. The $k_{cat}$ of AChE is approximately $10^4$ $s^{-1}$, and it operates near the diffusion limit as noted earlier. AChE can clear the ACh from the synaptic cleft in under 1 millisecond! This extraordinarily fast hydrolysis is what allows tight, precise control of muscle contraction.

AChE is a serine hydrolase: it uses a serine residue in the active site to form a covalent acyl-enzyme intermediate, which is then hydrolyzed by water to regenerate free enzyme. The cycle: ACh enters the active site, serine attacks the carbonyl carbon of the ester bond, acetate leaves with the proton from serine, the acetyl group is transferred to serine forming the acetyl-enzyme intermediate, water attacks and hydrolyzes the intermediate, and the enzyme is regenerated, having consumed about 100 microseconds total.

### Organophosphate Mechanism

Organophosphate compounds (OPs) such as sarin, tabun, VX, malathion, and parathion share a common core structure: a phosphorus atom with a good leaving group. When an OP enters the active site of AChE, the same serine residue that attacks acetylcholine now attacks the phosphorus, displacing the leaving group:

$$\text{AChE-Ser-OH} + \text{OP} \rightarrow \text{AChE-Ser-O-P(O)(OR)(OR')} + \text{leaving group}$$

The phosphorylated serine is chemically very different from the acetylated serine in the normal catalytic cycle. The acetyl-enzyme intermediate is hydrolyzed in microseconds. The phosphoryl-enzyme intermediate is extremely stable: hydrolysis is so slow (half-life of hours in some cases) that the enzyme is effectively inactivated permanently. This is irreversible inhibition by a mechanism-based (suicide) inhibitor.

### The Clinical Consequence: Cholinergic Crisis

With AChE inactivated, ACh is not cleared from synapses. It accumulates, and nicotinic and muscarinic acetylcholine receptors remain continuously stimulated. The clinical syndrome is a **cholinergic crisis**:

**Muscarinic effects** (smooth muscle, glands, heart): bradycardia (abnormally slow heart rate), bronchospasm (constriction of the airways), increased secretions (salivation, lacrimation, urination, defecation, GI motility), miosis (pupillary constriction). The mnemonic SLUDGE covers the secretory/GI effects: Salivation, Lacrimation, Urination, Defecation, GI distress, Emesis.

**Nicotinic effects** (neuromuscular junction, autonomic ganglia): muscle fasciculations (initial excessive stimulation), progressing to paralysis as the motor end plate cannot repolarize. Respiratory failure from paralysis of the diaphragm is the primary cause of death.

The farmer in the opening question has pinpoint pupils (muscarinic, miosis), bradycardia (muscarinic), excess salivation (muscarinic), and fasciculations progressing toward paralysis (nicotinic). The picture is a cholinergic crisis from AChE inhibition.

### The Antidotes: Two Different Mechanisms

Treatment involves two agents that work by completely different mechanisms.

**Atropine** is a muscarinic acetylcholine receptor antagonist. It competes with ACh for the muscarinic receptor binding site (competitive inhibition at the receptor level, not the enzyme level). Even though ACh is accumulating because AChE is inhibited, atropine outcompetes ACh for the receptor and blocks the muscarinic effects: it dries secretions, reverses bradycardia, dilates the pupils, and reduces bronchospasm. Atropine does not address the underlying enzyme problem and does not reverse nicotinic effects (so it does not directly treat muscle paralysis), but it buys time and addresses the immediate life threats. Atropine can be given at any time after OP exposure and will work as long as receptors are present; there is no time window issue.

**Pralidoxime (2-PAM)** works by a completely different mechanism. It does not antagonize a receptor. Instead, it reactivates AChE directly. 2-PAM enters the active site and attacks the phosphorus atom of the phosphorylated serine, removing the OP group and regenerating the free enzyme:

$$\text{AChE-Ser-O-P} + \text{2-PAM} \rightarrow \text{AChE-Ser-OH} + \text{2-PAM-P}$$

This restores functional AChE, which can then hydrolyze the accumulated ACh. Reactivating even a fraction of AChE molecules has an outsized effect because AChE's $k_{cat}$ is so high: even 10% of normal AChE activity may be sufficient to restore synaptic clearance.

### The Aging Problem: Why Timing Matters

Here is the molecular basis of the toxicologist's urgency from the opener. The phosphorylated AChE complex undergoes a slow spontaneous reaction called **aging**: one of the ester groups on the phosphorus is hydrolyzed, leaving a charged phosphonate group on the serine. The aged complex is even more stable and is resistant to 2-PAM reactivation. Once aging occurs, 2-PAM cannot remove the phosphoryl group.

The rate of aging depends on the specific OP compound. For tabun (a nerve agent), the aging half-life is on the order of 14 hours, meaning significant but not complete aging occurs within a day of exposure. For soman (another nerve agent), aging is essentially complete within minutes of exposure. For common agricultural OPs like malathion, aging takes longer, on the scale of a day or more. For all of them, the window is finite.

This is why the toxicologist said "give it now or don't bother." After aging, 2-PAM is useless: the covalent modification has been transformed into a form that cannot be reversed by the drug. Atropine, which works at the receptor and not the enzyme, remains effective regardless of whether aging has occurred. But 2-PAM requires that the phosphoryl-enzyme complex still be in the pre-aged form.

The full treatment picture for OP poisoning: atropine to block muscarinic effects immediately, 2-PAM to reactivate AChE before aging occurs, and benzodiazepines (a class of CNS depressant drugs that enhance inhibitory signaling and reduce neuronal excitability, used here to control seizures from excessive ACh at central synapses). Supportive care, including ventilation, addresses the nicotinic-mediated respiratory paralysis that atropine cannot reverse.

---

## Worked Problems

**Problem 1.** An enzyme has a $K_m$ of 2 mM and a $V_{max}$ of 120 nmol/min. You run the reaction at $[\text{S}] = 2$ mM. What is $V_0$? Then you add a competitive inhibitor such that $\alpha = 3$. What is the new apparent $K_m$, and what is $V_0$ under these conditions?

*Part 1 — no inhibitor:*

$$V_0 = \frac{V_{max}[\text{S}]}{K_m + [\text{S}]} = \frac{120 \times 2}{2 + 2} = \frac{240}{4} = 60 \text{ nmol/min}$$

At $[\text{S}] = K_m$, the enzyme is always at half-maximal velocity, so $V_0 = 60$ nmol/min. This is a useful shortcut worth memorizing.

*Part 2 — competitive inhibitor, $\alpha = 3$:*

The apparent $K_m$ becomes $\alpha K_m = 3 \times 2 = 6$ mM. $V_{max}$ is unchanged at 120 nmol/min.

$$V_0 = \frac{120 \times 2}{6 + 2} = \frac{240}{8} = 30 \text{ nmol/min}$$

The same substrate concentration now yields half the velocity, because the inhibitor is competing successfully at these concentrations. To recover the original $V_0$ of 60 nmol/min, you would need to raise $[\text{S}]$ to 6 mM (the new $K_m$), which confirms the defining feature of competitive inhibition: it can be overcome with enough substrate.

---

**Problem 2.** You are characterizing a new drug candidate and run Michaelis-Menten experiments with and without the drug. You obtain the following Lineweaver-Burk data:

| Condition | y-intercept ($1/V_{max}$) | x-intercept ($-1/K_m$) |
|---|---|---|
| No drug | 0.010 | $-0.50$ |
| With drug | 0.020 | $-0.50$ |

What type of inhibition does this drug produce? What are $K_m$ and $V_{max}$ in each condition?

*Reading the intercepts:*

No drug: $V_{max} = 1/0.010 = 100$ units; $K_m = 1/0.50 = 2$ mM.

With drug: $V_{max} = 1/0.020 = 50$ units; $K_m = 1/0.50 = 2$ mM.

The y-intercept doubled (so $V_{max}$ was halved) but the x-intercept is identical (so $K_m$ is unchanged). From the inhibition table: unchanged $K_m$, decreased $V_{max}$ — this is **noncompetitive inhibition**. The drug binds a site other than the active site, reducing the fraction of ES that can proceed to product, but does not interfere with substrate binding.

*Clinical implication:* Because $K_m$ is unchanged, adding more substrate will not rescue enzyme activity. This drug's effect cannot be overcome by increased substrate concentration, which may be a pharmacological advantage if you want durable inhibition regardless of local substrate levels.

---

**Problem 3.** Soman is an organophosphate nerve agent with an aging half-life of approximately 2 minutes. A soldier is exposed and receives 2-PAM exactly 10 minutes after exposure. Assuming aging follows first-order kinetics, approximately what fraction of AChE is still reactivatable at the time 2-PAM is administered?

For first-order decay, the fraction remaining in the pre-aged (reactivatable) form after time $t$ is:

$$f = \left(\frac{1}{2}\right)^{\frac{t}{t_{1/2}}}$$

With $t = 10$ min and $t_{1/2} = 2$ min:

$$f = \left(\frac{1}{2}\right)^{10/2} = \left(\frac{1}{2}\right)^{5} = \frac{1}{32} \approx 3\%$$

Only about 3% of the AChE-soman complex remains reactivatable. The 2-PAM will have essentially no clinical effect. This is why field treatment protocols for soman exposure call for antidote administration within the first minute of exposure, and why autoinjectors containing both atropine and 2-PAM are pre-loaded for immediate self-injection. Atropine should still be given aggressively since it acts at the receptor and is not affected by aging, but the window for enzymatic rescue with 2-PAM has already closed.

---

## Summary

Enzymes solve the kinetics problem that thermodynamics cannot: they accelerate reactions that are favorable but proceed too slowly without catalysis. They do this by binding and stabilizing the transition state, lowering the activation energy without changing the thermodynamics of the overall reaction.

Enzyme kinetics, described by the Michaelis-Menten equation, gives us two parameters that characterize any enzyme-substrate pair: $K_m$ (the substrate concentration at half-maximal velocity, an approximation of substrate affinity) and $V_{max}$ (the maximum velocity at saturating substrate, proportional to $k_{cat}$, the turnover number). Catalytic efficiency $k_{cat}/K_m$ is the best single measure of enzyme performance at low substrate concentrations and approaches a maximum set by the diffusion limit.

Inhibitors modulate enzyme activity by altering $K_m$, $V_{max}$, or both:
- Competitive inhibitors increase apparent $K_m$ (substrate can outcompete them)
- Uncompetitive inhibitors decrease both $K_m$ and $V_{max}$
- Noncompetitive inhibitors decrease $V_{max}$ without affecting $K_m$
- Irreversible inhibitors permanently inactivate a fraction of enzyme molecules, reducing effective $V_{max}$

Enzyme activity is regulated in real time by allosteric effectors (non-covalent, fast, reversible) and covalent modification, primarily phosphorylation (enzymatic, reversible on a longer timescale, amplifiable). Feedback inhibition at the first committed step is the general strategy for maintaining metabolic homeostasis.

The organophosphate case integrates the entire chapter: a mechanism-based irreversible inhibitor attacks the active site serine of a near-perfect enzyme (AChE), causing accumulation of the neurotransmitter substrate, producing clinical toxicity through receptor overstimulation, and requiring antidotes that work at two distinct molecular targets, one at the receptor (atropine) and one at the enzyme (2-PAM), with a time constraint set by the irreversible chemical transformation called aging.

---

## Problem Set

**Problem 1.**
An enzyme has a $K_m$ of 0.5 mM and a $V_{max}$ of 80 nmol/min under standard conditions.

(a) What is $V_0$ when $[\text{S}] = 0.5$ mM? When $[\text{S}] = 5$ mM? When $[\text{S}] = 0.05$ mM?

(b) The physiological concentration of this enzyme's substrate in the cell is approximately 0.4–0.6 mM. Why is it metabolically advantageous for an enzyme to have a $K_m$ close to the physiological substrate concentration? What would happen to the cell's ability to regulate flux through this pathway if $K_m$ were 0.001 mM or 50 mM instead?

(c) The enzyme is a regulatory enzyme in a biosynthetic pathway. A downstream product accumulates to high concentration and decreases $V_0$ by 50% without changing $K_m$. What type of inhibition (competitive, uncompetitive, or noncompetitive) is most consistent with this pattern? On a Lineweaver-Burk plot, what change would you observe?

---

**Problem 2.** *(Synthesis)*
Carbonic anhydrase catalyzes $\text{CO}_2 + \text{H}_2\text{O} \rightleftharpoons \text{H}_2\text{CO}_3 \rightarrow \text{H}^+ + \text{HCO}_3^-$ with a $k_{cat}$ of approximately $10^6 \text{ s}^{-1}$. The uncatalyzed reaction takes approximately 100 seconds. A red blood cell spends approximately 0.5 seconds in a pulmonary capillary.

(a) Calculate the approximate fold-rate enhancement achieved by carbonic anhydrase. Express your answer as a power of 10.

(b) Without carbonic anhydrase, could a red blood cell complete the $\text{CO}_2$ hydration reaction during its 0.5-second transit through the pulmonary capillary? What would the physiological consequence be?

(c) Carbonic anhydrase lowers the activation energy for this reaction. Does this change the equilibrium position of the $CO_2/HCO_3^-$ reaction? Explain using the relationship between $\Delta G^{\circ'}$ and $K_{eq}$ from Chapter 1. What is the enzyme changing and what is it not changing?

---

**Problem 3.**
You are studying an enzyme and obtain the following Lineweaver-Burk data:

| Condition | y-intercept | x-intercept |
|---|---|---|
| No inhibitor | 0.020 | $-0.25$ |
| + Drug X | 0.020 | $-0.10$ |
| + Drug Y | 0.040 | $-0.25$ |

(a) Determine $K_m$ and $V_{max}$ under the no-inhibitor condition.

(b) For Drug X, determine the new apparent $K_m$. What type of inhibition does Drug X produce? Justify your answer from the changes in intercepts.

(c) For Drug Y, determine the new apparent $V_{max}$. What type of inhibition does Drug Y produce? If a patient is on Drug Y at a therapeutic dose, would increasing the dose of substrate (e.g., providing more metabolite) rescue enzyme activity? Why or why not?

---

**Problem 4.** *(Synthesis)*
Aspirin irreversibly inhibits cyclooxygenase-1 (COX-1) in platelets by acetylating a serine residue in the active site. Platelets are anucleate (they lack a nucleus) and cannot synthesize new proteins.

(a) Aspirin is an irreversible inhibitor. What effect does irreversible inhibition have on $V_{max}$ and $K_m$? Explain mechanistically why $K_m$ is not changed even though the enzyme is permanently inactivated in some fraction of molecules.

(b) A single low-dose aspirin (81 mg) inhibits platelet COX-1 for approximately 7–10 days. Yet aspirin's half-life in circulation is only about 20 minutes before it is hydrolyzed to salicylate (which does not inhibit COX-1 irreversibly). Explain why the antiplatelet effect lasts far longer than the drug itself persists in the blood.

(c) Ibuprofen is a reversible competitive inhibitor of COX-1 and COX-2. A patient on daily low-dose aspirin for cardiovascular protection takes ibuprofen for a headache. Clinical studies show that ibuprofen taken before aspirin can block aspirin's antiplatelet effect. Using your understanding of competitive versus irreversible inhibition, explain the molecular basis of this interaction.

---

**Problem 5.** *(Synthesis)*
A biochemist is studying feedback inhibition of the pyrimidine biosynthesis pathway. The enzyme ATCase (aspartate transcarbamoylase) catalyzes the first committed step and is allosterically inhibited by CTP, the pathway's end product. When CTP binds the regulatory site, ATCase shifts from its R-state (high activity) toward its T-state (low activity). ATCase displays sigmoidal substrate kinetics (Hill coefficient ~2).

(a) Explain why feedback inhibition acts on the first committed step rather than on the last step of the pathway. What would be wasted if the last step were inhibited instead?

(b) ATCase's sigmoidal kinetics mean it behaves more like an on/off switch than a gradual responder. How does this switch-like behavior serve the cell better than hyperbolic kinetics would for a feedback-regulated enzyme?

(c) CTP is structurally unrelated to aspartate (the substrate of ATCase) and binds a site entirely separate from the active site. Yet it dramatically decreases catalytic activity. Name the general category of mechanism this exemplifies and explain how a conformational change at the allosteric site can influence chemistry at the active site, which may be 30–40 Å away.

---

**Problem 6.**
A farmer is brought to the emergency department with the following presentation: bradycardia, excessive salivation and lacrimation, miosis (pupillary constriction), muscle fasciculations in the arms and trunk, and labored breathing. His family reports he was applying pesticide spray earlier in the day. Blood acetylcholinesterase activity is measured at 8% of normal.

(a) What class of compound is responsible for these findings, and what is the molecular mechanism by which it reduces acetylcholinesterase activity to 8% of normal? Classify this type of inhibition and state what parameter of the Michaelis-Menten equation is affected.

(b) The clinical team administers atropine and pralidoxime (2-PAM). Explain the mechanism of each drug. Why does atropine address the salivation and bradycardia but not the muscle fasciculations, while pralidoxime addresses both (if given in time)?

(c) The toxicologist says 2-PAM must be given immediately. If the farmer was exposed 4 hours ago and the specific organophosphate involved has an aging half-life of 1 hour, what fraction of the phosphoryl-AChE complex is still reactivatable? Should 2-PAM be expected to have significant clinical benefit at this point? Assume first-order aging kinetics: $f = (1/2)^{t/t_{1/2}}$.

---

**Problem 7.** *(Synthesis)*
Transition state analogs are among the most potent enzyme inhibitors known. The enzyme adenosine deaminase (ADA) catalyzes the deamination of adenosine to inosine. The transition state of this reaction involves a distorted purine ring with partial positive charge at the C1' position. A researcher synthesizes a molecule that mimics this distorted geometry and partial charge distribution, and finds that it binds ADA with a $K_d$ of $3 \times 10^{-12}$ M (3 pM), compared to adenosine's $K_m$ of approximately $3 \times 10^{-5}$ M (30 µM).

(a) Calculate the fold-difference in affinity between the transition state analog and the substrate. Express your answer as a power of 10.

(b) This enormous affinity difference is not random; it follows directly from the theory of transition state stabilization. Explain why the active site should bind the transition state analog more tightly than the substrate, using the logic of what the active site is physically shaped and charged to complement.

(c) A drug based on this compound would likely exhibit what type of inhibition kinetics (competitive, uncompetitive, or noncompetitive) — and would it be reversible or effectively irreversible at physiological concentrations? Justify your answer using the relationship between $K_d$, $K_i$, and the concentrations of competing substrate that could realistically be achieved in a patient.

---

## References

1. Berg JM, Tymoczko JL, Gatto GJ, Stryer L. *Biochemistry*, 9th ed. W.H. Freeman; 2019.
2. Nelson DL, Cox MM. *Lehninger Principles of Biochemistry*, 8th ed. W.H. Freeman; 2021.
3. Michaelis L, Menten ML. Die Kinetik der Invertinwirkung. *Biochem Z*. 1913;49:333–369. [English translation: Biochemistry. 2011;50(39):8264–8269. doi:10.1021/bi201284u]
4. Briggs GE, Haldane JBS. A note on the kinetics of enzyme action. *Biochem J*. 1925;19(2):338–339. doi:10.1042/bj0190338
5. Lineweaver H, Burk D. The determination of enzyme dissociation constants. *J Am Chem Soc*. 1934;56(3):658–666. doi:10.1021/ja01318a036
6. Koshland DE Jr. Application of a theory of enzyme specificity to protein synthesis. *Proc Natl Acad Sci USA*. 1958;44(2):98–104. doi:10.1073/pnas.44.2.98
7. Wolfenden R, Snider MJ. The depth of chemical time and the power of enzymes as catalysts. *Acc Chem Res*. 2001;34(12):938–945. doi:10.1021/ar000058i
8. Knowles JR, Albery WJ. Perfection in enzyme catalysis: the energetics of triosephosphate isomerase. *Acc Chem Res*. 1977;10(4):105–111. doi:10.1021/ar50112a001
9. Bourne HR, Sanders DA, McCormick F. The GTPase superfamily: a conserved switch for diverse cell functions. *Nature*. 1990;348(6297):125–132. doi:10.1038/348125a0
10. Rang HP, Ritter JM, Flower RJ, Henderson G. *Rang and Dale's Pharmacology*, 8th ed. Churchill Livingstone; 2015. [Chapters on cholinergic pharmacology and organophosphate toxicology.]
11. Jokanović M. Neurotoxic effects of organophosphorus pesticides and possible association with neurodegenerative diseases in man: a review. *Toxicology*. 2018;410:125–131. doi:10.1016/j.tox.2018.09.009
12. Colovic MB, Krstić DZ, Lazarević-Pašti TD, Bondžić AM, Vasić VM. Acetylcholinesterase inhibitors: pharmacology and toxicology. *Curr Neuropharmacol*. 2013;11(3):315–335. doi:10.2174/1570159X11311030005
13. Fersht A. *Structure and Mechanism in Protein Science: A Guide to Enzyme Catalysis and Protein Folding*. W.H. Freeman; 1999. [Definitive mechanistic treatment of transition-state stabilization and catalytic strategies.]
14. Cornish-Bowden A. One hundred years of Michaelis–Menten kinetics. *Perspect Sci*. 2015;4:3–9. doi:10.1016/j.pisc.2014.12.002
