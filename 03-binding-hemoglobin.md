# Chapter 3: Molecular Binding and Hemoglobin

---

## Opener Questions

Think about these before you read. Come back to them at the end and see if your answer changed.

1. Oxygen is not very soluble in water. At body temperature and the partial pressure of oxygen in the lungs, roughly 3 mL of $O_2$ dissolves per liter of plasma. The body requires about 250 mL of $O_2$ per minute at rest and several times that during exercise. A single protein bridges this enormous gap. What property of a binding protein would allow it to carry far more oxygen than simple dissolution? And what would limit how much more it could carry?

2. Carbon monoxide binds hemoglobin approximately 240 times more tightly than oxygen does. A patient with carbon monoxide poisoning reads 98% on a standard pulse oximeter, yet is dying from oxygen deprivation. How is this possible? What does "oxygen saturation" actually measure in this context, and why does standard monitoring fail?

---

## The Big Picture

Chapters 1 and 2 established two things. First, thermodynamics governs what is possible: reactions proceed when $\Delta G < 0$, proteins fold because the native state is the free-energy minimum, and nothing in a cell violates the second law. Second, structure determines function: a protein's amino acid sequence determines its three-dimensional shape, and its shape determines what it can do.

This chapter is about the next step: **how shape becomes action**. Proteins do not function in isolation. They bind things. An enzyme binds a substrate. A receptor binds a hormone. A transporter binds an ion. A structural protein binds other structural proteins. The function of any protein is, at its core, a description of what it binds, how tightly, and under what conditions. Often, proteins can help to chemically transform the things they bind (**substrtates** in this case) by acting as biological catalysts. This specific class of enzyme is called and **enzyme**

Molecular binding is not a vague concept about proteins "recognizing" each other. It is quantitative, thermodynamic, and predictable. There is a number, the **dissociation constant** ($K_d$), that precisely describes how tightly a protein holds its ligand. There are curves that describe how binding changes with ligand concentration. And there is a phenomenon, **allostery**, in which binding at one site changes binding strength or affinity at a distant site, allowing proteins to integrate information from multiple sources.

All of this will be illustrated by one protein: hemoglobin. Hemoglobin is not just an example of binding; it is the best single example of molecular biology in all of biochemistry. It shows simple binding, cooperative binding, allostery, metabolic regulation, and structural pathology, all in one molecule that most students already know by name. The goal of this chapter is to understand hemoglobin so thoroughly that you could explain, in molecular terms, why a patient with CO poisoning reads 98% on a pulse oximeter while their cells are suffocating. By the end, you will be able to torture your friends and family with in an excruciating amount of detail on how a protein binds what it does.

The through-line for this chapter is carbon monoxide poisoning. Not because it is the most common presentation you will see, but because it reveals every important feature of binding in one clinical picture: the competition between ligands for a binding site, the role of affinity, the consequences of allostery, and why quantitative reasoning about binding is not an academic exercise. It is the difference between correct treatment and a patient who dies with a reassuring monitor readout.

---

## The Chemistry of Binding

### The Equilibrium View

Binding between a protein and its ligand is a **reversible**, non-covalent interaction. *Note: there are times when something will be covalently attached to a protein but this is not what is meant canonically by "binding".*

The general reaction is:

$$\text{P} + \text{L} \underset{k_{\text{off}}}{\overset{k_{\text{on}}}{\rightleftharpoons}} \text{PL}$$

where P is the free protein, L is the free ligand, and PL is the protein-ligand complex. Like any reversible reaction, this reaches a dynamic equilibrium. The equilibrium is characterized by two rate constants: $k_{on}$, the rate at which P and L associate, and $k_{off}$, the rate at which PL dissociates.

At equilibrium, the rates of association and dissociation are equal and the Equlibrium constant is referred to as $K_a$:

$$K_a = \frac{[PL]}{[P][L]} = \frac{k_{on}}{k_{off}}$$
$$k_{on}[\text{P}][\text{L}] = k_{off}[\text{PL}]$$

*Note: Recall that the rate of any reaction (e.g $A \rightarrow B$) is given by $V_o=k[A]$

Conversely, flipping the binding equation and thus taking the inverse of everything we've done so far what we have is the process, NOT of association but of dissociation with a new equilibrium value $K_d$, the dissociation constant

Rearranging gives the **dissociation constant** $K_d$:

$$K_d = \frac{1}{K_a} = \frac{[\text{P}][\text{L}]}{[\text{PL}]} = \frac{k_{off}}{k_{on}}$$

Notice that the units of $K_d$ are molar ($M$), much more intuitive than the $M^{-1}$ given by $K_a$. A small $K_d$ means tight binding: even at low ligand concentration, most of the protein is occupied. A large $K_d$ means weak binding: you need a high ligand concentration to substantially occupy the protein.

To get an intuition for $K_d$: if $K_d = 10^{-9}$ M (1 nM), then at a ligand concentration of 1 nM, half the protein is bound. If you have a femtomolar $K_d$ ($10^{-15}$ M), the interaction is so tight it is essentially irreversible on biological timescales. Biotin-streptavidin, at $K_d \approx 4 \times 10^{-14}$ M, is the tightest non-covalent interaction known in biology. Hemoglobin's $K_d$ for oxygen is on the order of micromolar, which, as we will see, is precisely tuned for physiological oxygen delivery. We will explore the math in more detail below.

### On-Rates, Off-Rates, and What They Mean

It is worth being explicit about $k_{on}$ and $k_{off}$ separately, because each tells you something different.

$k_{on}$ is limited by diffusion: two molecules have to encounter each other before they can bind. The diffusion-limited $k_{on}$ for most protein-ligand interactions is around $10^8$ to $10^9$ M$^{-1}$s$^{-1}$. Many interactions are somewhat slower than this because binding requires a specific geometric encounter (the ligand has to hit the binding site in the right orientation), but $k_{on}$ cannot exceed the diffusion limit regardless of how complementary the surfaces are. If you want a tighter interaction, you cannot make $k_{on}$ faster; you have to make $k_{off}$ slower. This means tight binding always means a slow off-rate. The price of high affinity is slow release.

For oxygen delivery, slow release would be catastrophic. Hemoglobin needs to bind oxygen at the lungs and release it at the tissues, and it needs to complete this cycle billions of times over the 120-day lifespan of a red blood cell. The off-rate for oxygen from hemoglobin is tuned to be fast enough to release oxygen at physiological tissue partial pressures. The precise value of $K_d$, not just "tight" or "loose," is what allows the system to work.

### Fractional Saturation and the Binding Curve

Rather than asking "is the protein bound or not," a more useful question is: at a given ligand concentration $[\text{L}]$, what fraction of protein molecules are occupied?

Define the fractional saturation $\theta$ as the fraction of binding sites occupied:

$$\theta = \frac{\text{Sites Occupied}}{\text{Total number of sites}} = \frac{[\text{PL}]}{[\text{P}] + [\text{PL}]}$$

While this is objectively true, it's not very useful, how do we measure $[\text{PL}]$ and if we could well our job would be done. Let us do some work now to make our lives easier in the lab. Take the $K_a$ definition above and solve instead for $[\text{PL}]$ which gives us the following:

$$[\text{PL}] = K_a[\text{P}][\text{L}]$$

Substituting this definition of $[\text{PL}]$ into the equation for $\theta$ above gives

