# Chapter 12: The Electron Transport Chain and Oxidative Phosphorylation

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. A firefighter is pulled unconscious from a burning building. The building contained synthetic materials that released cyanide-containing smoke in addition to carbon monoxide. In the emergency department his carboxyhemoglobin is elevated, and your team gives 100% oxygen to displace the CO. A colleague argues this is sufficient treatment. You disagree: you believe there may be a cellular component to the poisoning that oxygen therapy alone will not fix. Who is right, and why?

2. A pharmaceutical company tests a new compound that binds tightly to the c-ring of the ATP synthase $\text{F}_0$ subunit in isolated mitochondria. When added to mitochondria supplied with NADH and oxygen, the compound causes oxygen consumption to slow dramatically, the proton gradient across the inner membrane to rise, and ATP production to stop. The researchers then add FCCP, a well-known uncoupler (a small lipid-soluble molecule that ferries protons across the inner mitochondrial membrane, bypassing ATP synthase and collapsing the proton gradient). Predict what happens to oxygen consumption, proton gradient magnitude, and ATP production. What does this experiment tell you about how the electron transport chain and ATP synthesis are connected?

---

## The Big Picture

We left Chapters 10 and 11 having converted glucose all the way to $\text{CO}_2$, generating 10 NADH, 2 $\text{FADH}_2$, and 4 direct ATP equivalents per glucose. The chemistry is satisfying, but the real payoff is still coming. Those 10 NADH and 2 $\text{FADH}_2$ are loaded electron carriers, storing the chemical potential energy extracted from glucose oxidation as electrons held at high energy. The electron transport chain and oxidative phosphorylation convert that potential into ATP.

Here is the conceptual move that everything else depends on. High-energy electrons from NADH and $\text{FADH}_2$ are passed down a series of membrane-embedded protein complexes toward oxygen. At each transfer step the electrons drop to a lower energy level, and that energy is not wasted as heat. It is captured: used to pump protons from the mitochondrial matrix across the inner mitochondrial membrane into the intermembrane space. This creates a proton gradient, a difference in both concentration and charge across the membrane. ATP synthase then uses the flow of protons back into the matrix to drive the phosphorylation of ADP. The chain is the proton pump. ATP synthase is the turbine that runs on the gradient the chain builds.

This is **chemiosmosis**, and it was one of the most counterintuitive ideas in twentieth-century biochemistry. When Peter Mitchell proposed it in 1961, most biochemists expected to find a high-energy phosphorylated chemical intermediate linking electron transport to ATP synthesis, the same logic as substrate-level phosphorylation. There wasn't one. Mitchell argued instead that the intermediate is a gradient: a physical asymmetry across a membrane. He won the Nobel Prize in 1978. The key insight is that you cannot understand oxidative phosphorylation from a balanced equation alone. The membrane is the machine.

---

## The Inner Mitochondrial Membrane

The physical setting matters here. The mitochondrion has two membranes:

The **outer mitochondrial membrane** is relatively permeable. It contains large pores (the voltage-dependent anion channels, or VDACs) that allow small molecules including ATP, ADP, pyruvate, and most metabolites to pass freely. It is not a bioenergetic barrier.

The **inner mitochondrial membrane (IMM)** is where the action is. It is one of the most impermeable biological membranes known, essentially impermeable to protons, hydroxide ions, and most charged or polar molecules. This impermeability is not incidental; it is the whole point. A proton gradient can only do useful work if the membrane does not leak.

The inner membrane is highly folded into structures called **cristae**, which dramatically increase its surface area. More surface area means more room for the complexes and ATP synthase.

Between the two membranes is the **intermembrane space (IMS)**. Inside the inner membrane is the **matrix**, where the TCA cycle runs and where NADH and $\text{FADH}_2$ are produced.

The four respiratory complexes (I through IV) and ATP synthase (sometimes called Complex V) are all embedded in the inner membrane. They are not uniformly scattered: they are organized into large assemblies called **supercomplexes** (or respirasomes), particularly I + $\text{III}_2$ + IV, an area of active research whose functional significance is still being characterized. For the purpose of understanding function, we can treat the complexes as sequentially connected through two mobile electron carriers: **ubiquinone (CoQ)** in the membrane and **cytochrome c** in the intermembrane space.

---

## Mobile Electron Carriers

Two small molecules ferry electrons between the fixed complexes:

**Ubiquinone (coenzyme Q, CoQ)** is a lipid-soluble molecule that diffuses laterally within the inner membrane. Its quinone ring can accept two electrons and two protons from either NADH-linked or $\text{FADH}_2$-linked sources, becoming **ubiquinol ($\text{QH}_2$)**. It then delivers those electrons to Complex III. Because CoQ is lipophilic and free to move in the membrane, it collects electrons from both Complex I and Complex II (and from other FAD-linked dehydrogenases, including the electron-transferring flavoprotein dehydrogenase involved in fatty acid oxidation) and funnels all of them to Complex III. CoQ is the convergence point for electrons from NADH and $\text{FADH}_2$.

The standard reduction potential of the CoQ/QH₂ couple is approximately +0.045 V, placing it energetically between the upstream donors (NADH at −0.32 V; the succinate/fumarate couple that drives FAD reduction in Complex II at approximately +0.03 V) and the downstream acceptors. Note that free FAD/FADH₂ in solution has E°' ≈ −0.18 V; the value relevant here is the succinate/fumarate couple, because that is what reduces the covalently bound FAD in Complex II.

**Cytochrome c** is a small, water-soluble protein in the intermembrane space. It contains a heme group whose iron cycles between $\text{Fe}^{3+}$ (oxidized) and $\text{Fe}^{2+}$ (reduced). It accepts electrons one at a time from Complex III and delivers them to Complex IV. Unlike CoQ, which carries two electrons simultaneously, cytochrome c carries one at a time.

Cytochrome c doubles as a pro-apoptotic signal. When the outer mitochondrial membrane is permeabilized during programmed cell death, cytochrome c is released into the cytoplasm, where it assembles a complex that activates caspases. A protein that spends its normal life shuttling electrons in respiration also serves as a death trigger, an interesting example of evolution reusing components.

---

## The Four Complexes

### Complex I: NADH-CoQ Oxidoreductase (NADH Dehydrogenase)