$$\theta = \frac{K_a[\text{P}][\text{L}]}{[\text{P}] + K_a[\text{P}][\text{L}]}$$

Factoring out $K_a[\text{P}]$ produces the following

$$\theta = \frac{\cancel{K_a[\text{P}]}[\text{L}]}{\cancel{K_a[\text{P}]}(\frac{1}{K_a} + [\text{L}])}$$

Which finally yields:

$$\theta = \frac{[\text{L}]}{[\text{L}] + K_d}$$
*Note: recall that $K_d = \frac{1}{K_a}$

This is a hyperbola. When $[\text{L}] = K_d$, $\theta = 0.5$: half the sites are occupied. This is the physical meaning of $K_d$ on the binding curve. When $[\text{L}] \ll K_d$, most sites are empty ($\theta \approx [\text{L}]/K_d$). When $[\text{L}] \gg K_d$, most sites are occupied ($\theta \approx 1$).

The hyperbolic binding curve has a specific shape that carries information. It is steep at low $[\text{L}]$ and flat at high $[\text{L}]$. This means a hyperbolic protein is most sensitive to ligand concentration changes around the $K_d$. Below and above the $K_d$, changing the concentration has progressively less effect on saturation.

For oxygen delivery, the relevant question is: how much does saturation change between lung partial pressures (where the protein should load) and tissue partial pressures (where the protein should unload)? The answer depends entirely on the shape of the binding curve and where the $K_d$ sits relative to those physiological pressures.

---

## Oxygen as a Binding Problem

### Why the Body Needs a Carrier

Oxygen is nonpolar and has limited solubility in water. At 37°C and the partial pressure of $O_2$ in the lungs (about 100 mmHg or torr), only about 3 mL of $O_2$ dissolves per liter of plasma, which is mostly water. The resting body consumes roughly 250 mL $O_2$ per minute. If oxygen had to travel purely in solution, cardiac output would need to be over 80 liters per minute, roughly 16 times the actual resting value of 5 L/min. This is physiologically impossible. Interestingly this is the main limit on the size of an organism, the larger the organism the more oxygen is needed so there exists a natural ceiling on how practically large something can be. This is why we see so many examples of significantly larger animals and insects during the Jurrasic, Cretaceous and Cambrian eras, there was more atmosphteric oxygen available than today.

Hemoglobin solves the problem by concentrating oxygen in red blood cells. Each hemoglobin molecule can bind four oxygen molecules. Red blood cells contain approximately 280 million hemoglobin molecules. The oxygen-carrying capacity of blood with hemoglobin is about 200 mL $O_2$ per liter, roughly 65 times the dissolved capacity. Hemoglobin does not change the physics of $O_2$ solubility; it changes the effective capacity by providing a specific, high-affinity binding site that concentrates oxygen chemically (on Hb) rather than physically (dissolved in aqueous plasma).

### The Physiological Requirement

For hemoglobin to function as an oxygen transporter, it must satisfy two competing demands that a simple, fixed-affinity protein cannot simultaneously meet:

1. **Load efficiently in the lungs.** At the partial pressure of $O_2$ in the pulmonary alveoli (roughly 100 torr), hemoglobin should be nearly fully saturated.
2. **Unload efficiently in the tissues.** At the partial pressure of $O_2$ in peripheral tissues (roughly 20 to 40 mmHg), hemoglobin should release a substantial fraction of its oxygen.

A protein with a hyperbolic binding curve and a $K_d$ tuned to one of these pressures will necessarily fail at the other. If the $K_d$ is set to achieve high saturation at 100 mmHg, the curve is so flat in the tissue range that very little oxygen is released. If the $K_d$ is shifted to improve unloading at 20 to 40 mmHg, the protein is never fully loaded at 100 mmHg.

The solution, which evolution arrived at in hemoglobin, is cooperativity: a binding curve that is not hyperbolic but sigmoidal (S-shaped), with a steep rise in the physiological range. Myoglobin, the simpler oxygen-binding protein in muscle, will serve as the baseline case: it shows what a protein can do without cooperativity, and why that is insufficient for systemic oxygen delivery.

---

## Myoglobin: The Simple Case

### Structure and the Heme Group

Myoglobin is a monomeric protein of 153 amino acids. It is a single polypeptide chain folded into a compact globular structure made almost entirely of alpha helices. This all-helical architecture is called the **globin fold**, and it is found, with variation, in hemoglobin's subunits as well.

Buried inside myoglobin, tucked into a hydrophobic pocket formed by two helices, is the **heme group**. Heme is a porphyrin ring: four pyrrole rings connected by methine bridges in a flat, cyclic arrangement, with a central iron atom. In myoglobin and hemoglobin, the iron is in the ferrous state ($Fe^{2+}$). The iron has six coordination bonds: four are occupied by the nitrogen atoms of the porphyrin rings, one is occupied by a histidine residue from the protein (the **proximal histidine**), and the sixth is the binding site for oxygen.

Something remarkable occurs when $O_2$ binds to the sixth coordinate-covalent site of the heme iron atom. Because of oxygen's electronegativity, upon binding the $Fe^{2+}$ is effectively oxidized (partially at least) to $Fe^{3+}$. This shrinks the ionic radius of the iron atom, allowing it to more comfortably fit inside the plane of the heme. This movement of less than one Angstrom pulls on the proximal His occupying the 5th coordinate covalent site, moving the helix to which that His belongs. For myoglobin, this is rather pointless, but when we return to examining the cooperativity of hemoglobin binding oxygen, this small movement will be crucial.

On the other side of the heme, a second histidine residue (the **distal histidine**) does not coordinate the iron directly but sits close enough to interact with oxygen once it binds. The distal histidine forms a hydrogen bond with bound $O_2$, stabilizing it in the binding pocket. This hydrogen bond serves two protective functions. First, it discriminates against carbon monoxide: CO binds free iron with roughly 25,000 times the affinity of $O_2$, but in the protein, the distal histidine interferes sterically with CO's preferred linear orientation, reducing CO's relative affinity at the heme to *"only"* about 200 to 250 times that of $O_2$. Even with this geometric trick, CO still out-competes oxygen significantly, which is why CO poisoning is so dangerous. Second, the hydrogen bond helps prevent the spontaneous release of superoxide. As noted above, bound $O_2$ has partial $Fe^{3+} - O_2^{\bullet -}(\text{superoxide})$ character. If the superoxide were to dissociate and leave, the iron would be left as $Fe^{3+}$: methemoglobin, incapable of binding oxygen. The distal histidine stabilizes the iron-oxygen complex and suppresses this reaction, keeping the iron in a form that can release $O_2$ rather than $O_2^{\bullet -}$.

The iron must remain ferrous ($Fe^{2+}$) to bind oxygen. If iron is oxidized to ferric ($Fe^{3+}$), it cannot bind $O_2$. This oxidized form is **methemoglobin** (metHb). Red blood cells contain an enzyme, methemoglobin reductase, that continuously reduces any metHb back to functional hemoglobin. Certain drugs and toxins can overwhelm this system, leading to methemoglobinemia: hemoglobin is present, but cannot carry oxygen.

### The Myoglobin Binding Curve

Myoglobin has one heme group and one oxygen binding site. Its behavior follows the simple hyperbolic equation derived above:

$$\theta = \frac{pO_2}{P_{50} + pO_2}$$

where $P_{50}$ is the partial pressure at which half the myoglobin is saturated (the oxygen analog of $K_d$). For myoglobin, $P_{50} \approx 2$ to 3 mmHg.

This is an extremely low $P_{50}$: myoglobin has very high affinity for oxygen. At the partial pressure in lung capillaries (100 mmHg), myoglobin is essentially fully saturated (>97%). At the partial pressure in resting muscle (20 to 40 mmHg), myoglobin is still over 85% saturated. At the partial pressure in exercising muscle (which can fall below 5 mmHg), myoglobin begins to release its oxygen.

This tells you what myoglobin is for: it is an oxygen reservoir in muscle, not a systemic transporter. It loads oxygen from the blood in muscle capillaries and releases it to mitochondria when local $O_2$ tension falls very low during intense activity and so $pO_2$ drops below 8-9 mmHg. It is not designed to load at one location and unload at another on a systemic scale; it sits in place and buffers local oxygen supply. Myoglobin's high affinity and hyperbolic curve are exactly right for this role.

### Why Myoglobin Cannot Deliver Oxygen Systemically

If we imagine replacing hemoglobin with myoglobin as the blood oxygen carrier, the failure is clear from the binding curve.

At lung pO$_2$ (100 mmHg): myoglobin is ~97% saturated. Good: it loads.

At resting tissue pO$_2$ (30 mmHg): myoglobin is still ~91% saturated. Terrible: it does not unload.

The total oxygen delivered would be $97\% - 91\% = 6\%$ of carrying capacity per pass through the circulation. This is physiologically inadequate (worse than simple dissolution in plasma). A systemic oxygen transporter needs to unload a large fraction of its cargo in the tissue range. Myoglobin's curve is too flat there.

What is needed is a protein that is hypersensitive to $pO_2$ changes in the range between 20 and 100 mmHg: loading steeply in the lungs and unloading steeply in the tissues. This requires a binding curve with a different shape than a hyperbola. It requires cooperativity.

---

## Hemoglobin: Cooperativity Changes the Shape of the Curve

### The Sigmoidal Curve

Hemoglobin's oxygen binding curve is sigmoidal (S-shaped) rather than hyperbolic. It has a steep rise in the physiological range and a plateaus at high and low $pO_2$ values.

Compare the two proteins at physiological pressures:

| Location | $pO_2$ (mmHg) | Myoglobin ($\theta$) | Hemoglobin ($\theta$) |
|---|---|---|---|
| Lungs | 100 | ~97% | ~98% |
| Resting tissue | 30 | ~91% | ~65% |
| Exercising tissue | 10 | ~77% | ~27% |

The difference in unloading is dramatic. Hemoglobin delivers roughly 30 to 70% of its oxygen cargo per pass through resting or exercising tissues. Myoglobin would deliver less than 10% under the same conditions. The sigmoidal shape is not cosmetic; it is what makes systemic oxygen delivery work.

### The Hill Equation

How did we arrive at the numbers above? Consider a variation of the hypothetical protein/ligand system we examined in the previous section.

$$\text{P} + n\text{L} \underset{k_{\text{off}}}{\overset{k_{\text{on}}}{\rightleftharpoons}} \text{PL}_n$$

For Hemoglobin $n=4$ since each subunit of the $\alpha_2\beta_2$ hetertetramer contains an oxygen-binding Heme prosthetic group.

This of course presumes the reaction is all-or-nothing: nothing happens until all $n$ ligands bind simultaneously. Real hemoglobin can be bound to anywhere between 0 and 4 oxygens, so $n$ will never truly equal 4 in practice. If we proceed with this oversimplification anyway, the $\theta$ derivation from the previous section carries through with $[\text{L}]^n$ replacing $[\text{L}]$ (the full derivation is left as an exercise):

$$\theta = \frac{pO_2^n}{K_d + pO_2^n}$$

Now, $P_{50}$ is defined as the $pO_2$ at which $\theta = 0.5$. Substituting:

$$0.5 = \frac{P_{50}^n}{K_d + P_{50}^n} \implies K_d = P_{50}^n$$

So $K_d$ in the cooperative case equals $P_{50}^n$, not $P_{50}$. Substituting this back gives the **Hill equation**:

$$\theta = \frac{pO_2^n}{pO_2^n + P_{50}^n}$$

The $P_{50}^n$ in the denominator is not a separate assumption; it is what the equilibrium constant becomes when expressed in terms of the half-saturation point for a reaction involving $n$ ligands simultaneously. Both terms are raised to the same power $n$ as a direct consequence of the algebra.

When $n = 1$, this reduces to the hyperbolic equation. When $n > 1$, the curve is sigmoidal: it rises more steeply and the transition between low and high saturation is more abrupt. The Hill coefficient $n$ measures the **degree of cooperativity**.

For hemoglobin, the measured Hill coefficient is approximately 2.8 to 3.0. The theoretical maximum for a four-site protein with perfect cooperativity would be $n = 4$. For myoglobin (no cooperativity), $n = 1$. The value of 2.8 means hemoglobin's cooperativity is substantial but not perfect: the four sites behave as though roughly three of them are strongly coupled.

What $n > 1$ means physically is that binding of one oxygen molecule increases the $O_2$ affinity of the remaining sites. The protein is not a set of four independent, identical binding sites. They communicate.

---

## The Structural Basis of Cooperativity: T-State and R-State

### Two Conformations

Hemoglobin is a heterotetramer: two alpha chains and two beta chains, assembled as an $\alpha_2\beta_2$ complex. Each subunit has a globin fold, a heme group, and a single oxygen binding site. The four subunits are held together by a combination of hydrophobic interactions, hydrogen bonds, and ionic interactions at their interfaces.

Hemoglobin exists in two principal conformations, and the equilibrium between them is the molecular basis of cooperativity.

The **T-state** (tense state) is the low-affinity conformation. It is the conformation of deoxyhemoglobin. In the T-state, the four subunits are held together by a network of salt bridges (ionic interactions) at the interfaces between subunits, particularly between the alpha and beta chains at the $\alpha_1\beta_2$ and $\alpha_2\beta_1$ interfaces (think of HbA as a "dimer of dimers" i.e. a dimer of $\alpha\beta$ heterodimers). These salt bridges involve the C-terminal residues of both chains and several specific side chains including His146 of the beta chains (important for the Bohr effect, discussed below). The T-state is compact and constrained. The heme iron is slightly out of the plane of the porphyrin ring, closer toward the **proximal histidine**, in a geometry that reduces its affinity for oxygen. Each oxygen binding site in the T-state has a $P_{50}$ of roughly 30 to 40 mmHg. Importantly, in the T-state, the $\alpha\beta$ dimers are arranged such that there is a pore or pocket in the center (where all four subunits meet) that is lined with positively charged residues. This pocket does not exist in the R-state as we'll see.

The **R-state** (relaxed state) is the high-affinity conformation and its loading curve resembles that of myoglobin. In the R-state, the subunit-subunit salt bridges are broken. The $\alpha\beta$ dimers rotate ~$15^{\circ}$ relative to each other. This rotation collapses the central pore that was present in the T-state. With the geometric constraints of the T-state relieved, the heme iron sits more readily in the plane of the porphyrin ring: this in-plane geometry is what makes oxygen binding favorable, as established above. Each oxygen binding site in the R-state has a $P_{50}$ of roughly 0.3 mmHg: 100-fold more avid than in the T-state.