$$\text{NADH} + \text{H}^+ + \text{CoQ} \rightarrow \text{NAD}^+ + \text{QH}_2 \qquad (\Delta G^{\circ'} \approx -69 \text{ kJ/mol})$$

Complex I is the entry point for electrons from NADH. It is the largest of the respiratory complexes: in humans it contains about 45 subunits and has an L-shaped structure with one arm embedded in the membrane and one arm projecting into the matrix. The matrix arm is where NADH is oxidized, and electrons flow through a series of **iron-sulfur clusters** until they reach ubiquinone at the membrane arm. Iron-sulfur clusters are small inorganic cofactors built from iron and sulfide ions arranged in cage-like structures, most commonly [2Fe-2S] or [4Fe-4S]. Each cluster can accept and donate exactly one electron, with the iron cycling between $\text{Fe}^{2+}$ and $\text{Fe}^{3+}$. Strung together in a chain, they act as a wire: electrons hop from cluster to cluster, stepping down in energy with each transfer, until they reach the final acceptor. You will see them in Complexes I, II, and III, and they are also the functional center of aconitase in the TCA cycle. CoQ accepts two electrons and two protons from the matrix, becoming $\text{QH}_2$ and entering the lipid phase of the membrane.

For every pair of electrons passed through Complex I (one NADH oxidized), **4 protons are pumped from the matrix to the intermembrane space.** This is the largest proton contribution of any single complex.

How does that pumping actually work? The honest answer is that the full atomic mechanism is still being worked out, but the conceptual picture is clear. The key feature is that Complex I's two arms are physically far apart: electron transfer happens entirely in the matrix arm, but the proton-translocating machinery is entirely in the membrane arm, about 10 nm away. There is no direct chemical coupling of the kind we saw in substrate-level phosphorylation. Instead, the coupling is **mechanical and conformational**. As electrons step down through the iron-sulfur chain and ultimately reduce CoQ, the energy released drives a series of conformational changes that propagate through the membrane arm like a wave. The membrane arm contains three antiporter-like subunits whose structures are similar to bacterial $\text{Na}^+$/$\text{H}^+$ antiporters; the conformational wave drives each of them to translocate a proton across the membrane. The redox chemistry and the proton pumping are coordinated by shape changes, not by shared chemical intermediates. This is fundamentally different from Complex III, where the proton pumping is a direct consequence of the Q cycle chemistry, and from Complex IV, where some of the pumped protons are consumed as substrates in forming water. Complex I is a molecular machine that converts electron-transfer energy into mechanical motion that drives proton translocation.

Complex I is inhibited by **rotenone**, a plant-derived insecticide used in pest control and aquatic management, and by **metformin**, which at therapeutic doses modestly inhibits Complex I in the liver. Metformin's Complex I inhibition is thought to contribute to its mechanism of reducing hepatic glucose output, though this remains an active area of research.

Complex I is also a major source of reactive oxygen species in the cell. When electron transport slows and the CoQ pool becomes highly reduced (in the chemical sense: loaded with electrons, i.e., most CoQ exists as $\text{QH}_2$ rather than the oxidized form), electrons can leak from iron-sulfur clusters directly to oxygen, producing superoxide. This is the biochemical basis for the connection between mitochondrial dysfunction and oxidative stress.

### Complex II: Succinate-CoQ Oxidoreductase (Succinate Dehydrogenase)

You already know Complex II from Chapter 11. It is identical to succinate dehydrogenase, the enzyme that catalyzes step 6 of the TCA cycle. Complex II accepts electrons from succinate oxidation through FAD, through iron-sulfur clusters, and delivers them to CoQ.

The critical point: **Complex II does not pump protons.** It transfers electrons to the CoQ pool without translocating any protons across the membrane. This is why $\text{FADH}_2$ yields fewer ATP than NADH: its electrons bypass Complex I's proton pumping entirely. They enter the chain at CoQ, proceed through Complex III and IV only, and those two complexes together pump fewer protons than the full I + III + IV path.

Other $\text{FADH}_2$-linked dehydrogenases, such as the electron-transferring flavoprotein (ETF) dehydrogenase that handles electrons from fatty acid β-oxidation, similarly feed electrons into the CoQ pool without Complex I. All of them yield 1.5 ATP per electron pair, not 2.5.

SDH subunit mutations are tumor suppressors, as described in Chapter 11. Succinate accumulation from SDH loss stabilizes HIF-1α and drives pseudohypoxic tumor behavior.

### Complex III: CoQ-Cytochrome c Oxidoreductase (Cytochrome bc$_1$ Complex)

$$\text{QH}_2 + 2 \text{ cyt } c^{3+} \rightarrow \text{CoQ} + 2 \text{ cyt } c^{2+} + 4\text{H}^+ \text{ (IMS side)}$$

Complex III transfers electrons from $\text{QH}_2$ to cytochrome c, one electron at a time. The challenge is that $\text{QH}_2$ carries two electrons but cytochrome c accepts only one. Complex III solves this via the **Q cycle**, described below.

#### The Q Cycle

Start with the problem. $\text{QH}_2$ is a two-electron carrier. Cytochrome c is a one-electron carrier. You cannot directly hand two electrons from $\text{QH}_2$ to cytochrome c: the mismatch in electron valency requires a switching mechanism. The Q cycle is that mechanism, and the reason it matters is that it doubles the number of protons translocated compared to a simpler direct transfer would achieve.

Complex III has two distinct binding sites for ubiquinone:

- **Qo site (outer, IMS-facing):** where $\text{QH}_2$ is oxidized
- **Qi site (inner, matrix-facing):** where CoQ is reduced back to $\text{QH}_2$

The cycle proceeds in two rounds, each beginning with one $\text{QH}_2$ arriving at the Qo site:

**Round 1:**

A molecule of QH₂ binds at the Qo site and is oxidized and one molecule of Q binds at the Qi site. Its two electrons are split: one goes to the high-potential chain (an iron-sulfur protein in Complex III, then to cytochrome c$_1$, then to cytochrome c in the IMS), reducing one cytochrome c. The other electron takes the low-potential path: it travels to cytochrome b_L, then to cytochrome b_H, and reduces the Q at the Qi site to a semiquinone radical ($\text{Q}^{\bullet-}$). Meanwhile, the two protons from $\text{QH}_2$ oxidation are released into the IMS.

**Round 2:**

A second $\text{QH}_2$ arrives at the Qo site and is oxidized in the same way. Again one electron goes via the high-potential chain to reduce a **second** cytochrome c. The other electron travels down the cytochrome b chain to the Qi site and reduces the semiquinone $\text{Q}^{\bullet-}$ (left over from the last round) all the way to $\text{QH}_2$, picking up 2 protons from the matrix in the process.

**The net result for two $\text{QH}_2$ consumed:**

- 2 electrons have been delivered to 2 cytochrome c molecules (net output)
- 1 $\text{QH}_2$ has been regenerated at the Qi site from 2 matrix protons and the two recycled electrons
- 4 protons have appeared in the IMS: 2 from the first $\text{QH}_2$ oxidation and 2 from the second

So for every 2 electrons that actually leave Complex III toward cytochrome c, **4 protons are translocated to the IMS**. The Q cycle effectively doubles the proton yield by routing one electron from each $\text{QH}_2$ backward through a recycling loop instead of dumping it, picking up 2 matrix protons in the process. The "wasted" electron is not wasted at all; it is the mechanism.

This is also why **antimycin A** is so effective as an inhibitor. It blocks the Qi site, preventing the semiquinone from being reduced to $\text{QH}_2$. With the Qi site blocked, the first electron from each $\text{QH}_2$ can still reduce cytochrome c, but the second electron accumulates as a semiquinone radical at the Qo site. Semiquinone is highly reactive and will donate its electron directly to oxygen, producing superoxide. Antimycin A does not just block electron flow; it converts Complex III into a superoxide generator.


### Complex IV: Cytochrome c Oxidase

$$4 \text{ cyt } c^{2+} + 4\text{H}^+ + \text{O}_2 \rightarrow 4 \text{ cyt } c^{3+} + 2\text{H}_2\text{O}$$

Complex IV is the terminal enzyme. It accepts four electrons from four cytochrome c molecules one at a time and delivers them to molecular oxygen, reducing it completely to two water molecules. This is the reaction that makes aerobic respiration aerobic: oxygen is the **final electron acceptor**.

The chemistry is genuinely tricky. Partial reduction of oxygen is dangerous: superoxide ($\text{O}_2^{\bullet-}$) and hydrogen peroxide are toxic intermediates (more specifically **reactive oxygen species (ROS)**). Complex IV performs a full four-electron reduction without releasing these partially reduced species, holding all intermediates tightly at its active site until all four electrons have arrived. The catalytic center contains two copper centers ($\text{Cu}_\text{A}$ and $\text{Cu}_\text{B}$) and two heme groups (heme a and heme a$_3$). $\text{Cu}_\text{A}$ accepts electrons from cytochrome c, heme a passes them to the binuclear center formed by heme a$_3$ and $\text{Cu}_\text{B}$, and that is where $\text{O}_2$ binds and is reduced.

Here is how the four electrons are used, step by step. The first pair of electrons, arriving via the relay described above, reduces the binuclear center: heme a$_3$ iron goes from $\text{Fe}^{3+}$ to $\text{Fe}^{2+}$, and $\text{Cu}_\text{B}$ goes from $\text{Cu}^{2+}$ to $\text{Cu}^{+}$. $\text{O}_2$ then binds to the $\text{Fe}^{2+}$ of heme a$_3$. The two electrons already sitting in the binuclear center immediately donate into the $\text{O}_2$, forming a **peroxide bridge**: $\text{Fe}^{3+}-\text{O}-\text{O}-\text{Cu}^{2+}$. The two oxygens are now bridging the two metal centers, each holding one of the donated electrons. This is the critical intermediate, and it is why the toxic partials never escape: both oxygen atoms are held simultaneously by the two metals before the O–O bond is broken.

The second pair of electrons then arrives from cytochrome c, one at a time, and along with two protons abstracted from the matrix, cleaves the O–O bond. Each oxygen receives a total of two electrons and one proton, producing two metal-bound hydroxyl groups: $\text{Fe}^{3+}-\text{OH}$ on heme a$_3$ and –OH on $\text{Cu}_\text{B}$. Finally, two more protons from the matrix protonate these hydroxyl groups, releasing two molecules of water and returning the binuclear center to its oxidized resting state, ready for the next $\text{O}_2$. The full accounting: four electrons in, four matrix protons consumed, one $\text{O}_2$ reduced, two $\text{H}_2\text{O}$ released. None of the partially reduced intermediates leave the active site at any stage.

For every four electrons transferred (one O₂ reduced), Complex IV pumps **4 protons from the matrix to the IMS**, and consumes 4 protons from the matrix to form water. Net translocation from matrix to IMS: 4 $\text{H}^+$ per $\text{O}_2$ reduced, or 2 $\text{H}^+$ per pair of electrons.

Complex IV is the target of several clinically important inhibitors:

- **Cyanide ($\text{CN}^-$)**: binds to the $\text{Fe}^{3+}$ form of heme a$_3$, blocking $\text{O}_2$ binding
- **Carbon monoxide (CO)**: binds to the $\text{Fe}^{2+}$ form of heme a$_3$, blocking $\text{O}_2$ reduction
- **Azide ($\text{N}_3^-$)**: binds the binuclear center and blocks it
- **Hydrogen sulfide ($\text{H}_2\text{S}$)**: inhibits at high concentrations

All four stop the terminal step of electron transport. Electrons back up through the chain and proton pumping ceases, because pumping is driven by electron flow and there is nowhere for electrons to go. Meanwhile ATP synthase continues to drain the existing PMF. With pumping stopped and consumption continuing, the gradient is depleted without being replenished, and ATP synthesis stops once the PMF is exhausted. The clinical consequences are covered below in "When It Breaks."

---

## The Proton-Motive Force

The four complexes pump protons from the matrix into the intermembrane space, building an electrochemical gradient across the inner membrane. This gradient has two components:

1. **A concentration gradient (ΔpH):** The IMS becomes more acidic than the matrix because protons accumulate there.
2. **An electrical potential (ΔV):** The IMS becomes more positive than the matrix, because protons carry positive charge.

Together these constitute the **proton-motive force (PMF)**:

$$\Delta p = \Delta V - \frac{2.303 RT}{F}\Delta\text{pH}$$

This equation is simply derived from the electrochemical gradient equation from chapter 6:

$$\Delta G = RT\ln{\frac{c_f}{c_i}}+ZF\Delta V$$

Where $c_f=10^{-\text{pH}_{\text{mat}}}$ and $c_i=10^{-\text{pH}_{\text{ims}}}$. Substituting those values produces:

$$\Delta G = RT\ln{\frac{10^{-\text{pH}_{\text{mat}}}}{10^{-\text{pH}_{\text{ims}}}}}+ZF\Delta V$$

Rearranging this equation:

$$\Delta G = RT\ln(10^{\text{pH}_\text{ims}-\text{pH}_\text{mat}})+ZF\Delta V$$

Defining $\Delta\text{pH}=\text{pH}_\text{mat}-\text{pH}_\text{ims}$ and extracting the exponent from the logarithm gives us:

$$\Delta G = (-\Delta\text{pH})RT\ln(10)+ZF\Delta V$$

ln(10)=2.303, Z=+1, dividing both sides by F, defining $\Delta p=\frac{\Delta G}{F}$ gives us the final form:

$$\Delta p = \Delta V - \frac{2.303 RT}{F}\Delta\text{pH}$$

where $\Delta V$ is the membrane potential and the second term is the pH contribution. Under physiological conditions in mitochondria, the membrane potential ($\Delta V \approx -160$ mV, matrix negative) contributes about 80% of the total PMF, with the pH gradient providing the remaining 20%.

Why divide by F at all? Dividing $\Delta G$ (in kJ/mol) by F (in C/mol) gives units of J/C, which is volts. Expressing the PMF in volts is convenient for two reasons. First, the electrical component $\Delta V$ is already a voltage and is directly measured in mV; expressing the whole equation in the same units lets you see at a glance how much each component contributes. Second, it connects the PMF directly to the reduction potential framework from Chapter 9: just as $\Delta G = -nF\Delta E$ lets us convert between free energy and electrode potentials, dividing by $F$ here converts free energy per mole of protons into an equivalent voltage. You could just as well work with $\Delta G$ in kJ/mol throughout; you would just multiply both sides by $F$ every time you wanted to compare the electrical and chemical contributions, which is less convenient. The voltage form of the PMF ($\approx -220$ mV under typical mitochondrial conditions; $\Delta\text{pH}=1.0$, $\Delta V=-160\text{mV}$) is the one you will see in physiology and bioenergetics literature. This -220mV corresponds to a $\Delta G$ of -21.2kJ/mol (0.22V*F).

The PMF represents stored potential energy, comparable to water behind a dam. When the chain is running and the synthase is consuming the gradient as fast as it is built, the PMF sits at a steady-state level that reflects the balance between pumping and consumption. If the chain is blocked, proton pumping stops while ATP synthase continues draining the existing gradient, so the PMF falls until ATP synthesis stops. If the synthase is blocked instead, the chain keeps pumping but protons cannot return, and the PMF rises until the back-pressure stalls the complexes.

---

## ATP Synthase (Complex V)

ATP synthase is the machine that converts the proton gradient, Δp, into ATP. It is a molecular rotary motor, and it is one of the most remarkable molecular machines in biology.

The enzyme has two main domains:

**$\text{F}_0$ (the membrane domain):** Embedded in the inner membrane, $\text{F}_0$ consists of a ring of c-subunits (the c-ring, typically 8 c-subunits in humans) anchored in the lipid bilayer. Protons from the intermembrane space enter through a half-channel in the a-subunit, bind to a glutamate residue on the c-ring, travel around the ring as it rotates, and exit through a second half-channel into the matrix. Each proton that completes this transit rotates the ring by one c-subunit position.

**$\text{F}_1$ (the catalytic domain):** Protrudes into the matrix. It consists of three αβ-subunit pairs surrounding a central γ-subunit shaft, which is physically connected to the rotating c-ring. As the c-ring rotates, the γ-shaft rotates within the $\alpha_3\beta_3$ assembly. The three β-subunits cycle through three conformational states, with one subunit in each state at any given moment. A single subunit progresses: **O (open) $\rightarrow$ L (loose) $\rightarrow$ T (tight) $\rightarrow$ back to O.** Each 120° rotation of the γ-shaft advances each subunit one step forward.

Paul Boyer and John Walker shared one half of the 1997 Nobel Prize in Chemistry for working out this rotary mechanism. (The other half went to Jens C. Skou for the discovery of the $\text{Na}^+$/$\text{K}^+$-ATPase.) Boyer's key insight: the energy of proton flow is not used to drive the chemistry of phosphate transfer directly (that chemistry is near equilibrium in the tight site). Instead, it drives the conformational changes that release ATP from the enzyme, which would otherwise bind too tightly to leave. The hard step is not making ATP; it is letting go of it.

**How many protons per ATP?** The c-ring size varies across organisms: 8 subunits in humans and other mammals, 10 in *E. coli* and yeast, 14 in spinach chloroplasts, up to 15 in some cyanobacteria. Larger rings require more protons per rotation and yield fewer ATP per proton, which is why the P/O ratio differs between mitochondria and chloroplasts. In humans, the c-ring has 8 subunits. One complete 360° rotation requires 8 protons and synthesizes 3 ATP (one per β-subunit, one rotation per 3 ATPs), giving 8/3 ≈ 2.7 protons per ATP from the synthase alone. Adding the proton cost of importing ADP and $P_i$ into the matrix and exporting ATP out (via the adenine nucleotide translocase, which exchanges matrix ATP for cytoplasmic ADP using one proton's worth of energy per transport cycle), the effective cost is approximately **4 protons per ATP** synthesized and exported.

### Following a Proton Through $\text{F}_0$

The a-subunit contains two half-channels that do not connect to each other. One opens exclusively to the IMS; the other opens exclusively to the matrix. Each half-channel provides access to a single adjacent c-subunit on the ring. A proton from the IMS enters the IMS-facing half-channel and reaches a conserved glutamate (or aspartate) residue on the nearest c-subunit. Because the effective pKa of this residue is around 5–6, the low pH of the IMS drives it toward protonation. The proton binds, the residue becomes neutral, and that c-subunit is now uncharged and stable in the hydrophobic interior of the membrane.

On the other side of the ring, a different c-subunit is positioned at the matrix-facing half-channel. Exposed to the more alkaline matrix, its glutamate is deprotonated and carries a negative charge. A charged residue in a hydrophobic lipid bilayer is thermodynamically very unfavorable, so the ring rotates to move that subunit out of the membrane and toward the IMS half-channel, where it can pick up a proton and become neutral again. Simultaneously, the newly protonated subunit rotates away from the IMS channel and into the membrane, where it is now stable. The direction of rotation is determined by the electrochemical gradient: protonation at the IMS side and deprotonation at the matrix side are both thermodynamically favorable, and that asymmetry enforces one rotational direction. Every c-subunit in the ring carries a proton through the hydrophobic membrane in the same direction, one step at a time.

Eventually the proton we started with arrives at the matrix-facing half-channel, the glutamate releases it into the alkaline matrix, and it has completed its transit from IMS to matrix. The free energy released by this downhill movement is approximately $\Delta G = F\Delta p \approx 96{,}485 \text{ C/mol} \times 0.220 \text{ V} \approx 22 \text{ kJ/mol}$ per proton. That energy is not dissipated as heat. It was spent rotating the c-ring.

### From Ring Rotation to ATP: The β-Subunit Cycle

The c-ring is mechanically coupled to the γ-shaft, which extends down into the center of the $\alpha_3\beta_3$ hexamer of $\text{F}_1$. The γ-shaft is asymmetric: it presents three distinct faces along its long axis, one in contact with each β-subunit at any given moment. As the shaft rotates, each β-subunit encounters each face in sequence, and the face it is in contact with determines its conformation.

The three conformations and their roles in the synthesis cycle:

- **O (open):** The β-subunit is open to the solvent. ADP and $P_i$ diffuse in from the matrix, or ATP exits after the previous round.
- **L (loose):** ADP and $P_i$ are enclosed within the β-subunit. They are held, but the chemistry has not yet occurred.
- **T (tight):** The β-subunit clamps down tightly on the substrates. ADP and $P_i$ are held with very high affinity and the phosphoryl transfer reaction runs: ATP is formed. As Boyer showed, this step is not energetically difficult; the chemistry is near equilibrium at the T site.

The step that actually requires energy input is the T $\rightarrow$ O transition, where the subunit opens and releases ATP. ATP is bound so tightly in the T conformation that it would not leave spontaneously; the mechanical rotation of the γ-shaft forces the subunit open, ejecting ATP into the matrix. Boyer's binding change mechanism states that the energy from proton transit goes not into making the phosphoanhydride bond but into releasing the product.

Since all three β-subunits are advancing one step per 120° rotation, each full 360° rotation of the c-ring (8 protons, in humans) drives all three subunits through one complete O $\rightarrow$ L $\rightarrow$ T $\rightarrow$ O cycle, releasing one ATP each, for a total of 3 ATP per rotation.

---

## Proton Accounting and ATP Yield

In humans 1 rotation moves 8 protons into the matrix and produces 3 ATP. We also know that oxidizing one NADH drives the pumping of ~10 protons from the matrix into the IMS, and oxidizing one $\text{FADH}_2$ drives ~6 protons. Those IMS protons are what flows back through the c-ring to power rotation.

With approximately 4 $\text{H}^+$ per ATP:

**For NADH (enters at Complex I):**

| Complex | $\text{H}^+$ pumped per electron pair |
|---|---|
| Complex I | 4 |
| Complex III | 4 |
| Complex IV | 2 |
| **Total** | **~10 $\text{H}^+$ per NADH** |

$$\frac{1 \cancel{\text{NADH}}}{1}\times \frac{10 \cancel{\text{H}^+}}{\cancel{\text{NADH}}} \times \frac{1 \cancel{\text{rot}}}{8 \cancel{\text{H}^+}} \times \frac{3 \text{ATP}}{1 \cancel{\text{rot}}} = 3.75 \text{ ATP}$$

This gives 3.75, not 2.5. The calculation is correct as far as it goes, but it only accounts for the ATP synthase c-ring stoichiometry. Two additional transport costs are missing.

The first is the **adenine nucleotide translocase (ANT)**, which exports $\text{ATP}^{4-}$ from the matrix in exchange for $\text{ADP}^{3-}$ from the IMS. Because ATP carries one more negative charge than ADP, each cycle moves one net negative charge out of the already-negative matrix. This is thermodynamically equivalent to consuming one $\text{H}^+$ equivalent from the electrical component of the PMF (ΔΨ) per ATP.

The second is the **phosphate carrier (PiC)**, which imports $\text{H}_2\text{PO}_4^-$ into the matrix in exchange for $\text{OH}^-$. Because this exchange is electrically neutral (both species carry −1 charge), it does not draw on ΔΨ, but exporting $\text{OH}^-$ from the alkaline matrix is thermodynamically equivalent to consuming one $\text{H}^+$ equivalent from the chemical (ΔpH) component of the PMF per $P_i$ imported.

The reason the combined transport cost is approximately 1.33 H⁺ rather than 2 is that ANT and PiC draw on different components of the PMF. ΔΨ accounts for roughly 80% of the total PMF and ΔpH for roughly 20%, so each transporter consumes its respective component, and those components are not equal in magnitude. The combined additional cost works out to approximately 1.33 $\text{H}^+$ equivalents per ATP, bringing the total to 8/3 + 1.33 ≈ 4 $\text{H}^+$ per ATP.

The "~4 $\text{H}^+$ per ATP" figure used below is the shorthand that already incorporates the synthase, the ANT, and the PiC:

ATP yield: 10 / 4 = **~2.5 ATP per NADH**

**For $\text{FADH}_2$ (enters at Complex II, bypasses Complex I):**

| Complex | $\text{H}^+$ pumped per electron pair |
|---|---|
| Complex III | 4 |
| Complex IV | 2 |
| **Total** | **~6 $\text{H}^+$ per $\text{FADH}_2$** |

ATP yield: 6 / 4 = **~1.5 ATP per $\text{FADH}_2$**

These are the **P/O ratios** (P for phosphate incorporated into ATP, O for oxygen atom reduced at Complex IV; the ratio expresses how many ATPs are made per oxygen atom consumed) you will use throughout this course and for the MCAT/DAT: **2.5 per NADH and 1.5 per $\text{FADH}_2$.** Older textbooks used 3 and 2; those values date from before the precise proton stoichiometry was determined and are no longer considered accurate.

### Complete ATP Accounting Per Glucose

Combining with yields from Chapters 10 and 11:

| Stage | NADH | $\text{FADH}_2$ | Direct ATP/GTP |
|---|---|---|---|
| Glycolysis | 2 (cytoplasmic) | — | 2 |
| PDH (×2) | 2 (mitochondrial) | — | — |
| TCA (×2 turns) | 6 (mitochondrial) | 2 | 2 |
| **Totals** | **10** | **2** | **4** |

Converting to ATP:
- 8 mitochondrial NADH × 2.5 = 20 ATP
- 2 $\text{FADH}_2$ × 1.5 = 3 ATP
- 4 direct ATP/GTP = 4 ATP
- 2 cytoplasmic NADH (see shuttle section below): 3–5 ATP depending on shuttle

**Grand total: approximately 30–32 ATP per glucose**, consistent with what we stated at the end of Chapter 11. The range reflects shuttle variability, described next.

---

## The Cytoplasmic NADH Problem: Shuttle Systems

Glycolysis produces 2 NADH per glucose in the cytoplasm. The ETC is inside the mitochondrial matrix. NADH cannot cross the inner membrane, because the IMM is impermeable to it. To transfer those electrons into the mitochondria, cells use **shuttle systems** that transfer electron-carrying potential without transporting NADH itself.

**Malate-aspartate shuttle:** Used by heart, liver, and neurons. Cytoplasmic NADH reduces OAA to malate. Malate enters the matrix via the malate-α-ketoglutarate antiporter. In the matrix, malate is re-oxidized to OAA by malate dehydrogenase, generating mitochondrial NADH. Aspartate leaves the matrix (exchanged for glutamate via the glutamate-aspartate carrier), and transamination in the cytoplasm regenerates OAA (the aspartate aminotransferase reaction transfers the amino group from aspartate to α-ketoglutarate, yielding OAA and glutamate; glutamate then re-enters the matrix to restart the cycle). Net result: one cytoplasmic NADH becomes one mitochondrial NADH. Yield: **2.5 ATP per cytoplasmic NADH.**

**Glycerol-3-phosphate shuttle:** Used by skeletal muscle and brain under some conditions. Cytoplasmic NADH reduces DHAP to glycerol-3-phosphate. A FAD-linked glycerol-3-phosphate dehydrogenase on the outer face of the inner membrane re-oxidizes glycerol-3-phosphate back to DHAP, feeding electrons directly into the CoQ pool as $\text{QH}_2$. Net result: one cytoplasmic NADH enters the ETC as $\text{FADH}_2$ equivalents. Yield: **1.5 ATP per cytoplasmic NADH.**

This is why the total glucose yield is 30 ATP (glycerol-3-phosphate shuttle, 1.5 × 2 = 3 ATP from cytoplasmic NADH) to 32 ATP (malate-aspartate shuttle, 2.5 × 2 = 5 ATP). The difference is 4 ATP, two per cytoplasmic NADH.

If the malate-aspartate shuttle is more efficient, why doesn't every tissue use it? Two reasons. First, the malate-aspartate shuttle is **reversible** and depends on the concentration gradients of its intermediates (malate, aspartate, glutamate, OAA) being maintained in the right direction. Under high glycolytic flux when cytoplasmic NADH is rising rapidly, the shuttle can reverse and actually export reducing equivalents out of the mitochondria, which is counterproductive. The glycerol-3-phosphate shuttle is irreversible: once glycerol-3-phosphate is oxidized by the FAD-linked dehydrogenase on the outer face of the inner membrane, the electrons go into the CoQ pool and cannot come back. For tissues like fast-twitch skeletal muscle that need to sustain very high glycolytic rates and tolerate NADH surges, the irreversibility of the glycerol-3-phosphate shuttle is worth the 1 ATP per NADH penalty. Second, the malate-aspartate shuttle requires active transport of amino acid intermediates across the inner membrane and depends on transaminase activity in both compartments. It is a higher-maintenance system. The glycerol-3-phosphate shuttle requires only two enzymes and no amino acid intermediates, making it simpler and faster to operate under burst conditions.

---

## Uncoupling: When the Gradient Leaks

Normally, the ETC and ATP synthase are **coupled**: electron transport pumps protons, and those protons return only through ATP synthase. Another way to think of it is that if electrons flow through the chain ATP **must** be made and if ATP is being made electrons **must** flow through the chain. Uncoupling breaks this linkage by providing an alternate path for protons to cross the inner membrane, bypassing ATP synthase. When the membrane leaks protons, the gradient energy dissipates as heat instead of ATP.

### Physiological Uncoupling: Brown Adipose Tissue

**Brown adipose tissue (BAT)** is designed to generate heat instead of ATP. It does this via **uncoupling protein 1 (UCP1)**, also known as thermogenin, a proton channel in the inner mitochondrial membrane. When UCP1 is open, protons re-enter the matrix without going through ATP synthase, and the gradient energy is dissipated as heat.

BAT is densely packed with mitochondria, which is what makes it brown: the high mitochondrial density and their cytochromes give it a darker color than white adipose tissue. It is heavily innervated by sympathetic nerve fibers. Cold exposure triggers norepinephrine release, which activates β$_3$-adrenergic receptors on BAT cells, raises cAMP, activates PKA, and stimulates lipolysis (the hydrolysis of stored triacylglycerols to free fatty acids and glycerol, releasing the fatty acids that serve as fuel). Released fatty acids fuel the ETC (keeping the chain running and the gradient loaded) and also allosterically activate UCP1. The result is thermogenesis: heat production without ATP synthesis.

Neonates depend on BAT for non-shivering thermogenesis because they cannot yet shiver. BAT is concentrated around the kidneys, adrenals, and between the shoulder blades in infants. Premature infants with insufficient BAT are particularly vulnerable to cold stress.

In adults, metabolically active BAT is present in the supraclavicular region, along the spine, and around major vessels. It is detectable by PET/CT as warm, metabolically active tissue that concentrates FDG, which is how its presence in adult humans was rediscovered in the 2000s.

### Pharmacological Uncoupling: DNP

**2,4-Dinitrophenol (DNP)** is a small, lipid-soluble weak acid. In the acidic IMS (where $[\text{H}^+]$ is higher), DNP picks up a proton and crosses the inner membrane in its protonated form. In the more alkaline matrix, it releases the proton. It then returns deprotonated and picks up another. The net effect: DNP acts as a proton shuttle, cycling across the membrane and continuously draining the gradient without going through ATP synthase.

DNP was used as a weight loss drug in the United States in the 1930s. Without ATP synthesis, the body burns more fuel to meet its ATP demands, or more precisely, burns fuel just to generate heat. Weight loss was dramatic. Deaths from hyperthermia followed: without any regulatory mechanism (unlike UCP1, which responds to allosteric control), the ETC runs as fast as fuel is supplied, all the energy leaves as heat, and core body temperature can rise without limit. DNP was banned after multiple fatalities.

People continue to obtain DNP online for weight loss, with predictable results. From a biochemical standpoint, DNP deaths are deaths from uncontrolled metabolic overheating. The ETC runs maximally because the PMF is continuously drained, providing no back-pressure on the complexes. All fuel combustion exits as thermal energy. Core temperature can exceed 40°C, and no intervention short of removing the DNP source can stop it.

---

## Regulation

The ETC is not regulated the way the TCA cycle is, with allosteric effectors on specific enzymes. Its regulation is primarily **thermodynamic**: the rate of electron transport is controlled by the availability of substrates (NADH, $\text{FADH}_2$, $\text{O}_2$) and by the magnitude of the PMF acting as back-pressure on the proton-pumping complexes.

When the PMF is high (gradient is built up), it becomes harder to pump more protons against it. The work per proton pumped increases as the gradient grows. Electron transport slows, NADH builds up, and feedback inhibition at the TCA cycle slows everything upstream.

When ATP demand is high (lots of ADP present, PMF is being drained by ATP synthase), the gradient is continuously consumed. The reduced back-pressure allows the complexes to pump faster, electron transport accelerates, NADH is consumed more rapidly, and the TCA cycle is stimulated to replenish NADH. This is **respiratory control**: the rate of the entire pathway is governed by the ATP/ADP ratio, which controls how rapidly the synthase drains the PMF.

The corollary is important for interpreting experiments. If you block ATP synthase with **oligomycin** (an antibiotic that plugs the $\text{F}_0$ proton channel), the PMF rises, electron transport slows, and oxygen consumption drops. If you add an **uncoupler** instead, which drains the PMF, electron transport accelerates, oxygen consumption rises, but no ATP is made. Measuring oxygen consumption in the presence and absence of ADP, oligomycin, and uncouplers is how mitochondrial function is characterized experimentally.

---

## When It Breaks

### Cyanide Poisoning

Cyanide, most commonly as hydrogen cyanide gas (HCN) or soluble salts (NaCN, KCN), is one of the most rapid-acting toxic agents known. Its mechanism is precise: **$\text{CN}^-$ binds to the $\text{Fe}^{3+}$ center of heme a$_3$ in Complex IV, preventing $\text{O}_2$ from binding.**

With the terminal acceptor blocked, electrons cannot leave the chain. The CoQ pool becomes fully reduced, which backs electrons up into Complexes I and II. No proton pumping occurs. The PMF collapses. ATP synthase has no gradient to run on. Cellular ATP falls.

Every cell is affected, but the two most sensitive are neurons (high continuous ATP demand, no glycogen buffer, minimal ability to sustain function glycolytically) and cardiomyocytes (nearly 100% reliant on oxidative phosphorylation, continuous pump requirement). Cyanide produces **histotoxic hypoxia**: tissues cannot use the oxygen delivered to them. Venous blood remains bright red, because hemoglobin never offloads its oxygen to cells that cannot consume it. Pulse oximetry reads normal even as the patient is dying of cellular energy failure. This is a critical clinical point: normal SpO₂ does not rule out cyanide poisoning.

The clinical course is rapid. Initial anxiety and dyspnea give way within minutes to seizures, cardiovascular collapse, and death. Treatment targets cyanide's affinity for iron:

**Sodium nitrite** converts hemoglobin iron from $\text{Fe}^{2+}$ to $\text{Fe}^{3+}$, forming methemoglobin. Methemoglobin's $\text{Fe}^{3+}$ competes with Complex IV's $\text{Fe}^{3+}$ for $\text{CN}^-$, pulling it off the enzyme. The cost: methemoglobin cannot carry oxygen ($\text{Fe}^{3+}$ cannot bind $\text{O}_2$), so the treatment causes a temporary functional anemia. You are trading Complex IV inhibition for reduced oxygen-carrying capacity.

**Sodium thiosulfate** donates a sulfur atom to $\text{CN}^-$ via rhodanese (a mitochondrial enzyme), converting it to thiocyanate ($\text{SCN}^-$), which is excreted in urine. This is slower but permanent.

**Hydroxocobalamin** (Cyanokit) is the preferred modern antidote. Cobalamin (the cobalt-containing core of vitamin B12) binds $\text{CN}^-$ directly with high affinity, forming cyanocobalamin and freeing Complex IV. It has minimal side effects and acts quickly.

### Carbon Monoxide Poisoning

CO binds to hemoglobin approximately 240 times more tightly than oxygen, forming **carboxyhemoglobin (COHb)**. It also causes a left shift in the oxygen-hemoglobin dissociation curve (the Haldane effect), meaning the hemoglobin molecules not blocked by CO also release $\text{O}_2$ less readily to tissues. At typical environmental CO exposures, the dominant toxicity is therefore impaired oxygen delivery: a delivery failure, not a utilization failure.

However, CO also binds to the $\text{Fe}^{2+}$ of heme a$_3$ in Complex IV, causing direct cellular toxicity similar to cyanide. At typical atmospheric CO concentrations, this cellular effect is secondary to the hemoglobin effect. At very high exposures (industrial accidents, enclosed-space fires), both mechanisms may operate simultaneously. This is the relevance of the Opener Question: CO can cause a cellular hypoxia component that oxygen therapy alone does not fully address, particularly in severe poisoning or in highly oxygen-dependent tissues like the heart and brain.

Treatment is **100% oxygen**. At high partial pressure of O₂, hemoglobin binding equilibrium shifts and CO is displaced more rapidly. The half-life of COHb at room air is approximately 5 hours; at normobaric 100% $\text{O}_2$ it falls to 60–90 minutes; in a hyperbaric chamber at 3 atm $\text{O}_2$ it falls to 20–30 minutes. **Hyperbaric oxygen (HBO)** is used for severe poisoning because it accelerates CO removal and, via elevated dissolved plasma $\text{O}_2$, partially compensates for reduced oxygen-carrying capacity while COHb clears.

### Inhibitors of the Chain: A Summary

| Compound | Complex targeted | Mechanism |
|---|---|---|
| Rotenone | Complex I | Blocks CoQ reduction site |
| Metformin (therapeutic) | Complex I | Mild, partial Complex I inhibition |
| Antimycin A | Complex III | Blocks Qi site, prevents CoQ re-reduction |
| Cyanide ($\text{CN}^-$) | Complex IV | Binds $\text{Fe}^{3+}$ of heme a$_3$, blocks $\text{O}_2$ binding |
| Carbon monoxide (CO) | Complex IV | Binds $\text{Fe}^{2+}$ of heme a$_3$, blocks $\text{O}_2$ reduction |
| Azide ($\text{N}_3^-$) | Complex IV | Binds binuclear center |
| Hydrogen sulfide ($\text{H}_2\text{S}$) | Complex IV | Inhibits at high concentrations |
| Oligomycin | ATP synthase ($\text{F}_0$) | Plugs proton channel, blocks $\text{H}^+$ flux |
| DNP, FCCP | Inner membrane | Uncouplers: provide alternate $\text{H}^+$ path, bypass ATP synthase |

When a chain inhibitor is added to respiring mitochondria: electron transport slows or stops, the PMF rises (protons have no outlet), oxygen consumption drops, and ATP production falls. Adding an uncoupler instead produces the opposite: $\text{O}_2$ consumption rises, PMF falls, ATP production falls. The two results look the same at the ATP level but opposite at the oxygen consumption level. This distinction is diagnostically useful in the laboratory.

### Mitochondrial Disease

The mitochondrial genome encodes 13 of the roughly 90 proteins in the respiratory chain (and the rRNAs and tRNAs needed to translate them). The remaining subunits are nuclear-encoded, synthesized in the cytoplasm, and imported. Mutations in either genome can cause mitochondrial disease.

**Mitochondrial inheritance** follows unusual rules. Mitochondria are inherited almost exclusively maternally: sperm contribute little or no mitochondria at fertilization. Mitochondrial DNA mutations are therefore transmitted through the mother. Men with mitochondrial mutations do not pass them to their children.

**Heteroplasmy** makes mitochondrial disease more complicated than most genetic diseases. A cell contains hundreds to thousands of mitochondria, each with multiple mtDNA copies. When a mutation arises in one copy, there is initially a mix of mutant and wild-type genomes in the same cell. The ratio of mutant to wild-type (the heteroplasmy fraction) determines the phenotype: below a threshold, wild-type copies compensate and the cell functions near-normally; above the threshold, dysfunction appears. This threshold effect means that mitochondrial disease severity can vary dramatically between family members carrying the same mutation, and symptoms can appear or worsen unpredictably as heteroplasmy fraction shifts over time.

**MELAS** (Mitochondrial Encephalomyopathy, Lactic Acidosis, and Stroke-like episodes) is most commonly caused by mutations in the mt-tRNA gene for leucine (mt-tRNA: transfer RNA encoded by the mitochondrial genome; transfer RNAs are the adapter molecules that read mRNA codons and deliver the corresponding amino acids during protein synthesis; a defective mitochondrial tRNA for leucine impairs synthesis of all 13 mitochondrially encoded respiratory chain subunits, since leucine appears in each), impairing translation of respiratory chain subunits. The result is combined oxidative phosphorylation deficiency: lactic acidosis (from failed aerobic metabolism and pyruvate backup), episodic neurological events resembling strokes, and myopathy. The lactic acidosis in MELAS reflects the same principle as any severe ETC defect: when NADH cannot be reoxidized, pyruvate backs up and is shunted to lactate. The lactate-to-pyruvate ratio is typically very high (>25), distinguishing it from PDH deficiency where the ratio is only mildly elevated (discussed in Chapter 11 Problem 3).

**Leigh syndrome** is a devastating pediatric mitochondrial encephalopathy caused by defects in Complex I, Complex IV, or the PDH complex, or in their assembly factors. The bilateral symmetric lesions in the basal ganglia and brainstem reflect the selective vulnerability of high-energy-demanding brain regions with limited alternate fuel sources. The ETC-deficiency form of Leigh syndrome is the more common variant; Chapter 11's worked problems used a PDH-deficiency case as the clinical vignette.

---

## The MCAT Angle

**The four complexes and their proton contributions:**

| Complex | Electron donor | $\text{H}^+$ pumped per 2e$^-$ |
|---|---|---|
| I | NADH | 4 |
| II | $\text{FADH}_2$ (succinate) | 0 |
| III | CoQ ($\text{QH}_2$) | 4 |
| IV | Cytochrome c | 2 |

**P/O ratios:** 2.5 per NADH, 1.5 per $\text{FADH}_2$. Know these numbers and where they come from.

**Why $\text{FADH}_2$ yields fewer ATP:** Electrons from $\text{FADH}_2$ enter via Complex II, which pumps no protons. They bypass Complex I entirely. Fewer protons pumped means a smaller gradient contribution, which means fewer ATP synthesized.

**Chemiosmosis:** Free energy from electron transport is stored as a proton electrochemical gradient (the PMF) across the inner mitochondrial membrane. ATP synthase uses the return flow of protons through $\text{F}_0$ to drive conformational changes in $\text{F}_1$ that synthesize ATP. The membrane is the machine.

**Respiratory control:** The ETC rate is governed by ADP availability and the PMF back-pressure. High ADP drains the PMF, which accelerates the chain. High ATP lets the PMF build up, which slows it. This is how ATP demand controls the rate of the entire upstream pathway.

**Inhibitors vs. uncouplers:**
- Chain inhibitors (cyanide, CO, rotenone, antimycin A) and ATP synthase inhibitors (oligomycin) all reduce $\text{O}_2$ consumption and ATP output. The PMF rises when synthase is blocked (protons cannot return), falls when chain is blocked (proton pumping stops).
- Uncouplers (DNP, FCCP) drain the PMF by providing an alternate proton path. $\text{O}_2$ consumption rises (chain runs unchecked), ATP production falls, body temperature rises.

**Histotoxic vs. anemic vs. hypoxic hypoxia:** In cyanide poisoning, $\text{O}_2$ delivery is normal but cells cannot use $\text{O}_2$ (histotoxic hypoxia: a cellular poison blocks $\text{O}_2$ utilization). Venous blood is bright red, pulse oximetry reads normal, but the patient is dying. In CO poisoning, $\text{O}_2$ delivery is impaired because hemoglobin's effective $\text{O}_2$-carrying capacity is reduced (anemic hypoxia: insufficient functional hemoglobin, whether from low total hemoglobin, CO occupation of heme sites, or methemoglobin formation). In altitude-related hypoxia, PO₂ is low so hemoglobin cannot fully load in the lungs (hypoxic hypoxia: inadequate O₂ tension in the alveoli). These are different mechanisms with different diagnostic and treatment implications.

**Mitochondrial inheritance:** Maternal, subject to heteroplasmy, threshold effects explain variable penetrance.

**Shuttles:** Cytoplasmic NADH from glycolysis cannot cross the IMM directly. The malate-aspartate shuttle yields 2.5 ATP per cytoplasmic NADH (heart, liver, neurons); the glycerol-3-phosphate shuttle yields 1.5 ATP (skeletal muscle under some conditions). This is the source of the 30 vs. 32 ATP range for complete glucose oxidation.

---

## Worked Problems

### Problem 1: Respiratory Control in Isolated Mitochondria

A researcher adds isolated mitochondria to a sealed vessel with excess NADH, ADP, and $\text{O}_2$, and monitors oxygen consumption over time. She then adds oligomycin (blocks the $\text{F}_0$ proton channel of ATP synthase). Oxygen consumption drops sharply. The proton gradient rises. ATP production stops. She then adds FCCP, a potent uncoupler.

(a) Explain why oxygen consumption dropped after oligomycin was added.

(b) Why did the proton gradient rise when ATP synthesis was blocked?

(c) After FCCP is added, predict what happens to: oxygen consumption, the proton gradient, and ATP production.

(d) A colleague argues this experiment shows that a chemical intermediate links electron transport to ATP synthesis, not a proton gradient, because blocking the synthase should cause that intermediate to accumulate. Is this interpretation correct? What does the experiment actually demonstrate?

**Solution:**

(a) Oxygen consumption dropped because the electron transport chain slowed. Oligomycin blocks F₀, preventing protons from flowing back through ATP synthase. With no proton outlet, the gradient builds continuously. The rising back-pressure makes it thermodynamically harder for Complexes I, III, and IV to pump more protons against it. Pumping rate slows, electron transport slows in parallel, and $\text{O}_2$ (the terminal acceptor) is consumed more slowly. This is respiratory control: the chain rate is governed by the PMF, which is in turn governed by the rate at which ATP synthase drains the gradient.

(b) The gradient rose because proton pumping continued (at reduced rate) while proton return through ATP synthase was sealed off. Protons are being added to the IMS but none are leaving. The gradient accumulates until back-pressure equilibrates with the maximum pumping capacity, at which point no further net proton translocation occurs.

(c) After FCCP:
- **$\text{O}_2$ consumption rises sharply.** FCCP is a lipid-soluble proton shuttle that collapses the PMF by allowing protons to bypass ATP synthase. With the back-pressure suddenly eliminated, the complexes can pump as fast as they are capable of running. The chain operates at its maximum kinetic rate and consumes oxygen rapidly.
- **Proton gradient falls toward zero.** Protons are pumped out but FCCP immediately returns them to the matrix. The gradient is continuously dissipated.
- **ATP production stays near zero.** The gradient that drives ATP synthase is gone. Oligomycin still blocks the $\text{F}_0$ channel, and even if it did not, there is no PMF to drive synthesis.

(d) The colleague is wrong. This experiment is strong evidence for the chemiosmotic model, not against it. If the linking intermediate were a covalent chemical compound, blocking ATP synthase would cause that compound to accumulate, detectable by chemical assay. Instead, what accumulates is a measurable electrochemical proton gradient across the membrane. Furthermore, an uncoupler drains that gradient specifically by providing a proton pathway, and doing so restores electron transport (at the cost of ATP synthesis). An uncoupler cannot short-circuit a hypothetical covalent intermediate; it can only short-circuit a proton gradient. The experiment shows that the free energy of electron transport is stored as a proton electrochemical gradient, and that ATP synthase is the device that converts that gradient energy into phosphate bond energy.

---

### Problem 2: Cyanide vs. Carbon Monoxide

Both cyanide and carbon monoxide bind to cytochrome c oxidase (Complex IV). Yet the clinical presentations differ:

- In cyanide poisoning, pulse oximetry shows normal SpO₂ but the patient is in cardiovascular collapse.
- In moderate CO poisoning, the patient has low SpO₂ and symptoms of oxygen delivery failure.

(a) Explain the normal SpO₂ in cyanide poisoning. Why is pulse oximetry misleading here?

(b) CO also binds Complex IV. Why is CO poisoning treated primarily as a hemoglobin delivery problem at typical environmental exposures, even though the cellular target is the same?

(c) A patient with severe CO poisoning (COHb 60%) is stabilized on 100% O₂ by non-rebreather mask. A physician asks whether hyperbaric oxygen therapy is warranted. Explain the biochemical rationale for preferring HBO over normobaric 100% O₂ in severe cases.

**Solution:**

(a) Pulse oximetry measures the ratio of oxyhemoglobin to deoxyhemoglobin by comparing their absorption of red and infrared light. In cyanide poisoning, oxygen delivery is entirely normal: the lungs are functioning, hemoglobin is carrying oxygen, and oxygenated blood is arriving at tissues. The problem is that cells cannot extract and use that oxygen, because Complex IV is blocked by $\text{CN}^-$. Cells that cannot run their ETC have no downstream demand for $\text{O}_2$; oxygen stays bound to hemoglobin and returns in venous blood nearly as oxygenated as it arrived. The pulse oximeter reads normal or high SpO₂ because it only measures what is in the blood, not whether cells are using it. This is histotoxic hypoxia: cellular oxygen utilization failure with normal delivery, invisible to a monitor that assesses delivery.

(b) CO's binding affinity for hemoglobin iron is approximately 240 times greater than for oxygen, meaning CO occupies a large fraction of hemoglobin at concentrations that are far below what would be required to substantially inhibit Complex IV (which has its own affinity profile). At typical environmental CO exposures, the hemoglobin effect dominates: reduced $\text{O}_2$-carrying capacity, plus the Haldane-effect left shift that impairs $\text{O}_2$ release from the remaining unblocked hemoglobin. The amount of CO that reaches the mitochondria at these concentrations is below the threshold for significant Complex IV inhibition. At very high CO concentrations (enclosed industrial spaces, severe fire exposure), direct cellular toxicity from Complex IV inhibition may contribute meaningfully, which is why severe CO poisoning has a cellular component that may not fully respond to $\text{O}_2$ alone.

(c) The therapeutic rationale for HBO has two components. First: at 3 atmospheres of 100% $\text{O}_2$, the partial pressure of oxygen in alveoli is approximately 2000 mmHg (vs. 760 mmHg at normobaric 100% $\text{O}_2$), greatly increasing dissolved $\text{O}_2$ in plasma via Henry's law (which states that the amount of a gas dissolved in a liquid is proportional to its partial pressure above the liquid; tripling the $\text{O}_2$ pressure roughly triples the dissolved $\text{O}_2$ in plasma). This dissolved $\text{O}_2$ can supply a significant fraction of tissue $\text{O}_2$ demand independently of hemoglobin, partially compensating for the reduced carrying capacity while COHb clears. Second: the higher PO₂ shifts the hemoglobin/CO equilibrium more strongly toward CO displacement, reducing the COHb half-life from roughly 90 minutes (normobaric 100% $\text{O}_2$) to 20–30 minutes (3 atm HBO). Faster CO removal means faster restoration of hemoglobin function. For severe poisoning with cardiovascular or neurological complications, the combination of faster CO clearance and interim tissue oxygenation via dissolved $\text{O}_2$ improves outcome compared with normobaric 100% $\text{O}_2$ alone.

---

### Problem 3: Fatty Acid Oxidation and the Energy Budget

A person fasting for 48 hours relies primarily on fatty acid oxidation. Consider palmitoyl-CoA, the 16-carbon saturated fatty acid as its CoA thioester (already activated). Complete β-oxidation of palmitoyl-CoA yields 8 acetyl-CoA, 7 NADH, and 7 $\text{FADH}_2$ from the 7 rounds of β-oxidation before any acetyl-CoA is metabolized (β-oxidation, covered fully in Chapter 13, cleaves two carbons at a time as acetyl-CoA; each round also produces one NADH and one FADH₂ from the oxidation steps that shorten the chain; a 16-carbon chain goes through exactly 7 rounds before releasing the final 2-carbon unit as the 8th acetyl-CoA).

(a) How many additional NADH and $\text{FADH}_2$ are generated when all 8 acetyl-CoA pass through the TCA cycle?

(b) Calculate the total ATP yield from complete oxidation of palmitoyl-CoA. Use 2.5 ATP/NADH and 1.5 ATP/$\text{FADH}_2$.

(c) In the liver of this fasting individual, fatty acid oxidation has been active for 48 hours. A large glucose infusion is now given. Using your knowledge of PDH regulation, explain what happens to PDH activity in the liver immediately after the glucose arrives, and which molecular signals mediate it.

(d) Brown adipose tissue in this person was activated by fasting-state sympathetic stimulation. The heart is simultaneously trying to maximize ATP output. Both are running their ETCs hard. What is the difference in the fate of the proton gradient in BAT versus heart?

**Solution:**

(a) Each acetyl-CoA through one full TCA turn yields 3 NADH, 1 $\text{FADH}_2$, and 1 GTP. For 8 acetyl-CoA:
- TCA NADH: 8 × 3 = **24 NADH**
- TCA $\text{FADH}_2$: 8 × 1 = **8 $\text{FADH}_2$**
- Direct GTP: 8 × 1 = **8 GTP** (8 ATP equivalents)

(b) Total NADH: 7 (β-oxidation) + 24 (TCA) = **31 NADH**

Total $\text{FADH}_2$: 7 (β-oxidation) + 8 (TCA) = **15 $\text{FADH}_2$**

Direct GTP/ATP: **8**

ATP from NADH: 31 × 2.5 = 77.5

ATP from $\text{FADH}_2$: 15 × 1.5 = 22.5

Total: 77.5 + 22.5 + 8 = **108 ATP per palmitoyl-CoA**

Note: since palmitoyl-CoA is already the activated thioester, no ATP cost is subtracted. If starting from free palmitate (which requires activation by fatty acyl-CoA synthetase: palmitate + CoA + ATP $\rightarrow$ palmitoyl-CoA + AMP + $\text{PP}_i$, equivalent to 2 ATP equivalents spent), the net yield would be approximately 106 ATP. Some sources tabulate 129 ATP for palmitate using older P/O ratios of 3 and 2; using the current 2.5 and 1.5 gives 108 from palmitoyl-CoA or ~106 from free palmitate. Be consistent with whichever convention your source uses.

Compare with glucose: approximately 30–32 ATP per glucose, from a 6-carbon compound. Palmitate is 16 carbons and yields 108 ATP: roughly 6.8 ATP per carbon, vs. about 5.2 ATP per carbon from glucose. This is why fat is a richer fuel per gram: the carbons in fatty acids are more reduced than those in glucose, carrying more electrons per carbon atom.

(c) When glucose arrives after 48 hours of fatty acid oxidation, glycolysis in the liver generates pyruvate. However, the liver still has elevated mitochondrial NADH and acetyl-CoA from the preceding fatty acid oxidation (these signals do not vanish instantly; the ETC takes time to clear the NADH backlog). PDH kinase (PDK) is activated by both high NADH/$\text{NAD}^+$ ratio and high acetyl-CoA: these are products of the reaction PDH catalyzes, and they signal that there is more than enough of what PDH makes. PDK phosphorylates E1 on the PDH complex, inactivating it. Even though glucose-derived pyruvate is now arriving, the liver suppresses the pyruvate $\rightarrow$ acetyl-CoA step because acetyl-CoA is already abundant. Pyruvate is diverted toward gluconeogenesis via pyruvate carboxylase (which is activated by the same high acetyl-CoA) rather than toward the TCA cycle. Over the following hours, as fatty acid oxidation winds down, NADH and acetyl-CoA fall, PDK activity decreases, insulin rises in response to the glucose load and activates PDH phosphatase (PDP), E1 is dephosphorylated, and PDH activity is restored.

(d) In the **heart**, the proton gradient drives ATP synthase. Protons returning through $\text{F}_0$ rotate the c-ring, driving the conformational changes in $\text{F}_1$ that synthesize ATP. Essentially all of the PMF is converted to phosphate bond energy. The heart is maximizing P/O coupling: for every proton pumped by the ETC, a corresponding fraction becomes ATP.

In **BAT**, UCP1 provides an alternate proton channel in the inner membrane. Protons pumped by the ETC return through UCP1 rather than through ATP synthase, and the energy is released as heat. BAT runs its ETC just as hard as the heart (burning fatty acids, generating a strong PMF), but deliberately routes all the gradient energy to thermogenesis rather than to ATP. This is physiologically controlled uncoupling, regulated by fatty acid allosteric activation of UCP1 and by the norepinephrine signaling cascade. The same electron transport rate that would produce ~36 ATP per glucose equivalent in the heart produces essentially zero ATP net in maximally active BAT: all the free energy exits as heat.

---

## Opener Questions Revisited

**1. Firefighter with potential cyanide and CO exposure. Does 100% oxygen treat both?**

No, and the distinction is clinically critical.

100% oxygen treats CO poisoning by mass action: high PO₂ competes with CO for hemoglobin binding and accelerates its displacement. The half-life of COHb falls from ~5 hours at room air to ~60–90 minutes at normobaric 100% $\text{O}_2$. This directly addresses CO's primary mechanism, which is hemoglobin delivery failure.

Cyanide operates differently. $\text{CN}^-$ binds to Complex IV in every mitochondrion in every cell, preventing $\text{O}_2$ from being used regardless of how much is delivered. Flooding the blood with dissolved $\text{O}_2$ by raising the inspired PO₂ does not reverse a Complex IV block: the enzyme cannot use oxygen if cyanide occupies its active site. Oxygen delivery is not the problem; cellular oxygen utilization is. The treatment requires antidotes that remove $\text{CN}^-$ from Complex IV directly: hydroxocobalamin (which binds $\text{CN}^-$ via its cobalt center), or the sodium nitrite and sodium thiosulfate combination. Simply continuing 100% $\text{O}_2$ while ignoring cyanide toxicity is inadequate.

A firefighter from a fire involving synthetic materials (polyurethane, nylon, wool, acrylonitrile) may have both exposures simultaneously. The treating team should administer both 100% O₂ and cyanide antidote, not one or the other.

**2. ATP synthase inhibitor raises the gradient and drops $\text{O}_2$ consumption. Uncoupler reverses this. What does the experiment demonstrate?**

It demonstrates that electron transport and ATP synthesis are linked through a proton electrochemical gradient, not through a covalent chemical intermediate.

Consider what the results require. Blocking the synthase causes the proton gradient to rise: protons continue being pumped but cannot return, so the gradient builds. If the intermediate were a chemical compound, blocking synthesis would cause that compound to accumulate, not a proton gradient. The gradient also rises, consistent with protons being the intermediate.

Adding FCCP then collapses the gradient by providing an alternate proton path, restoring electron transport (the PMF back-pressure is gone, so the chain runs fast again) while ATP production remains zero. An uncoupler cannot short-circuit a covalent intermediate. It can only short-circuit a proton gradient. The entire sequence, namely gradient accumulation when outlet is blocked, gradient dissipation when alternate proton path is opened, and the precise anti-correlation between $\text{O}_2$ consumption and gradient magnitude, is only consistent with the proton gradient being the linking intermediate. Mitchell was right.

---

*Chapter 13: With the major oxidative pathways in place, we can now look at a parallel route for glucose that solves two problems glycolysis cannot: producing NADPH for biosynthesis and antioxidant defense, and generating ribose-5-phosphate for nucleotide synthesis. The pentose phosphate pathway runs alongside glycolysis in the cytoplasm, and its clinical significance is on display in G6PD deficiency, the most common enzyme deficiency in humans.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*

---

## Problem 1

$\text{FADH}_2$ yields approximately 1.5 $\text{ATP}$ per molecule, while $\text{NADH}$ yields approximately 2.5 $\text{ATP}$. Without simply stating "$\text{FADH}_2$ bypasses Complex I," trace the electron path of each carrier from its oxidation to the final reduction of $\text{O}_2$, and explain mechanistically why the proton yield — and therefore the ATP yield — differs. Your answer should account for which complexes are involved, how many protons each pumps per electron pair, and why the entry point of $\text{FADH}_2$ electrons changes the accounting.

---

## Problem 2

A research group synthesizes a compound called **Qblock** that binds irreversibly to the Qi site of Complex III, identical in action to antimycin A. Isolated mitochondria are supplied with succinate (as the sole electron donor), excess $\text{O}_2$, and $\text{ADP}$. Qblock is then added.

(a) Will the CoQ pool become more oxidized or more reduced after Qblock is added? Explain why.

(b) Predict the effect on cytochrome c reduction state, proton-motive force, and $\text{ATP}$ production.

(c) The researchers add FCCP after Qblock is already present. Predict what happens to oxygen consumption. Does it rise substantially, stay the same, or rise only modestly? Explain your reasoning.

(d) Based on the chapter's discussion of antimycin A and reactive oxygen species, predict whether Qblock would increase ROS production at Complex III. What is the chemical species responsible, and why does the blocked Qi site cause it to form?

---

## Problem 3

The proton-motive force equation is:

$$\Delta p = \Delta V - \frac{2.303 RT}{F} \Delta\text{pH}$$

In a mitochondrial preparation at 37°C, the membrane potential is measured as $-150$ mV (matrix negative relative to IMS) and the pH gradient is 1.0 unit (matrix more basic than IMS).

(a) Calculate the PMF ($\Delta p$) in millivolts. Use $R = 8.314 \text{ J mol}^{-1}\text{K}^{-1}$, $T = 310 \text{ K}$, $F = 96{,}485 \text{ C/mol}$.

(b) Convert the PMF to a free energy value in kJ/mol for the transfer of one mole of protons down this gradient.

(c) Given that the human c-ring contains 8 subunits, and each full rotation synthesizes 3 $\text{ATP}$, how many kJ per mol of $\text{ATP}$ does proton transit provide to the synthase (ignoring transport costs)? Is this sufficient to drive $\text{ATP}$ synthesis, given that $\Delta G^{\circ'}$ for $\text{ATP}$ hydrolysis is approximately $-30.5 \text{ kJ/mol}$?

---

## Problem 4

A 3-year-old is brought to the pediatric neurology clinic with developmental regression, episodic vomiting, and poor feeding. MRI shows bilateral symmetric lesions in the basal ganglia and brainstem. Blood work reveals lactic acidosis with a lactate-to-pyruvate (L:P) ratio of 32. Muscle biopsy respiratory chain enzyme assays show Complex I activity at 8% of normal. Genetic sequencing reveals a heteroplasmic mutation in the mtDNA-encoded ND4 subunit, found in 85% of mitochondria in muscle and 90% in brain.

(a) Why is the L:P ratio elevated in Complex I deficiency? Trace the biochemical logic from Complex I blockade to elevated lactate.

(b) The basal ganglia and brainstem are the most severely affected regions. What property of these tissues makes them selectively vulnerable to ETC defects?

(c) The parents report the child seemed neurologically normal at birth and for the first 18 months of life. The geneticist mentions heteroplasmy and threshold effects. Explain how a child with 90% mutant mtDNA could appear normal at birth and deteriorate later.

(d) The parents have a second, currently healthy child aged 5 with the same mutation at 55% heteroplasmy. The parents ask whether the older child will eventually develop the disease. What is the most scientifically accurate answer you can give, and what concept does it illustrate?

---

## Problem 5

A pharmacologist proposes testing a new lipid-soluble weak acid as a potential anti-obesity agent. In preliminary cell culture experiments, the compound causes:

- $\text{O}_2$ consumption to roughly double
- $\text{ATP}$ levels to fall by approximately 40%
- Mitochondrial membrane potential to collapse
- Cells to release more heat

A colleague immediately raises a safety concern, citing historical precedent.

(a) Identify the mechanism of action of this compound, and name the classical compound it resembles.

(b) What is the biochemical explanation for the doubled $\text{O}_2$ consumption?

(c) Explain why this mechanism cannot be made safe by simply "titrating the dose." In your answer, contrast it with UCP1-mediated uncoupling in brown adipose tissue and explain the key regulatory difference.

(d) From a thermodynamic standpoint, where does the free energy from NADH oxidation go in cells treated with this compound, compared with normally coupled cells?

---

## Problem 6

A cell biologist is studying cytoplasmic NADH handling in two cell types: hepatocytes (liver cells) and fast-twitch skeletal muscle fibers. Both cell types are supplied with excess glucose and are performing glycolysis at high rate.

(a) Which shuttle system is the primary route for cytoplasmic NADH in each cell type? Explain one functional reason why they differ.

(b) In a patient with a mutation that abolishes the matrix isoform of aspartate aminotransferase (GOT2), which shuttle would be non-functional, and why? Which shuttle would the liver be forced to rely on, and what would be the per-glucose ATP cost?

(c) Calculate the ATP yield difference per glucose molecule between a hepatocyte using the malate-aspartate shuttle versus one forced to use the glycerol-3-phosphate shuttle. Show your work.

(d) Under conditions of very high glycolytic flux in skeletal muscle, the glycerol-3-phosphate shuttle is preferred despite its lower yield. What property of this shuttle makes it advantageous under these conditions?

---

## Problem 7

Two isolated mitochondrial preparations are set up side by side:

- **Preparation A** is treated with **oligomycin** (an $\text{F}_0$ proton channel blocker) and then given excess NADH and $\text{O}_2$.
- **Preparation B** is treated with **cyanide** and then given excess NADH and $\text{O}_2$.

(a) In which preparation does $\text{O}_2$ consumption drop more sharply? Explain the mechanism in each case.

(b) In which preparation does the proton-motive force rise? In which does it fall? Explain.

(c) Both preparations produce little or no $\text{ATP}$. A student concludes: "Both experiments prove that ATP synthesis requires electron transport, since blocking either the chain or the synthase abolishes ATP." Evaluate this reasoning. Is the conclusion correct? Is the logic sound?

(d) Now FCCP is added to each preparation simultaneously. Predict the effect on $\text{O}_2$ consumption in each, and explain the difference.

---
---

## References

1. Mitchell P. Coupling of phosphorylation to electron and hydrogen transfer by a chemi-osmotic type of mechanism. Nature. 1961;191:144-148.

2. Mitchell P. Chemiosmotic coupling in oxidative and photosynthetic phosphorylation. Biol Rev Camb Philos Soc. 1966;41:445-502.

3. Boyer PD. The ATP synthase — a splendid molecular machine. Annu Rev Biochem. 1997;66:717-749.

4. Abrahams JP, Leslie AG, Lutter R, Walker JE. Structure at 2.8 Å resolution of F1-ATPase from bovine heart mitochondria. Nature. 1994;370:621-628.

5. Noji H, Yasuda R, Yoshida M, Kinosita K Jr. Direct observation of the rotation of F1-ATPase. Nature. 1997;386:299-302.

6. Stock D, Leslie AG, Walker JE. Molecular architecture of the rotary motor in ATP synthase. Science. 1999;286:1700-1705.

7. Sazanov LA. A giant molecular proton pump: structure and mechanism of respiratory complex I. Nat Rev Mol Cell Biol. 2015;16:375-388.

8. Brandt U. Energy converting NADH:quinone oxidoreductase (complex I). Annu Rev Biochem. 2006;75:69-92.

9. Iwata S, Lee JW, Okada K, et al. Complete structure of the 11-subunit bovine mitochondrial cytochrome bc1 complex. Science. 1998;281:64-71.

10. Tsukihara T, Aoyama H, Yamashita E, et al. The whole structure of the 13-subunit oxidized cytochrome c oxidase at 2.8 Å. Science. 1996;272:1136-1144.

11. Murphy MP. How mitochondria produce reactive oxygen species. Biochem J. 2009;417:1-13.

12. Enerbäck S, Jacobsson A, Simpson EM, et al. Mice lacking mitochondrial uncoupling protein are cold-sensitive but not obese. Nature. 1997;387:90-94.

13. Lowell BB, Spiegelman BM. Towards a molecular understanding of adaptive thermogenesis. Nature. 2000;404:652-660.

14. DiMauro S, Schon EA. Mitochondrial respiratory-chain diseases. N Engl J Med. 2003;348:2656-2668.

15. Weaver LK. Carbon monoxide poisoning. N Engl J Med. 2009;360:1217-1225.