In the absence of oxygen (as in venous blood returning from tissues), the equilibrium strongly favors the T-state. In the presence of high oxygen (as in the lungs), the equilibrium shifts strongly toward the R-state.

### How Cooperativity Works

Here is the key point: when one oxygen molecule binds to a T-state hemoglobin subunit, it pulls the iron into the porphyrin plane. This movement is transmitted through covalent bonds to the proximal histidine, which shifts the position of the helix to which it belongs (the F-helix, see I promised it would be important later). The F-helix movement alters contacts at the subunit interface which is how the separate subunits "communicate" with one another. The strain propagates through the $\alpha_2\beta_2$ tetramer, making it thermodynamically easier for the entire complex to shift toward the R-state. The next oxygen to bind encounters a protein that is already partway toward the R-state: a higher-affinity conformation. The third oxygen shifts the tetramer further, and the fourth oxygen encounters a protein that is essentially already in the R-state.

This is the structural mechanism of cooperativity: binding propagates a conformational change from one subunit to the others through the subunit interfaces. A monomeric protein cannot be cooperative, because there are no subunit interfaces to transmit conformational information. Quaternary structure is a prerequisite.

The **MWC model** (Monod-Wyman-Changeux, or **concerted model**) treats the T-to-R transition as concerted: all four subunits shift simultaneously. In the MWC model, hemoglobin is always all-T or all-R, and oxygen binding simply shifts the equilibrium between these two states. This is a simplification, but it captures the essential features of hemoglobin cooperativity and is the model used most commonly in teaching.

The **KNF model** (Koshland-Nemethy-Filmer, or sequential model) treats the conformational change as occurring one subunit at a time: each oxygen binding event converts one subunit from T-like to R-like geometry. The sequential model accounts better for certain detailed observations about hemoglobin, but both models are approximations of the reality. The important take-home message is not which model is correct, but the physical principle both share: **binding at one site changes the properties of other sites through conformational change propagated across the subunit interfaces**.

---

## Allostery: Binding Sites That Listen to Each Other

Cooperativity is one form of a broader phenomenon: **allostery**. An allosteric protein has at least two binding sites whose properties are coupled. A change at one site, whether binding of a ligand or a conformational perturbation, alters the affinity, activity, or specificity of a distant site.

Hemoglobin is the canonical allosteric protein. Its four oxygen binding sites are allosterically coupled to each other (cooperativity). But oxygen is not the only molecule that regulates hemoglobin. Several other molecules bind hemoglobin at sites distinct from the oxygen-binding hemes and profoundly alter oxygen affinity. These are **allosteric effectors**: molecules that modulate protein function by binding away from the active site.

Understanding allosteric regulation of hemoglobin requires understanding one central principle: any molecule that preferentially stabilizes the T-state will decrease oxygen affinity (shift the curve right, to higher $P_{50}$, meaning more oxygen is released at any given $pO_2$). Any molecule that preferentially stabilizes the R-state will increase oxygen affinity (shift the curve left, to lower $P_{50}$, meaning less oxygen is released). These would be referred to in this case as either **negative** or **positive** allosteric effectors (decreasing or increasing affinity respectively). 

The two major allosteric effectors of hemoglobin are protons ($H^+$) and 2,3-bisphosphoglycerate (2,3-BPG). Carbon monoxide, in addition to competing directly for the oxygen binding site, also acts as an allosteric effector of the remaining sites. Each is a different kind of lesson in how protein function is regulated beyond the level of simple binding.

---

## The Bohr Effect: pH and $CO_2$ as Allosteric Effectors

### The Phenomenon

In 1904, Christian Bohr (father of physicist Niels Bohr incidentally) observed that hemoglobin's affinity for oxygen decreases as pH decreases. This is the **Bohr effect**: at lower pH, the oxygen-hemoglobin dissociation curve shifts to the right. The same shift occurs with increasing CO$_2$ concentration.

The physiological context makes the Bohr effect immediately recognizable as adaptive. Active tissues are metabolically demanding: they consume oxygen, produce $CO_2$, and generate lactic acid and other proton sources. The pH in capillary blood perfusing active muscle is lower, and $pCO_2$ is higher, than in the lungs. The Bohr effect means that hemoglobin automatically releases more oxygen precisely where it is most needed: in high-metabolism, high-CO$_2$, low-pH environments.

### The Molecular Mechanism

The Bohr effect is mediated by **Bohr protons**: specific ionizable residues in hemoglobin whose pKa values are different in the T-state and R-state. The most important Bohr proton in human hemoglobin is His146 of the $\beta$ chains (the C-terminal histidine of the beta chain).

Recall from Chapter 1 that the protonation state of a histidine residue depends on pH relative to its *apparent* $pK_a$, and from Chapter 2 that the apparent $pK_a$ of a side chain can be shifted substantially by the local electrostatic environment. In the T-state of deoxyhemoglobin, His146 forms a salt bridge with Asp94 of the same $\beta$ chain. This salt bridge stabilizes the protonated (positively charged) form of His146, shifting its apparent pKa upward from the free solution value of about 6.0 toward 7.0 to 7.5. His146 is therefore partly protonated at physiological pH in the T-state.

In the R-state of oxyhemoglobin, the salt bridge between His146 and Asp94 is broken. Without the stabilizing salt bridge, His146's apparent pKa returns to near 6.0, and it releases its proton at physiological pH since the pH is now higher than its $pK_a$. The net result: going from T-state to R-state (i.e., binding oxygen) releases protons. Conversely, increasing $H^+$ concentration (lowering pH) pushes His146 and other Bohr protons toward the protonated form, which stabilizes the *T-state*, which decreases oxygen affinity, shifting the loading curve to the right. The thermodynamic linkage is exact and quantitative: if proton binding favors the T-state, then T-to-R transitions must release protons, and the equilibrium is coupled in both directions.

$CO_2$ contributes to the Bohr effect through an additional mechanism. $CO_2$ reacts directly with the uncharged alpha-amino groups at the N-termini of hemoglobin chains (both alpha and beta) to form **carbamino compounds**:

$$-\text{NH}_2 + \text{CO}_2 \rightleftharpoons -\text{NH-COO}^- + \text{H}^+$$

You might expect these N-terminal amino groups to be fully protonated ($-\text{NH}_3^+$) at physiological pH, since free alpha-amino groups typically have a pKa of 8 to 9. In hemoglobin, however, the local electrostatic environment depresses the apparent pKa of the N-terminal amino groups to around 7.0 to 7.8, so a meaningful fraction exist in the uncharged $-\text{NH}_2$ form at pH 7.4. This is the same pKa-shifting logic from Chapter 2 applied here: the protein environment, not the textbook value, determines the actual protonation state. The uncharged form matters because only $-\text{NH}_2$ can act as a nucleophile and react with $CO_2$; the protonated $-\text{NH}_3^+$ form cannot, since its nitrogen lone pair is tied up in the bond to the extra proton.

This reaction introduces a negatively charged carbamate on the N-terminal residue, which forms additional salt bridges that stabilize the T-state. High $pCO_2$ (actively exercising tissues) therefore shifts hemoglobin toward the T-state, shifting the loading curve even further right, reinforcing the Bohr effect from the pH mechanism.

There is also a second route by which $CO_2$ itself acts, this time indirectly. $CO_2$ dissolved in plasma and red blood cells is hydrated by carbonic anhydrase to form carbonic acid, which immediately dissociates:

$$CO_2 + H_2O \underset{\text{carbonic anhydrase}}{\rightleftharpoons} H_2CO_3 \rightleftharpoons HCO_3^- + H^+$$

The protons released lower local pH, which engages the Bohr proton mechanism described in the previous section. Note also that the carbamino reaction itself releases a proton (visible in the reaction equation above), adding further to the acidification. Taken together, high pCO$_2$ shifts hemoglobin toward the T-state through three converging mechanisms: (1) direct H$^+$ binding to Bohr residues such as His146, (2) carbamino formation on N-terminal amino groups, and (3) pH drop from CO$_2$ hydration to carbonic acid. All three push toward the T-state in active tissues, and all three reverse in the lungs where pCO$_2$ is low and CO$_2$ is exhaled.

The Bohr effect is one of the most elegant examples of molecular integration in biology. Hemoglobin acts as a sensor of metabolic activity (via CO$_2$ and pH), and automatically delivers more oxygen where metabolic demand is highest. No hormone, no signal transduction cascade, and no regulatory enzyme is required. The physics of proton binding and conformational equilibrium does the work.

---

## 2,3-Bisphosphoglycerate: Metabolic Adaptation

### The Molecule and Its Binding Site

2,3-Bisphosphoglycerate (2,3-BPG) is a highly charged molecule produced in red blood cells as a byproduct of glycolysis. It carries four negative charges at physiological pH.

2,3-BPG binds in the central cavity of deoxyhemoglobin. This cavity exists in the T-state of the tetramer, formed by residues from both beta chains. The binding site is lined with positively charged residues: His2, Lys82, and His143 from each beta chain contribute eight positive charges that embrace the four negatively charged phosphate groups of 2,3-BPG. The interaction is electrostatically driven.

Critically, when hemoglobin shifts to the R-state, the central cavity narrows and 2,3-BPG cannot fit; 2,3-BPG binds exclusively to the T-state. By extension this means that, if present, 2,3-BPG must be expelled from the pocket when the state switches from T to R, which requires energy in order to break the ionic interactions between it and the positively charged pocket. In other words, switching from T to R (binding oxygen) just got harder, shifting the Hb loading curve to the right. 2,3-BPG selectively stabilizes deoxyhemoglobin: it drives the T-to-R equilibrium toward the T-state and decreases oxygen affinity. The $P_{50}$ of hemoglobin in the presence of physiological 2,3-BPG concentrations is about 26 mmHg. Strip out the 2,3-BPG, and the $P_{50}$ drops to about 1 mmHg: hemoglobin would load in the lungs and essentially never release oxygen in the tissues, behaving just like myoglobin, which we have already established is unacceptable. 2,3-BPG is not a minor modulator; it is responsible for roughly half the functional oxygen-delivering capacity of blood.

### Altitude Adaptation

At altitude, the partial pressure of atmospheric oxygen is lower. Barometric pressure falls proportionally with altitude, and $pO_2$ falls with it. At 4,500 meters, $pO_2$ in the lungs is roughly 60 mmHg instead of 100 mmHg. Hemoglobin is less saturated when it leaves the lungs: instead of 98%, it might be 85% loaded.

Within hours of ascent to altitude, red blood cells increase their production of 2,3-BPG. The logic is straightforward: lower $pO_2$ means hemoglobin binds less oxygen and therefore spends more time in the T-state (the deoxy conformation), and the T-state sequesters 2,3-BPG in its central cavity. As more 2,3-BPG is bound to hemoglobin, the free concentration inside the red blood cell falls, which signals the cell to produce more. Elevated 2,3-BPG shifts the oxygen dissociation curve to the right: the $P_{50}$ increases. This improves unloading in the tissues, partially compensating for the reduced loading in the lungs.

This is a metabolic regulation of a binding equilibrium: the cell's energy metabolism (glycolysis which we'll examine in great detail later) produces a small molecule (2,3-BPG) that acts as an allosteric effector of a transport protein (hemoglobin), adjusting its properties in response to an environmental change (altitude). The adaptation is automatic, quantitative, and mediated entirely through the chemistry of binding.

### Temperature

Temperature shifts the oxygen dissociation curve to the right: higher temperature decreases hemoglobin's oxygen affinity and raises $P_{50}$. The mechanism is the same thermodynamic logic from Chapter 1. Non-covalent interactions, including the hydrogen bonds and salt bridges that stabilize both the T-state and the oxygen-heme coordination bond, are weakened at higher temperatures. The net effect is that hemoglobin holds oxygen less tightly when warm.

This is physiologically useful in exactly the same way as the Bohr effect. Exercising muscle is warmer than resting tissue. The local temperature rise in an active muscle shifts the dissociation curve right, promoting oxygen unloading precisely where demand is highest. Like the pH and $CO_2$ effects, temperature acts automatically: no signaling is required. The muscle generates its own heat, and that heat directly adjusts hemoglobin's behavior in the capillaries perfusing it.

The left-shift corollary matters in clinical contexts. In hypothermia, lower body temperature increases hemoglobin's oxygen affinity, shifting the curve left. Hemoglobin loads readily but releases oxygen poorly in the tissues. This contributes to the tissue hypoxia seen in severe hypothermia even when blood oxygen content appears adequate.

### Fetal Hemoglobin

Fetal hemoglobin (HbF) has a different subunit composition: two alpha chains and two gamma chains ($\alpha_2\gamma_2$), rather than the adult $\alpha_2\beta_2$ (HbA). The gamma chain differs from the beta chain at the 2,3-BPG binding site: a critical histidine residue (His143 in the beta chain) is replaced by serine in the gamma chain. Serine is uncharged at physiological pH, so the gamma chain makes fewer favorable contacts with the negatively charged 2,3-BPG. HbF binds 2,3-BPG more weakly than HbA.

The consequence is that HbF has a higher oxygen affinity than HbA at the same 2,3-BPG concentration: its $P_{50}$ is about 19 mmHg, versus 26 mmHg for adult hemoglobin. Since the interacction between 2,3-BPG and the T-State pocket is weaker it take less energy to transition from T to R, allowing HbF to bind Oxygen more readily. At any given $pO_2$, HbF holds more oxygen than HbA. In the placenta, where both fetal HbF and maternal HbA are in capillaries in close proximity at similar $pO_2$ values, oxygen spontaneously flows from the lower-affinity maternal hemoglobin (HbA) to the higher-affinity fetal hemoglobin (HbF), without any active transport. The gradient in affinity drives oxygen transfer. After birth, the gamma chains are gradually replaced by adult beta chains, and HbF is replaced by HbA over the first year of life.

---

## Carbon Monoxide Poisoning: The Full Picture

Now the clinical case from the opener can be fully analyzed.

### Competitive Binding and Affinity

$CO$ competes with $O_2$ for the same binding site on heme iron. The relative affinity of hemoglobin for $CO$ versus $O_2$ is described by the **Haldane constant** $M$:

$$M = \frac{[\text{Hb}_{CO}]}{[\text{Hb}_{O_2}]} \times \frac{pO_2}{pCO}$$

For human hemoglobin, $M \approx 200 \text{to} 250$. This means that at equal partial pressures, hemoglobin binds CO approximately 200 to 250 times more tightly than $O_2$. In ambient air, $pCO$ is essentially zero and the competition is irrelevant. In an environment with significant $pCO$ (a closed garage with a running engine, a house fire, a malfunctioning heater), $pCO$ can reach tens or hundreds of ppm, and at these concentrations, CO effectively displaces oxygen from hemoglobin.

The competitive aspect of CO poisoning is the part most people intuit: CO occupies hemoglobin binding sites, leaving fewer available for oxygen. But this is only half the story, and arguably not the more insidious half.

### The Allosteric Dimension: Why CO Is Worse Than Expected

If CO simply blocked four out of four heme groups, blood would carry zero oxygen, and the patient would be unconscious almost immediately. What actually happens in CO poisoning is more complex and more treacherous.

CO does not necessarily occupy all four binding sites simultaneously. In partial CO poisoning, a hemoglobin molecule might have one, two, or three sites occupied by CO and the remaining sites occupied by oxygen. Here is the allosteric problem: CO binds and locks hemoglobin in the R-state (high-affinity conformation). The T-to-R transition that CO causes at the occupied sites is transmitted through the subunit interfaces, just as oxygen binding is. The result is that the hemoglobin molecules with some CO bound have their remaining oxygen-binding sites locked in the high-affinity R-state.

High-affinity R-state hemoglobin loads oxygen readily in the lungs. It does not unload oxygen readily in the tissues. The sigmoidal curve is eliminated: the molecule is stuck at the left end of the binding curve, holding its oxygen even at tissue pO$_2$ values that would normally drive substantial release. This is the **Haldane effect**: CO not only displaces oxygen from some sites but also prevents the oxygen at the remaining sites from being released where it is needed.

The clinical consequence is that a patient with only 25 to 30% carboxyhemoglobin (75% of sites still available for oxygen) can be far more severely hypoxic than a patient who simply had 25% of their hemoglobin removed by anemia. The CO-poisoned patient has a hemoglobin that loads and does not deliver; the anemic patient has less hemoglobin, but what is present still functions cooperatively and unloads appropriately.

### Why the Pulse Oximeter is a Lying Liar

Standard pulse oximetry works by measuring light absorption at two wavelengths: 660 nm (red) and 940 nm (infrared). Oxyhemoglobin and deoxyhemoglobin absorb differently at these wavelengths, and the ratio of absorbances allows the device to calculate oxygen saturation. The oximeter clip you put on your finger shines LEDs emitting these two wavelengths through your finger which is read by a photodiode on the other end of the clip. Comparing the starting (known) value with the read value and applying a conversion produces the reading on the screen.

Carboxyhemoglobin (HbCO) absorbs 660 nm light in almost exactly the same way as oxyhemoglobin. The pulse oximeter cannot distinguish between $HbO_2$ and $HbCO$. A patient with 40% HbCO and 58% $HbO_2$ reads as 98% "saturated" on a standard pulse oximeter, because it sees 98% of the signal it would expect from fully oxygenated blood. The device is not malfunctioning; it is measuring what it is designed to measure, and $HbCO$ happens to look identical to $HbO_2$ at the wavelengths it uses.

Accurate diagnosis of CO poisoning requires co-oximetry: a device that measures absorbance at multiple wavelengths and can distinguish $HbO_2$, $HbCO$, methemoglobin, and deoxyhemoglobin separately. Emergency departments use co-oximetry on arterial blood gas samples, but it requires a blood draw and is not continuous like pulse oximetry.

Treatment follows from the binding chemistry. CO's affinity is high, but the binding is still reversible (as are all binding events): $K_d$ is low but not zero, and there IS an off-rate ($k_{off}$). Administration of 100% $O_2$ floods the system with competing ligand, using mass action to push CO off the heme. At 100% $O_2$ (versus the 21% you normally find room air), the effective $pO_2$ is about five times higher, shortening the half-life of HbCO from roughly 5 hours in room air to about 60 to 90 minutes. Hyperbaric oxygen (100% $O_2$ at 2 to 3 atmospheres) reduces the HbCO half-life to about 20 to 30 minutes and is used in severe poisoning because of the additional benefit of dissolving enough $O_2$ directly in plasma to supply the brain independent of hemoglobin.

---

## When It Breaks

### Methemoglobinemia

When heme iron is oxidized from $Fe^{2+}$ to $Fe^{3+}$, it cannot bind oxygen. This is methemoglobin (metHb). A small amount of metHb is always forming in red blood cells (perhaps 1 to 2% of total hemoglobin at any time), but methemoglobin reductase (which uses NADH as a reducing agent, more on NADH in a future chapter) continuously reduces it back to functional HbA ($Fe^{2+}$).

Certain oxidizing agents overwhelm this system. Nitrites (from contaminated well water, dapsone, benzocaine) and nitrates (from nitroglycerin, dietary sources) can oxidize enough iron to cause symptomatic methemoglobinemia. Dapsone, used for malaria prophylaxis and certain dermatological conditions, is a particularly important cause in clinical medicine.

Clinical findings mirror those of CO poisoning in some ways: cyanosis (because metHb, like deoxyhemoglobin, is dark-colored and absorbs different wavelengths), and hypoxia despite normal $pO_2$ on blood gas panels. But the mechanism is different: no oxygen is being displaced by a competing ligand; the heme iron is simply oxidized and cannot bind anything. Treatment is methylene blue, which provides an alternative electron pathway to reduce metHb back to active hemoglobin. As an aside, the use of this blue dye as a remedy for methoglobinemia is objectively hilarious given that a tell-tale sign of methemoglobinemia is blue colored skin.

Like CO poisoning, methemoglobinemia illustrates that hemoglobin function depends not only on the binding equilibrium but on the oxidation state of the iron at its core. Structure is not just about protein conformation; it extends to the coordination chemistry of the cofactor.

### Sickle Cell Disease Revisited: Binding Meets Allostery

Chapter 2 covered the structural basis of sickle cell disease: the E6V substitution creates a hydrophobic patch that drives polymerization of deoxyhemoglobin. This chapter adds the binding dimension.

Sickling is state-dependent. HbS polymerizes in the T-state (deoxyhemoglobin), not in the R-state (oxyhemoglobin). The hydrophobic region that accepts the Val6 patch is exposed in the T-state and buried in the R-state. This explains why sickling is triggered by hypoxia: deoxygenation shifts HbS toward the T-state, exposing the binding site for polymerization.

This is a direct connection between oxygen binding (the cooperative, allosteric equilibrium described in this chapter) and the structural pathology described in Chapter 2. The T-to-R transition is not just a curiosity of hemoglobin biochemistry; in HbS, it is the molecular switch that determines whether the protein causes disease. Therapeutic strategies that keep HbS in the R-state (by raising oxygen affinity, as voxelotor does by covalently modifying the N-terminus of the alpha chain to stabilize the R-state) prevent polymerization by preventing T-state formation.

This is also why any condition that lowers $pO_2$ precipitates sickle cell crises: high altitude, pulmonary infection, acidosis (via the Bohr effect, which shifts hemoglobin toward the T-state), and dehydration (which increases intracellular HbS concentration and raises the probability of polymerization). Every mechanism covered in this chapter maps directly onto a clinical trigger for vaso-occlusion.

---

## The MCAT Angle

### Oxygen Dissociation Curve Shifts

The most tested concept from this chapter is interpreting shifts in the oxygen-hemoglobin dissociation curve.

A **right shift** (increased $P_{50}$, decreased oxygen affinity) is caused by increased $H^+$ (decreased pH), increased $CO_2$, increased temperature, and increased 2,3-BPG. Right shift means hemoglobin releases oxygen more readily in the tissues. Remember the Bohr effect: high metabolism, high $CO_2$, low pH, right shift, more $O_2$ delivery.

A **left shift** (decreased $P_{50}$, increased oxygen affinity) is caused by decreased $H^+$ (increased pH), decreased $CO_2$, decreased temperature, and decreased 2,3-BPG. Left shift means hemoglobin holds oxygen more tightly and releases less in the tissues. Carbon monoxide causes a left shift on the remaining sites (locking R-state), and fetal hemoglobin has an intrinsic left shift due to weaker 2,3-BPG binding.

The mnemonic CADET, face RIGHT: $CO_2$, Acid, DPG (2,3-BPG), Exercise/elevated temperature, and Temperature all shift right. Everything else shifts left.

### Hill Coefficient and Cooperativity

A Hill coefficient of 1 means no cooperativity (hyperbolic curve). A Hill coefficient greater than 1 means positive cooperativity: binding of one ligand increases affinity at other sites. A Hill coefficient less than 1 means negative cooperativity: binding of one ligand decreases affinity at other sites (rare, but it exists, not with Hemoglobin ever though). Hemoglobin's Hill coefficient of about 2.8 reflects positive cooperativity among its four oxygen-binding sites.

If a question describes a mutation that disrupts subunit-subunit contacts in hemoglobin, what would you expect to happen to cooperativity? What would happen to the Hill Coeffecient?

### Allosteric Reasoning

The allosteric effectors of hemoglobin stabilize one conformational state preferentially. The reasoning framework:
- If an effector binds the T-state, the T-state is stabilized: oxygen affinity decreases, oxygen unloading increases, right shift, $P_{50}$ increases.
- If an effector binds the R-state, the R-state is stabilized: oxygen affinity increases, oxygen unloading *decreases*, left shift, $P_{50}$ decreases.
- 2,3-BPG binds the T-state: right shift.
- CO binds the R-state conformation (at non-oxygen sites, through the conformational mechanism): left shift on remaining sites.
- Protons bind residues stabilized in T-state: right shift (Bohr effect).

### CO Poisoning Reasoning

The two-mechanism nature of CO poisoning is a common MCAT target:
1. Direct competition: CO occupies heme binding sites, reducing the number of sites available for $O_2$ (reduces carrying capacity).
2. Allosteric effect: CO-bound subunits lock remaining subunits in R-state, decreasing oxygen delivery from those sites (impairs unloading).

The clinical consequence: CO is far more toxic per molecule than simple site blockade would suggest. A patient with 30% HbCO is not equivalent to a patient with 30% anemia.

---

## Worked Problems

### Problem 1: Binding Curve Reasoning

A researcher measures the oxygen-hemoglobin dissociation curves under two conditions: (A) pH 7.4 and standard 2,3-BPG, and (B) pH 7.0 and elevated 2,3-BPG.

(a) Predict the direction of the shift between conditions A and B and explain the molecular basis.

(b) Condition B approximates what is found in the capillaries of skeletal muscle during vigorous exercise. What is the physiological significance of this shift?

(c) If the hemoglobin had a Hill coefficient of 1 (no cooperativity) rather than 2.8, how would the oxygen delivery from conditions A to B change? Would the shift in $P_{50}$ have more or less impact on oxygen delivery?

**Solution:**

(a) Condition B shifts the curve to the right (higher $P_{50}$, lower oxygen affinity). Two factors contribute. First, lower pH (7.0 vs 7.4) means higher H$^+$ concentration. Protons bind Bohr residues such as His146 of the beta chain, stabilizing the T-state, which decreases oxygen affinity. This is the Bohr effect. Second, elevated 2,3-BPG concentrations provide more allosteric effector to bind in the central cavity of the T-state tetramer, further stabilizing the T-state and decreasing oxygen affinity. Both effects shift the curve in the same direction: right.

(b) Exercising muscle has low pH (from lactic acid and $CO_2$ production) and high 2,3-BPG (red blood cells produce more 2,3-BPG in response to increased glycolysis). Both conditions reduce hemoglobin's oxygen affinity in the exact location where oxygen demand is highest. The right-shifted curve means that at the low $pO_2$ of exercising muscle capillaries, hemoglobin releases a larger fraction of its oxygen cargo per pass than it would under resting conditions. This adaptive response is entirely automatic: the metabolic activity of the tissue generates the very molecules ($H^+$, $CO_2$, driving 2,3-BPG production) that enhance oxygen delivery to that tissue.

(c) With a Hill coefficient of 1 (hyperbolic curve), the curve is flat at the low-$pO_2$ end where tissues operate. The sigmoidal curve with $n = 2.8$ is steep in the physiological range (20 to 100 mmHg), meaning a shift in $P_{50}$ has a large effect on the fractional saturation at tissue $pO_2$ values. With a hyperbolic curve, the same $P_{50}$ shift produces a smaller change in saturation in the tissue range because the hyperbola is already flattening out there. Cooperativity amplifies the benefit of allosteric regulation: the sigmoidal curve makes the system more sensitive to changes in $P_{50}$ precisely where sensitivity matters most, in the physiological range.

---

### Problem 2: CO Poisoning Analysis

A 35-year-old firefighter is rescued from a burning building. Initial pulse oximetry reads 96%. Blood co-oximetry shows 35% carboxyhemoglobin (HbCO), 61% oxyhemoglobin ($HbO_2$), and 4% deoxyhemoglobin.

(a) Explain why the pulse oximeter reads 96% despite 35% HbCO.

(b) At the tissue level, explain why this patient is more severely hypoxic than a patient who simply had 35% of their hemoglobin destroyed by hemolysis (leaving 65% of normal hemoglobin that functions normally).

(c) The treatment team administers 100% $O_2$ via non-rebreather mask. Explain the mechanism by which this treatment reduces $HbCO$ levels.

**Solution:**

(a) Standard pulse oximetry uses two wavelengths of light (660 nm and 940 nm) and determines oxygen saturation from the ratio of absorption at these wavelengths. Oxyhemoglobin and deoxyhemoglobin have different absorption profiles, allowing the device to distinguish them. However, carboxyhemoglobin absorbs 660 nm light very similarly to oxyhemoglobin. The pulse oximeter interprets $HbCO$ as $HbO_2$. The device reports: $HbO_2 + HbCO = 61\% + 35\% = 96\%$, which is what it reads. The device is not malfunctioning; it simply lacks the spectral resolution to distinguish the two. Accurate measurement requires co-oximetry, which uses more than two wavelengths.

(b) A patient with hemolytic loss of 35% of their hemoglobin has 65% of normal hemoglobin that is fully functional: it is cooperative, responds to the Bohr effect and 2,3-BPG, and unloads oxygen appropriately in the tissues. At tissue $pO_2$ values (roughly 20 to 30 mmHg), this hemoglobin might release 30 to 40% of its cargo per pass. The CO-poisoned patient has 35% HbCO occupying binding sites AND an allosteric effect: CO locks the remaining hemoglobin subunits in the R-state (high-affinity), eliminating cooperativity for the mixed-CO molecules and preventing oxygen unloading. The hemoglobin molecules that contain CO and $O_2$ together arrive at the tissues at 98% saturation and leave at nearly the same saturation, having delivered very little. The hemolytic patient's 65% hemoglobin delivers oxygen; the CO patient's 61% $HbO_2$ largely cannot.

(c) Binding at the heme site is an equilibrium: $CO$ and $O_2$ compete for the same site, with CO having roughly 240 times higher affinity under equivalent partial pressures. This affinity ratio means that at equal partial pressures, hemoglobin will be predominantly CO-bound. However, the partial pressure of inspired $O_2$ can be manipulated. In room air, $pO_2$ is approximately 160 mmHg. At 100% $O_2$ through a non-rebreather mask (assuming minimal room air contamination), inspired $pO_2$ approaches 760 mmHg. By Le Chatelier's principle (or equivalently, by mass-action kinetics), greatly increasing the concentration of the competing ligand $O_2$ shifts the equilibrium away from $HbCO$. Although CO's off-rate is slow (reflecting its tight binding), it is not zero, and the elevated $pO_2$ ensures that any heme iron that dissociates $CO$ is rapidly rebound by $O_2$ rather than $CO$. The half-life of HbCO drops from roughly 5 hours in room air to 60 to 90 minutes on 100% $O_2$, and to 20 to 30 minutes in a hyperbaric chamber at 2 to 3 atmospheres, where $O_2$ partial pressure is 1,500 to 2,280 mmHg.

---

### Problem 3: Allosteric Effector Reasoning

A pharmacologist designs a drug that binds to the central cavity of deoxyhemoglobin (the same site as 2,3-BPG) but has much higher affinity than 2,3-BPG. The drug is administered to evaluate its effect on oxygen delivery.

(a) Predict the effect of this drug on the shape and position of the oxygen-hemoglobin dissociation curve.

(b) Under what physiological circumstances might such a drug be harmful? Under what circumstances might it be beneficial?

(c) A second drug is designed that binds only to the R-state of hemoglobin, stabilizing it. How would this drug's effect on the dissociation curve differ from the first drug?

**Solution:**

(a) By binding the same site as 2,3-BPG with higher affinity, the drug selectively and strongly stabilizes the T-state (deoxyhemoglobin conformation). This shifts the T-to-R equilibrium toward T, decreasing oxygen affinity. The oxygen-hemoglobin dissociation curve shifts to the right (higher $P_{50}$). The sigmoidal shape is likely preserved (cooperativity still depends on subunit-subunit communication, which this drug does not disrupt), but the midpoint of the transition is at a higher $pO_2$. In extreme cases, if the drug shifts $P_{50}$ to 60 to 80 mmHg, hemoglobin might not be adequately loaded even in the lungs.

(b) Harmful circumstances: at altitude, where $pO_2$ in the lungs is already reduced, a further reduction in oxygen affinity would impair loading and cause hypoxia. In pulmonary disease (low lung $pO_2$), the same problem. In anemia, where there is little reserve capacity, decreasing the efficiency of whatever hemoglobin is present is dangerous. For any patient with compromised oxygen loading at the lungs, a rightward shift reduces saturation at the point where it needs to be highest.

Beneficial circumstances: sickle cell disease, as noted in the chapter, is worsened by T-state formation. A drug that stabilizes the T-state would in principle worsen sickling (which is exactly the opposite of what is therapeutic). However, a rightward shift might benefit patients with left-shifted hemoglobin variants or in conditions where enhanced $O_2$ unloading is the goal. Hemoglobin Kansas (a naturally occurring variant with reduced cooperativity and a right-shifted curve) presents with mild cyanosis but preserved tissue oxygenation, illustrating that moderate right shifts are tolerable at sea level with normal lungs.

(c) A drug that stabilizes the R-state shifts the equilibrium in the opposite direction: it decreases the effective T-state population, increases oxygen affinity, and shifts the dissociation curve to the left (lower $P_{50}$). Hemoglobin holds oxygen more tightly at all $pO_2$ values. This is the mechanism of voxelotor, a drug approved for sickle cell disease: it modifies the N-terminus of the alpha chain covalently to stabilize the R-state, preventing the T-state formation that enables HbS polymerization. The tradeoff is that a very left-shifted curve reduces oxygen unloading in the tissues. The clinical strategy is to stabilize enough R-state to prevent sickling while not shifting the curve so far left that tissue hypoxia results. The therapeutic window is determined by the relationship between the dissociation curve and tissue $pO_2$ requirements: a quantitative binding problem with direct clinical consequences.

---

## Opener Questions Revisited

**Question 1:** What property of a binding protein allows it to carry vastly more oxygen than simple dissolution, and what limits how much more it could carry?

The key property is the existence of a specific, high-affinity binding site. Hemoglobin does not simply dissolve oxygen; it binds it with a defined $K_d$, concentrating oxygen in the binding site far beyond what Henry's law would allow for a simple solution. Each hemoglobin molecule binds four oxygens; each red blood cell contains 280 million hemoglobin molecules; blood carries about 65 times more oxygen per unit volume than plasma alone.

The limit on additional concentration is set by the on-rate and off-rate of the binding interaction. A protein with a lower $K_d$ (tighter binding) would carry more oxygen but would not release it in the tissues: tight binding means a slow off-rate, and a slow off-rate means the oxygen never leaves. Myoglobin has a $P_{50}$ of about 2 mmHg: it carries oxygen very tightly and does not release it at tissue pO$_2$ values. It is not a useful systemic transporter precisely because its binding is too tight for delivery. Hemoglobin's $K_d$ is tuned (by cooperativity and allosteric effectors) to be in the physiological range where loading in the lungs and unloading in the tissues are both efficient. The limit is not how much you can carry, but whether what you carry can be released where it is needed.

**Question 2:** How does a patient with 35% HbCO read 98% on a pulse oximeter while dying from hypoxia?

The pulse oximeter operates at two wavelengths (660 nm and 940 nm) calibrated to distinguish oxyhemoglobin from deoxyhemoglobin. Carboxyhemoglobin absorbs 660 nm light nearly identically to oxyhemoglobin, so the device cannot distinguish HbCO from $HbO_2$ and reports both together as "saturated." The measurement is technically accurate for what the device is measuring, but that measurement is not functional oxygen saturation; it is the sum of $HbO_2$ and HbCO, irrespective of whether either is actually delivering oxygen.

The deeper point is that what "oxygen saturation" measures matters less than what the hemoglobin is doing with its oxygen. Even the 61% $HbO_2$ in this patient is partially non-functional: CO locks the remaining binding sites in the R-state (high affinity), preventing cooperative unloading in the tissues. The patient has hemoglobin that is nominally loaded with oxygen but cannot efficiently release it where it is needed. The correct measurement requires co-oximetry. The correct treatment exploits the reversibility of binding: flood the system with high- $pO_2$ oxygen, shift the competitive equilibrium away from CO, and restore functional hemoglobin.

Binding chemistry is not an abstraction. In this patient, the difference between a correct and incorrect understanding of hemoglobin's binding properties is the difference between appropriate treatment and reassurance based on a number that means almost nothing.

---

*Chapter 4: Enzymes and Catalysis*
