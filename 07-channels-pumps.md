# Chapter 7: Membrane Channels and Pumps

---

## Opener Questions

Think about these before you read. Come back to them at the end and see if your answer changed.

1. A 19-year-old college athlete collapses during basketball practice. He is resuscitated with a defibrillator. His ECG shows a QT interval of 580 ms (normal is under 440 ms). His older sister died suddenly at age 22. Genetic testing reveals a missense mutation in a gene encoding a voltage-gated potassium channel expressed in cardiac muscle. How does a mutation in a single ion channel protein cause the heart to stop?

2. A 35-year-old woman sees her neurologist for worsening double vision and eyelid drooping. She notices the weakness is worse at the end of the day and improves after sleep. She has no sensory symptoms. Her reflexes are normal. An edrophonium injection dramatically reverses her weakness for several minutes. Her serum contains antibodies against a protein on the postsynaptic membrane of the neuromuscular junction. What is the protein, and why do antibodies against it cause muscle weakness?

---

## The Big Picture

Chapter 6 built the bilayer: a two-dimensional fluid of amphipathic lipids that separates inside from outside. The bilayer does exactly one thing well. It is an excellent barrier. Small nonpolar molecules, gases, steroid hormones, pass through it freely. Charged molecules, large polar molecules, essentially all ions do not. A lipid bilayer is nearly impermeable to sodium, potassium, calcium, and chloride ions, which means it can maintain large concentration differences for these species across its surface.

That barrier function is essential. But a barrier alone is not enough to run a cell.

Consider what you actually need from a membrane: you need to import nutrients, export waste, send and receive signals, generate electrical impulses in neurons, pump calcium out of the cytoplasm to reset signaling cascades, expel sodium to maintain cell volume, and convert the energy stored in ion gradients into mechanical work and chemical synthesis. None of those things can happen across a pure lipid barrier. They all require protein machinery embedded in that barrier.

This chapter is about that machinery. The two major classes are **channels**, which provide a protein-lined aqueous pore through which specific ions or molecules can diffuse down their electrochemical gradient, and **pumps** (also called active transporters), which use energy to move ions or molecules against their electrochemical gradient. Channels are passive. Pumps are active. The combination of the two creates and uses the ion gradients that are the energy currency of the nervous system, the heart, and virtually every epithelial cell in the body.

The two clinical anchors are long QT syndrome and myasthenia gravis. Long QT syndrome is a failure of a voltage-gated potassium channel in cardiac muscle that causes the heart's electrical cycle to run too long, destabilizing the rhythm and precipitating fatal arrhythmia. Myasthenia gravis is an autoimmune attack on a ligand-gated ion channel at the neuromuscular junction that reduces the signal reaching the muscle. Together, they illustrate how a single molecular defect at the membrane level cascades into catastrophic physiology. The mechanism is the point. By the end of this chapter, you will be able to explain both cases from the atomic structure of the channel to the cardiac monitor and the examination room.

---

## Why the Bilayer Is a Barrier to Ions

The lipid bilayer has a hydrophobic core approximately 30 Angstroms thick. Moving a charged ion from aqueous solution into that hydrophobic core carries a very large thermodynamic cost.

In water, ions are surrounded by shells of oriented water molecules. A sodium ion in aqueous solution carries six water molecules in its first coordination shell. These water molecules stabilize the charge by electrostatic interaction. The free energy of this hydration is large and negative: it is why ionic compounds dissolve in water at all. Moving the sodium ion from water into the hydrophobic core of the bilayer would require stripping those water molecules away, which costs roughly 150 kJ/mol for sodium. This is the **Born energy** of transfer, the cost of moving a charge from a high-dielectric environment (water, $\varepsilon \approx 80$) to a low-dielectric environment (hydrocarbon, $\varepsilon \approx 2$). The higher the charge and the smaller the ionic radius, the greater the penalty.

The practical consequence is that the bare lipid bilayer is essentially impermeable to ions. The measured permeability of a pure phospholipid bilayer to potassium ions is on the order of $10^{-14}$ cm/s. Real biological membranes have measured potassium permeabilities many orders of magnitude higher, entirely because of ion channels. The channels solve the Born energy problem by providing a protein-lined aqueous pore: the ion moves through water the entire way, never actually contacting the hydrophobic core.

This is not a minor technical point. It is the foundation of all electrical signaling in biology. The impermeable bilayer lets the cell build up large concentration differences across the membrane; the selective, regulated pores of channels let the cell discharge those differences rapidly and in a controlled fashion.

---

## Electrochemical Gradients

### Two Forces, One Ion

An ion in solution experiences two driving forces simultaneously. The first is the **chemical gradient**: the tendency to diffuse from high concentration to low concentration, driven by the increase in entropy upon mixing. The second is the **electrical gradient**: the force exerted on a charged particle by the electric field across the membrane, quantified by the membrane potential $V_m$ (which we will explore shortly). An ion moves in the direction that makes both forces happy, or it sits still when the two forces exactly balance.

The combined driving force is the **electrochemical gradient**, the relevant quantity for predicting which way an ion moves through an open channel:

$$\Delta G = RT\ln(\frac{c_f}{c_i}) + ZF\Delta V$$

Where R is the universal gas constant ($0.0083145 \frac{\text{kJ}}{\text{mol} \cdot \text{K}}$), T is temperature in Kelvin, F is Faraday's constant ($96.5 \frac{\text{kJ}}{\text{mol} \cdot \text{V}}$), and Z is the charge number (valence) of the ion (+1 for $\text{Na}^+$, +2 for $\text{Ca}^{2+}$, $-1$ for $\text{Cl}^-$).

$\Delta V$ is often confused with $V_m$. The membrane potential is defined as $V_m = V_{in} - V_{out}$: inside minus outside, always. The absolute reference voltage is arbitrary; only the difference matters. By convention we set $V_{out} = 0$, so $V_m = -60\;\text{mV}$ simply means $V_{in} = -60\;\text{mV}$. $\Delta V$ in the equation above is $V_f - V_i$: the potential at the destination minus the potential at the origin, so its sign depends on the direction of ion movement across the membrane.

### The Nernst Equation and Equilibrium Potential

Where does this membrane potential, $V_m$ come from then? Consider a container divided in 2. On the left is an equimolar 1M mixture of hypothetical ions $X^+$ and $X^-$; on the right is an equimolar 0.1M mixture of the same two ions. Because each side carries equal positive and negative charge, the electrical potential is 0 on both sides: $\Delta V = 0$ and the $ZF\Delta V$ term vanishes. Now imagine the divider becomes selectively permeable to $X^-$ but not $X^+$. The concentration of $X^-$ is higher on the left, so $X^-$ diffuses right, driven entirely by the $RT\ln(\frac{c_f}{c_i})$ term.

Here's the catch: as $[X^-]$ increases in the right chamber, the right side develops a net negative charge. This growing electrical potential opposes further $X^-$ entry, since negative charge repels negative charge. The system reaches equilibrium when the diffusion tendency driving $X^-$ rightward is exactly balanced by the electrical repulsion from the accumulated negative charge. At this equilibrium, by definition, $\Delta G = 0$

$$0 = RTln(\frac{c_f}{c_i}) + ZF\Delta V$$

Solving for $\Delta V$ gives us

$$\Delta V = -\frac{RT}{ZF}\ln(\frac{c_f}{c_i})$$

A slight rearrangement and generalization of this equation produces the **Nernst equation**

$$V_{eq} = \frac{RT}{zF}\ln\frac{[ion]_{out}}{[ion]_{in}}$$

In plain English: $V_{eq}$ is the membrane voltage at which an ion with a given concentration difference across the membrane would feel zero net force. If the actual membrane potential equals $V_{eq}$ for that ion, the electrical gradient exactly cancels the concentration gradient and there is no net ion flow even through an open channel. If the actual membrane potential differs from $V_{eq}$, the difference between the two is the net driving force on that ion.

$V_{eq}$ is also written $E_{ion}$ in most texts; both refer to the equilibrium potential for a given ion. At $37^\circ C$, $\frac{RT}{F} \approx 26.7$ mV, and for a monovalent ion this simplifies to approximately:

$$E_{ion} \approx 61.5\;\text{mV} \times \log_{10}\frac{[ion]_{out}}{[ion]_{in}}$$

The switch from $\ln$ to $\log_{10}$ is purely practical: the conversion factor $\ln(10) \approx 2.303$ is folded into the prefactor ($26.7 \times 2.303 \approx 61.5$ mV), and base-10 logs are far easier to estimate quickly. A 10-fold concentration ratio gives exactly 61.5 mV; a 100-fold ratio gives 123 mV. Biological concentration gradients are often round powers of ten, so this form is the one you will actually use at the bedside or on an exam.

For potassium, the typical concentrations are approximately 5 mM outside the cell and 140 mM inside. Plugging in:

$$E_K \approx 61.5\;\text{mV} \times \log_{10}\frac{5}{140} \approx 61.5\;\text{mV} \times (-1.45) \approx -90\;\text{mV}$$

For sodium, the concentrations are approximately 145 mM outside and 12 mM inside:

$$E_{Na} \approx 61.5\;\text{mV} \times \log_{10}\frac{145}{12} \approx +66\;\text{mV}$$

These numbers define the equilibrium positions for each ion. The resting membrane potential of a typical neuron is approximately $-70$ mV. Since $-70$ mV is more positive than $E_K$ ($-90$ mV), there is a net driving force pushing potassium out of the cell. Since $-70$ mV is much more negative than $E_{Na}$ ($+66$ mV), there is a massive driving force pushing sodium into the cell. Sodium is being kept outside by the impermeability of the resting membrane, not by thermodynamic equilibrium. The sodium gradient is a loaded spring.

### Resting Membrane Potential

The resting membrane potential in neurons is approximately $-70$ mV (inside negative). It arises because the resting membrane is selectively permeable to potassium. Potassium leak channels (KCNK family) are open at rest and provide a constant background conductance. Potassium diffuses out down its concentration gradient, carrying positive charge out and leaving behind negatively charged intracellular proteins and phosphate groups that cannot cross the membrane. The departure of positive charge builds up a negative inside potential that increasingly opposes further potassium exit. The resting potential is close to but not exactly $E_K$ because there is a small resting permeability to sodium and chloride as well, which shifts the resting potential slightly toward their respective equilibrium potentials.

The **Goldman equation** (not required for this course but worth knowing exists) gives the membrane potential when multiple ion species are simultaneously permeable, weighting each ion's Nernst potential by its relative permeability. In other words, the membrane potential is a weighted average of the equilibrium potentials of all permeable ions, with the most permeable ion contributing most.

The resting potential is not a passive equilibrium; it is a steady state maintained by active pumping. Specifically, the $\text{Na}^+/\text{K}^+$ ATPase continuously extrudes sodium and imports potassium against their gradients. Without the pump, the gradients would run down. The pump is covered in detail in the active transport section below.

---

## Ion Channels

An ion channel is a transmembrane protein that forms an aqueous pore through the membrane. When the channel is open, ions that are electrochemically favored to cross the membrane do so by diffusion through the pore. In other words ion channels facilitate thermodynamically downhill movement ($\Delta G < 0$) of ions across a membrane, a process knowon as **passive transport**. Channels are also remarkably fast: a single open channel passes $10^6$ to $10^8$ ions per second, close to the diffusion limit. This is orders of magnitude faster than any pump or carrier.

### Selectivity

Ion channels are selective: most allow only a specific ion or class of ions to pass. The potassium channel passes potassium but not sodium, despite the fact that sodium is smaller and, one might naively expect, should fit more easily through any given pore. The molecular mechanism of selectivity was resolved by Roderick MacKinnon, who solved the crystal structure of the KcsA potassium channel and received the Nobel Prize in Chemistry in 2003 for his work.

The key is the **selectivity filter**: a narrow constriction in the pore formed by a highly conserved sequence (the signature sequence TVGYG in potassium channels) whose backbone carbonyl oxygens are precisely positioned to coordinate a potassium ion. In solution, potassium carries a hydration shell of coordinated water molecules; passing through the selectivity filter requires shedding that shell, which costs energy. The backbone carbonyl oxygens of the filter are geometrically optimized for potassium's ionic radius (1.33 Angstroms) and substitute for the water molecules one-for-one, providing coordination energy that nearly offsets the cost of dehydration. The net energy barrier is close to zero, and potassium passes through freely. Sodium has a smaller radius (0.95 Angstroms) and cannot be properly coordinated by the potassium-sized filter after attempting to shed its hydration shell: the Born energy cost of dehydrating sodium without adequate compensation from the protein oxygens is prohibitive, so sodium is effectively excluded.

This is a beautiful example of a principle that will recur throughout this course: molecular geometry at the atomic scale determines selectivity and specificity. The potassium channel does not actively exclude sodium; it simply does not coordinate it well enough to compensate for dehydration.

### Gating

Channels are not always open, that would be disastrous. **Gating** refers to the transition between open and closed states of the channel. The stimulus that triggers this transition defines the channel type.

**Voltage-gated channels** open in response to changes in membrane potential. They have a transmembrane voltage-sensing domain, classically the S4 helix as in the voltage-gated $\text{K}^+$ channel, which contains several positively charged arginine or lysine residues spaced every three positions. Because these charges are embedded in the transmembrane helix, the electric field across the membrane exerts a force on them. When the membrane depolarizes (becomes less negative inside), the outward electric force on the positively charged S4 helix causes it to move outward, triggering a conformational change that opens the pore. Voltage-gated sodium channels ($\text{Na}_\text{V}$), voltage-gated potassium channels ($\text{K}_\text{V}$), and voltage-gated calcium channels ($\text{Ca}_\text{V}$) are all built on this basic architecture and are the essential machinery of the action potential.

Voltage-gated sodium channels have an additional feature: **inactivation**. After opening in response to depolarization, they close again within milliseconds even if the membrane remains depolarized. This is distinct from DE-activation (closing when the voltage returns to resting). The structural mechanism is the **ball-and-chain model**: a cluster of hydrophobic residues on the cytoplasmic N-terminus (the "ball") swings into the open pore and physically plugs it after a short delay. Inactivation is the reason the action potential is a brief, unidirectional event rather than a sustained depolarization.

**Ligand-gated channels** (also called ionotropic receptors) open when a specific ligand binds. The ligand binding site and the channel pore are parts of the same protein or protein complex; ligand binding directly changes the protein conformation to open the pore. The nicotinic acetylcholine receptor at the neuromuscular junction is the canonical example: two acetylcholine molecules bind to the extracellular domain on the post-synaptic neuron and cause a conformational change that opens a nonselective cation channel, allowing $\text{Na}^+$ (primarily) and $\text{K}^+$ to flow, depolarizing the muscle membrane. $\text{GABA}_A$ receptors and glycine receptors are ligand-gated chloride channels; their opening hyperpolarizes or stabilizes the membrane potential, producing inhibition rather than excitation. Glutamate receptors (AMPA, NMDA, kainate) are ligand-gated cation channels and are the primary mediators of excitatory synaptic transmission in the CNS.

**Mechanically gated channels** open in response to physical deformation of the membrane. They are found in hair cells of the cochlea (where sound-induced vibration deflects stereocilia and opens channels to produce hearing), in proprioceptors, and in the touch receptors of the skin. Their molecular mechanism involves the channel being physically tethered to the cytoskeleton or to the extracellular matrix such that membrane stretch directly pulls the channel open.

### Single-Channel Physiology: Patch Clamp

Individual ion channels can be recorded electrically using the **patch clamp** technique, developed by Erwin Neher and Bert Sakmann (Nobel Prize in Physiology or Medicine, 1991). A fire-polished glass pipette with a tip diameter of roughly 1 micron is pressed against the membrane and a gigaohm seal forms between the glass and the membrane. The pipette can be configured to record from a single channel in the membrane patch. A single open potassium channel passes a current of approximately 2 to 4 picoamperes. Channels gate stochastically between defined open and closed states, with the probability of being open ($P_o$) dependent on the stimulus (voltage, ligand, or mechanical force). Patch clamp recording shows that channels do not have graded conductance states: they are either fully open or fully closed, with rapid transitions between the two. The stochastic gating of individual channels averages out when thousands of channels are open simultaneously in a whole cell, producing the smooth, graded currents seen in whole-cell recordings.

---

## Ion Pumps and Membrane Transporters

Channels provide downhill pathways for ion movement. But the electrochemical gradients that drive channel-mediated flow must be established and maintained by **active transport**: moving ions uphill against their electrochemical gradients. This requires energy input.

### The $\text{Na}^+/\text{K}^+$ ATPase

The ${\text{Na}^+/\text{K}^+}$ ATPase is the primary pump responsible for maintaining the sodium and potassium gradients across animal cell plasma membranes. It is also called the sodium-potassium pump. It uses the energy of ATP hydrolysis to move three sodium ions out of the cell and two potassium ions into the cell per cycle, against the electrochemical gradients for both ions. The stoichiometry is electrogenic: three positive charges leave, two return, so each cycle produces a net outward movement of one positive charge. This makes a small direct contribution to the resting membrane potential, but the dominant effect is indirect: by maintaining the $Na^+$ and $K^+$ gradients, the pump sustains the electrochemical driving forces that the channels use.

The mechanism follows an alternating-access model:

1. In the **E1** conformation, three cytoplasmic sodium-binding sites face inward and have high affinity for $\text{Na}^+$.
2. Three $\text{Na}^+$ ions bind from the cytoplasm.
3. ATP is hydrolyzed; the gamma-phosphate is transferred to an aspartate residue on the pump, forming a phosphorylated intermediate (E1-P). *Note: The phosphoryl-aspartate that is formed in this step is where the P in P-type ATPase gets its name*
4. Phosphorylation drives the conformational change to the **E2** state, which exposes the three sodium sites to the extracellular space and simultaneously reduces their affinity for $\text{Na}^+$. Sodium dissociates to the outside.
5. In the E2 conformation, two extracellular potassium-binding sites have high affinity for $\text{K}^+$.
6. Two $\text{K}^+$ ions bind from the extracellular space.
7. $\text{K}^+$ binding stimulates hydrolysis of the aspartyl-phosphate bond, returning the pump to the E1 conformation with the two potassium sites now facing inward and having reduced affinity for $\text{K}^+$.
8. $\text{K}^+$ dissociates into the cytoplasm and the cycle repeats.
9. The pump, now empty and in the E1 conformation begins the cycle again at step 1.

The energy expenditure is significant: the $\text{Na}^+/\text{K}^+$ ATPase accounts for roughly 20 to 30% of total resting ATP consumption in most cells and up to 70% in neurons. In terms of energy, each complete cycle consumes one ATP molecule (approximately 50 kJ/mol under cellular conditions) and moves a net charge against a combined electrochemical gradient. The energy is worthwhile: the sodium gradient created is subsequently used to drive secondary active transport of glucose, amino acids, and other nutrients, to extrude calcium through the $\text{Na}^+/\text{Ca}^{2+}$ exchanger, and to power electrical signaling.

The $\text{Na}^+/\text{K}^+$ ATPase is a P-type ATPase: it forms a phosphorylated intermediate during each cycle. Other clinically important P-type ATPases include the sarcoplasmic/endoplasmic reticulum $\text{Ca}^{2+}$ ATPase (SERCA), which pumps calcium from the cytoplasm back into the ER/SR following a calcium signal, and the gastric $H^+/\text{K}^+$ ATPase, which pumps protons into the stomach to achieve the low pH needed for pepsin activity (proton pump inhibitors like omeprazole irreversibly inhibit this enzyme and are among the most prescribed drugs in the world).

**Cardiac glycosides** (digoxin, ouabain) inhibit the $\text{Na}^+/\text{K}^+$ ATPase by binding to its extracellular face in the E2-P state. Inhibiting the pump raises intracellular $\text{Na}^+$, which secondarily reduces the activity of the $\text{Na}^+/\text{Ca}^{2+}$ exchanger (which normally extrudes calcium using the inward sodium gradient), leading to a rise in intracellular $\text{Ca}^{2+}$ and increased force of cardiac contraction. Digoxin, derived from the foxglove plant, has been used for centuries to treat heart failure and certain arrhythmias.

### Secondary Active Transport

Because the sodium gradient is a store of free energy (sodium sitting outside a cell is like a compressed spring held shut by the membrane), cells can harness that gradient to drive the uphill transport of other molecules. This is **secondary active transport**: using the free energy stored in one gradient to move another molecule against its own gradient.

A **symporter** (cotransporter) moves two species in the same direction: For example sodium down its gradient and the passenger molecule up its gradient simultaneously. The canonical example is the **sodium-glucose cotransporter** (SGLT1) in intestinal epithelial cells, which imports glucose from the intestinal lumen into the enterocyte by coupling its transport to the inward flow of two sodium ions. The free energy released by moving 2 $\text{Na}^+$ down the electrochemical gradient is sufficient to drive glucose import against a concentration gradient, allowing complete absorption of dietary glucose even when luminal glucose concentrations are low.

An **antiporter** moves two species in opposite directions. The $\text{Na}^+$/$\text{Ca}^{2+}$ exchanger (NCX) extrudes one calcium ion in exchange for three sodium ions flowing inward. The large inward driving force on sodium drives calcium extrusion against a steep concentration gradient (cytoplasmic $\text{Ca}^{2+}$ is maintained at roughly 100 nM at rest versus roughly 1 mM extracellular).

A **uniporter** moves a single molecule down its concentration gradient via a protein-facilitated mechanism, with no coupling to ion flow. The GLUT family of glucose transporters in most tissues (other than intestine) are uniporters: they facilitate glucose entry into cells by simple facilitated diffusion, driven by the glucose concentration gradient. Note that uniporters are mechanistically different from channels. A channel is essentially a hole in the membrane (with a selectivity filter and gating, but a hole nonetheless): ions flow through without the protein changing shape. A uniporter is a carrier protein; moving a molecule across requires a conformational change in the transporter itself. This means uniporters follow saturation kinetics, with defined $K_m$ and $k_{\text{cat}}$ values, and can be saturated at high substrate concentrations. They are consequently much slower than channels, but saturation also means their transport rate is concentration-sensitive in a predictable, regulatable way.

---

## The Action Potential

An action potential is a transient, self-propagating reversal of the membrane potential in a neuron (or other electrically excitable cell). It is the fundamental unit of information transmission in the nervous system: the event by which a signal is encoded, transmitted along an axon, and ultimately delivered to a synapse.


### Resting State

At rest, the membrane potential of a neuron is approximately $-70$ mV. Voltage-gated sodium channels are closed. Potassium leak channels are open. The $\text{Na}^+$/$\text{K}^+$ ATPase is running continuously to maintain the sodium and potassium gradients.

### Initiation: Reaching Threshold

A depolarizing stimulus (a synaptic input or a sensory stimulus) raises the membrane potential toward a **threshold**, typically around $-55$ mV. Below threshold, the depolarization is subthreshold and will decay without producing an action potential (this decay is called an electrotonic potential or graded potential). At threshold, enough voltage-gated $\text{Na}^+$ channels open to initiate a regenerative cycle.

### Phase 1: Depolarization

Above threshold, the opening of voltage-gated $\text{Na}^+$ channels initiates a positive feedback loop. Depolarization opens some $\text{Na}^+$ channels; $\text{Na}^+$ flows in (driven by an enormous electrochemical gradient: the chemical gradient pushes $\text{Na}^+$ in, and the interior negativity attracts $\text{Na}^+$). $\text{Na}^+$ entry further depolarizes the membrane, which opens more $\text{Na}^+$ channels, which causes more $\text{Na}^+$ entry. This is a runaway regenerative process: the action potential fires in an all-or-nothing fashion. The membrane potential races toward the $\text{Na}^+$ equilibrium potential ($+66$ mV) but never quite reaches it because two processes begin to terminate depolarization.

### Phase 2: Repolarization

Two simultaneous events terminate the depolarization and restore the membrane to negative values.

First, voltage-gated $\text{Na}^+$ channels **inactivate**. The ball-and-chain inactivation described above closes the $\text{Na}^+$ channel from the cytoplasmic side within 1 to 2 milliseconds of opening, even though the membrane is still depolarized. Inactivated channels cannot reopen until the membrane is repolarized and the channels return to the closed (deactivated) state: this is why a second action potential cannot be initiated during the inactivation period.

Second, voltage-gated $\text{K}^+$ channels open. These channels are slower than $\text{Na}^+$ channels: they open in response to depolarization, but with a delay of a few milliseconds. When they open, $\text{K}^+$ flows out of the cell (down its electrochemical gradient: the membrane is depolarized, closer to 0 mV, while $E_K$ is $-90$ mV, so there is a large outward driving force). Outward movement of positive charge repolarizes the membrane.

### Phase 3: Afterhyperpolarization and Refractory Period

The voltage-gated $\text{K}^+$ channels close slowly. For a brief period, the membrane potential overshoots past the resting potential and transiently hyperpolarizes toward $E_K$ ($-90$ mV). This is the **afterhyperpolarization**.

During and around the action potential, the neuron passes through two refractory periods.

The **absolute refractory period** lasts while $\text{Na}^+$ channels are in the inactivated state (typically 1 to 2 ms after the peak). During this period, no stimulus of any strength can trigger another action potential, because the $\text{Na}^+$ channels needed to generate one are unavailable. The absolute refractory period sets an upper limit on firing frequency: a neuron firing at maximum frequency cannot exceed roughly 500 to 1000 action potentials per second.

The **relative refractory period** follows immediately after: $\text{Na}^+$ channels are recovering from inactivation, but $\text{K}^+$ channels are still partially open and the membrane is hyperpolarized. An action potential can be triggered during this period, but only by a stronger-than-normal stimulus, because the starting potential is more negative. The relative refractory period lasts several milliseconds.

The refractory periods also ensure **directionality** of propagation. When an action potential propagates along an axon, the membrane just behind the active zone (in the direction the impulse came from) is in the absolute refractory period. Only the membrane ahead of the action potential can fire next. This is why action potentials travel in one direction along an axon rather than spreading backward.

### Propagation

An action potential at one location on the axon depolarizes adjacent membrane through electrotonic spread of current. This brings the adjacent membrane to threshold, triggering an action potential there. The local circuit flows in a wave along the axon. In unmyelinated axons, propagation is slow because every patch of membrane must be sequentially depolarized.

**Myelination** dramatically increases propagation velocity. Myelin is a lipid-rich wrapping provided by Schwann cells (peripheral nervous system) or oligodendrocytes (central nervous system) that electrically insulates the axon. Myelinated axons have $\text{Na}^+$ channels concentrated at the **nodes of Ranvier**: small gaps in the myelin sheath spaced approximately 1 mm apart. The action potential jumps from one node to the next (**saltatory conduction**), because current can flow rapidly through the insulated internodal segments without depolarizing the axonal membrane there. Saltatory conduction in a large myelinated axon can achieve velocities of up to 100 m/s, compared to 0.5 to 2 m/s in unmyelinated fibers of similar diameter. Multiple sclerosis is a demyelinating disease in which autoimmune destruction of oligodendrocytes disrupts saltatory conduction, slowing or blocking action potential propagation and producing the variety of neurological deficits characteristic of the disease.

---

## Synaptic Transmission

An action potential arriving at a nerve terminal must cross the **synapse** to communicate its signal to the next cell, whether another neuron or a muscle fiber. The synapse is a gap of roughly 20 to 40 nm between the presynaptic terminal and the postsynaptic membrane. The signal crosses this gap chemically, via **neurotransmitters**: small molecules released from the presynaptic terminal that diffuse across the cleft and bind to receptors on the postsynaptic cell.

### Presynaptic Release: Calcium-Triggered Exocytosis

Neurotransmitters are stored in **synaptic vesicles** that are clustered near the presynaptic membrane at specialized release sites called active zones. When an action potential arrives at the terminal:

1. Depolarization opens voltage-gated $\text{Ca}^{2+}$ channels ($\text{Ca}_\text{V}$2.1, $\text{Ca}_\text{V}$2.2) in the presynaptic membrane.
2. $\text{Ca}^{2+}$ flows in from the extracellular space (extracellular $\text{Ca}^{2+}$ is approximately 2 mM; cytoplasmic $\text{Ca}^{2+}$ at rest is roughly 100 nM, a 20,000-fold gradient).
3. The local rise in $\text{Ca}^{2+}$ is sensed by **synaptotagmin**, a $\text{Ca}^{2+}$-binding protein on the synaptic vesicle.
4. Synaptotagmin interacts with the SNARE complex (synaptobrevin on the vesicle with syntaxin and SNAP-25 on the target membrane), which catalyzes vesicle fusion with the presynaptic membrane.
5. Fusion releases neurotransmitter into the synaptic cleft by exocytosis.

The entire sequence from action potential arrival to neurotransmitter release takes less than 1 millisecond. The $\text{Ca}^{2+}$ trigger is essential: blocking voltage-gated $\text{Ca}^{2+}$ channels or chelating $\text{Ca}^{2+}$ in the presynaptic terminal abolishes neurotransmitter release. Botulinum toxin cleaves SNARE proteins (different toxin serotypes cleave synaptobrevin, syntaxin, or SNAP-25) and thereby blocks vesicle fusion and neurotransmitter release at neuromuscular junctions, producing the flaccid paralysis of botulism. The same mechanism underlies the cosmetic use of botulinum toxin (Botox): injecting a dilute, precisely localized dose into a muscle blocks ACh release at that neuromuscular junction, preventing contraction and relaxing the overlying skin. The effect is temporary because axon terminals sprout new branches over weeks to months, restoring neuromuscular transmission as the old terminals regenerate their SNARE machinery.

### Postsynaptic Receptors: Ionotropic vs. Metabotropic

Neurotransmitters act on two classes of postsynaptic receptor that differ fundamentally in their mechanism and kinetics.

**Ionotropic receptors** are ligand-gated ion channels: the receptor and the channel are the same protein. Neurotransmitter binding directly opens the channel, producing a fast (millisecond timescale) change in membrane conductance. Examples: nicotinic acetylcholine receptors (cation channels, excitatory at the neuromuscular junction and in ganglia, and what I described in the summary above), $\text{GABA}_\text{A}$ receptors ($\text{Cl}^{-}$ channels, inhibitory), glycine receptors ($\text{Cl}^{-}$ channels, inhibitory in the spinal cord), AMPA receptors and NMDA receptors (both glutamate-gated cation channels, excitatory in the CNS). **Ionotropic signaling is the mechanism of fast synaptic transmission**.

**Metabotropic receptors** are G protein-coupled receptors (GPCRs, which we will cover more in the next chapter): the receptor and the channel (or other effector) are separate proteins. Neurotransmitter binding activates a G protein, which modulates effectors downstream, including ion channels that are regulated indirectly (via phosphorylation or via direct $\text{G}_{\beta\gamma}$ subunit interaction). The onset is slower (tens of milliseconds to seconds) *however* the effect can be amplified (one receptor activating many G protein molecules). Metabotropic receptors mediate neuromodulation: they tune neuronal excitability and synaptic strength rather than providing point-to-point fast transmission. Examples: muscarinic acetylcholine receptors, metabotropic glutamate receptors (mGluRs), $\text{GABA}_\text{B}$ receptors. G protein signaling is covered in detail in the cell signaling chapter.

### The Neuromuscular Junction

The neuromuscular junction (NMJ) is the synapse between a motor neuron and a skeletal muscle fiber. It is the best-characterized synapse in biology and the clinical target of myasthenia gravis.

The presynaptic terminal of the motor neuron releases **acetylcholine (ACh)** from synaptic vesicles when an action potential arrives. ACh diffuses across the synaptic cleft and binds to **nicotinic acetylcholine receptors (nAChRs)** on the motor endplate of the muscle fiber.

The nicotinic AChR is a pentameric ligand-gated ion channel: five subunits ($\alpha_2\beta\gamma\delta$ at the fetal or denervated NMJ; $\alpha_2\beta\varepsilon\delta$ at the adult NMJ) arranged symmetrically around a central pore. Two ACh molecules must bind simultaneously, one to each of the two alpha subunits, to open the channel. When both sites are occupied, the channel opens within microseconds and allows $\text{Na}^+$, $\text{K}^+$, and small amounts of $\text{Ca}^{2+}$ to flow. The net effect is a large inward $\text{Na}^+$ current that depolarizes the motor endplate: this is the **endplate potential (EPP)**. If the EPP is large enough to bring the adjacent muscle membrane to threshold, voltage-gated $\text{Na}^+$ channels in the muscle fire an action potential, calcium is released from the sarcoplasmic reticulum via RyR1, and the muscle contracts. Signal terminated: the enzyme **acetylcholinesterase** in the basal lamina of the NMJ rapidly hydrolyzes ACh to choline and acetate, clearing the cleft and allowing the nAChR to return to the closed state. Choline is taken up by the presynaptic terminal and resynthesized into ACh by choline acetyltransferase.

This is the exact pathway targeted by organophosphate nerve agents (Chapter 4): they inhibit acetylcholinesterase, causing ACh to accumulate at every cholinergic synapse, producing continuous depolarization and the cholinergic crisis described in that chapter's opener.

### Putting It All Together

1. The membrane is at rest, with a membrane potential of approximately $-60$ mV.
2. In the presynaptic neuron, when an action potential reaches the synapse, ACh-containing vesicles fuse to the membrane and release ACh into the synaptic cleft.
3. ACh in the synaptic cleft binds to the nAChR, a non-selective cation channel. This allows sodium to enter the cell and potassium to exit.
4. Because the membrane is now equally permeable to both sodium and potassium, the membrane potential is governed by their equilibrium potentials as described by the Goldman equation: $E_{\text{Na}} \approx +60\;\text{mV}$ and $E_{\text{K}} \approx -90\;\text{mV}$. The membrane potential therefore approaches the average of the two, roughly $-15\;\text{mV}$.
5. As the membrane potential rises past the threshold of approximately $-40\;\text{mV}$, the S4 voltage sensors of the voltage-gated $\text{Na}^+$ channels reorient and open the channel. At around the same time, ACh in the synaptic cleft has been hydrolyzed by acetylcholinesterase, closing the nAChR.
6. With the membrane now permeable mainly to $\text{Na}^+$, the membrane potential rises toward $E_{\text{Na}} \approx +60\;\text{mV}$.
7. Before that potential is reached, two things happen. First, the inactivation domain of the $\text{Na}^+$ channel plugs the pore. Second, the slower voltage sensors of the $\text{K}^+$ channels reorient and open those channels, increasing potassium permeability and driving the membrane potential back down toward $E_{\text{K}} \approx -90\;\text{mV}$.
8. As the membrane repolarizes, the $\text{K}^+$ channels deactivate: their voltage sensors return to the resting position and the channels close. The membrane potential stabilizes near the resting value.
9. The $\text{Na}^+/\text{K}^+$ ATPase continuously maintains the sodium and potassium gradients across many cycles of firing. The ion movements per action potential are small relative to the standing gradients, so the gradients are not meaningfully depleted by a single AP; the pump sustains them over time.
10. The depolarization propagates: the local current from each active zone brings the adjacent patch of membrane to threshold, triggering an action potential there, and so on down the axon.
11. Action potentials travel in only one direction because the membrane just behind the active zone is in the absolute refractory period ($\text{Na}^+$ channels inactivated). By the time inactivation lifts, the action potential has moved far enough away that back-propagation cannot occur, ensuring unidirectional travel toward the next synapse.

---

## When It Breaks

### Long QT Syndrome

The **QT interval** on an electrocardiogram measures the duration of the cardiac action potential: from the beginning of ventricular depolarization to the end of ventricular repolarization. Prolonged repolarization, reflected in a lengthened QT interval, predisposes to **torsades de pointes** (literally "twisting of the points"), a polymorphic ventricular tachycardia that can degenerate into ventricular fibrillation and sudden cardiac death.

The cardiac action potential differs from the neuronal action potential primarily in its Phase 2, a prolonged plateau lasting 200 to 300 ms in which voltage-gated $\text{Ca}^{2+}$ channels (L-type, $\text{Ca}_\text{V}1.2$) maintain a depolarized state to allow sufficient $\text{Ca}^{2+}$ entry to trigger myocyte contraction. Repolarization in Phase 3 requires coordinated outward $\text{K}^+$ currents.

**Congenital long QT syndrome (LQTS)** is most commonly caused by loss-of-function mutations in one of two potassium channel genes:

- **LQT1**: mutations in KCNQ1, encoding the $\alpha$-subunit of the $\text{K}_\text{V}$)LQT1 channel (also called $\text{I}_\text{Ks}$), which carries a slow delayed rectifier $\text{K}^+$ current that contributes to Phase 3 repolarization. Loss of function slows repolarization and prolongs the action potential.

- **LQT2**: mutations in KCNH2 (hERG), encoding the $\alpha$-subunit of the channel carrying $\text{I}_\text{Kr}$, the rapid delayed rectifier $\text{K}^+$ current, also critical for Phase 3 repolarization.

In both cases, reducing outward $\text{K}^+$ current during repolarization prolongs the action potential plateau. The prolonged depolarization reopens L-type $\text{Ca}^{2+}$ channels, generating **early afterdepolarizations (EADs)**: secondary depolarizations that can trigger premature action potentials and initiate the arrhythmia. The patient in the opener has a gain-of-delay phenotype: his potassium channels fail to repolarize the myocardium on schedule, and the prolonged action potential triggers the arrhythmia that arrested him.

The hERG channel (LQT2) is also a frequent target of acquired LQTS: many drugs inadvertently block hERG and prolong the QT interval. This off-target effect has caused multiple drugs to be withdrawn from the market and is now screened for in all drug development programs.

Treatment for congenital LQTS is risk stratification and may include beta-blockers (which reduce sympathetic stimulation of the heart and decrease the likelihood of EAD-triggered arrhythmia), implantable cardioverter-defibrillators (ICDs) for high-risk patients, and avoidance of QT-prolonging drugs and hypokalemia (low $\text{K}^+$ reduces the driving force for repolarization and worsens QT prolongation).

### Myasthenia Gravis

**Myasthenia gravis (MG)** is an autoimmune disorder of the NMJ. In approximately 85% of cases, the patient produces IgG antibodies against the **nicotinic acetylcholine receptor**, primarily targeting the extracellular domain. The antibodies cause NMJ failure by three mechanisms:

1. **Receptor cross-linking and internalization**: antibodies bind to adjacent nAChRs on the endplate, cross-link them, and trigger their internalization and degradation by the muscle cell. Fewer receptors remain on the surface.

2. **Complement activation**: the Fc portion of IgG bound to nAChR activates the complement cascade at the NMJ, causing focal membrane lysis and structural disruption of the endplate.

3. **Direct blockade**: some antibodies bind near the ACh-binding site and sterically prevent ACh from binding, directly blocking channel opening.

The net result is a reduction in functional nAChR at the motor endplate. Each vesicle of ACh still releases approximately the same amount of ACh (quantal content is initially normal), but the reduced number of receptors means the EPP is smaller. Below a threshold EPP amplitude, voltage-gated $\text{Na}^+$ channels in the muscle membrane do not reach threshold and the muscle does not fire. With repeated stimulation, acetylcholine stores are depleted faster than they are resynthesized, further reducing EPP amplitude and causing the characteristic fatigable weakness: the patient is weakest after sustained effort and recovers partially with rest.

The **edrophonium test** (used in the opener) exploits this mechanism. Edrophonium is a short-acting inhibitor of acetylcholinesterase. By blocking ACh degradation, it prolongs the dwell time of ACh in the synaptic cleft, allowing each ACh molecule to bind and rebind to the reduced pool of nAChRs. This temporarily compensates for the receptor loss and dramatically reverses weakness for several minutes. A positive edrophonium test is highly specific for MG.

Treatment of MG includes long-acting acetylcholinesterase inhibitors (pyridostigmine), immunosuppression (corticosteroids, azathioprine), plasmapheresis or intravenous immunoglobulin to reduce circulating antibody titers during crises, and in some patients thymectomy (the thymus is the site of autoreactive T cell maturation in MG and its removal can reduce antibody production).

A subset of MG patients (approximately 10%) do not have anti-nAChR antibodies but instead carry antibodies against **muscle-specific kinase (MuSK)**, a receptor tyrosine kinase that organizes nAChR clustering at the endplate during development and maintains the postsynaptic apparatus in adults. Anti-MuSK MG has a distinct clinical profile (more bulbar involvement, less limb weakness) and different treatment sensitivities.

### Local Anesthetics and Voltage-Gated Sodium Channels

Local anesthetics (lidocaine, bupivacaine, procaine) block voltage-gated $\text{Na}^+$ channels by entering the channel pore from the cytoplasmic face and physically occluding it. They preferentially bind to the **inactivated state** of the channel: because open channels rapidly inactivate, and local anesthetics bind and stabilize the inactivated state, they preferentially block rapidly firing neurons (the use-dependent block). Sensory neurons carrying pain signals tend to fire at higher frequencies than motor neurons, and sensory axons are generally smaller and less myelinated, making them more susceptible. This accounts for the differential block of pain sensation before motor function during local anesthesia. The clinical use is direct: blocking $\text{Na}^+$ channels prevents action potential generation and propagation in the injected area.

---

## The MCAT Angle

### What Gets Tested

Channel and transport questions on the MCAT tend to cluster around a few high-yield concepts.

**Passive vs. active transport**: Know that channels and uniporters are passive (move molecules down their electrochemical gradient, no energy required). Pumps and secondary active transporters are active. Primary active transport uses ATP directly. Secondary active transport couples downhill movement of one species (usually $\text{Na}^+$) to uphill movement of another.

**Electrochemical gradients**: Be able to predict which direction an ion will move through an open channel given the membrane potential and the ion's concentration gradient. The driving force is the difference between the actual membrane potential and the ion's equilibrium potential. If $V_m > E_{ion}$, the net force is outward for a cation; if $V_m < E_{ion}$, the net force is inward.

**The Nernst equation**: Know what it calculates (the equilibrium potential for a single ion) and be able to apply it qualitatively. Doubling the concentration ratio of a monovalent cation shifts the equilibrium potential by approximately 18 mV (since $\log_{10}(2) \approx 0.3$ and $61.5 \times 0.3 \approx 18$). The direction follows: if the ratio $[\text{ion}]_{out}/[\text{ion}]_{in}$ increases, $E_{ion}$ becomes more positive for a cation.

**Action potential phases**: Know the sequence (resting, threshold, depolarization via $\text{Na}^+$ channels, repolarization via $\text{K}^+$ channels and $\text{Na}^+$ channel inactivation, afterhyperpolarization, refractory periods). Know that the absolute refractory period is due to $\text{Na}^+$ channel inactivation. Know that action potentials are all-or-nothing.

**Synaptic transmission**: Know the sequence (action potential arrives, $\text{Ca}^{2+}$ enters, vesicle fusion, neurotransmitter release, receptor activation, postsynaptic response). Know the difference between ionotropic (fast, direct channel opening) and metabotropic (slow, GPCR-mediated) receptors.

**$\text{Na}^+$/$\text{K}^+$ ATPase**: Know the stoichiometry (3 $\text{Na}^+$ out, 2 $\text{K}^+$ in per ATP), that it is electrogenic, and that cardiac glycosides inhibit it. Know that its indirect effect (maintaining the $\text{Na}^+$ gradient) is the basis for secondary active transport of glucose and other nutrients.

### The Reasoning Pattern

Transport and channel questions often present a novel scenario (a new drug, a mutant channel, an unusual organism) and ask you to predict the consequence. The chain of reasoning is: what is the normal function of this channel or pump? What happens to the ion gradient if it is blocked or hyperactivated? What does the change in ion gradient do to the membrane potential or to transport of other molecules? What does that change in membrane potential mean for downstream physiology? Work through the chain step by step, not by memorization of outcomes but by first principles.

For MCAT passages on the NMJ, remember that anything that increases ACh at the cleft (acetylcholinesterase inhibition) will initially increase the postsynaptic response, but sustained elevation produces desensitization of nAChR (receptors become unresponsive) and a depolarization block, which is actually inhibitory at high doses. This is the paradox of organophosphate toxicity: the NMJ is flooded with ACh, the muscle initially fasciculates, and then becomes flaccid because the endplate is locked in depolarization.

---

## Worked Problems

### Problem 1

A researcher places a potassium-selective channel into an artificial lipid bilayer separating two solutions. Solution A (left side) contains 150 mM KCl. Solution B (right side) contains 15 mM KCl. Both solutions contain no other ions that permeate the channel. The channel is open.

1. In which direction will potassium initially flow?
2. What voltage (in mV) will develop across the membrane at equilibrium, and which side will be positive?
3. If a second experiment uses 50 mM KCl on the left and 5 mM KCl on the right, how does the equilibrium voltage compare to the first experiment?

**Reasoning:**

1. Potassium will initially flow from high concentration (150 mM, left) to low concentration (15 mM, right). This is the chemical gradient driving potassium from left to right.

2. As potassium flows right, positive charge accumulates on the right side, making the right side positive and the left side negative. This electrical gradient grows until it exactly opposes further net potassium flow: the equilibrium potential. Applying the Nernst equation at 37$^\circ$C (using the ratio from the left side's perspective of outside/inside, but here we need to choose a reference direction):

Using the Nernst equation with left as the "inside" and right as "outside":

$$E_K = 61.5\;\text{mV} \times \log_{10}\frac{[K^+]_{right}}{[K^+]_{left}} = 61.5\;\text{mV} \times \log_{10}\frac{15}{150} = 61.5 \times (-1) = -61.5\;\text{mV}$$

This means the left side is $-61.5$ mV relative to the right side, or equivalently the right side is $+61.5$ mV relative to the left. The right side becomes positive.

3. The ratio in the second experiment is 5/50, which also equals 1/10. The logarithm is identical ($\log_{10}(1/10) = -1$), so the equilibrium voltage is the same: $-61.5$ mV (left relative to right). Only the ratio of concentrations, not the absolute concentrations, determines the Nernst potential.

**Answer:** Potassium flows left to right initially. At equilibrium, the right side is $+61.5$ mV relative to the left. The second experiment produces the same voltage because the concentration ratio is identical.

---

### Problem 2

A patient is brought to the emergency department with profound muscle weakness and respiratory failure after eating home-canned vegetables. He cannot swallow and has bilateral ptosis. Deep tendon reflexes are present and normal. Sensation is intact. A nerve conduction study shows normal sensory nerve conduction but reduced compound muscle action potential (CMAP) amplitude that increases with rapid repetitive stimulation.

1. What is the diagnosis, and what is the molecular mechanism?
2. Why does the CMAP amplitude increase with rapid repetitive stimulation, rather than decrease as it would in myasthenia gravis?
3. An antitoxin and guanidine hydrochloride (which opens voltage-gated $\text{Ca}^{2+}$ channels nonspecifically) are given. Why would guanidine be helpful?

**Reasoning:**

1. The combination of descending paralysis, no fever, intact sensation, preserved reflexes, and increased CMAP with rapid stimulation is botulism. Botulinum toxin cleaves SNARE proteins in the presynaptic motor nerve terminal (the specific SNARE targeted depends on the serotype: serotype A cleaves SNAP-25, serotype B cleaves synaptobrevin/VAMP). SNARE cleavage prevents synaptic vesicles from fusing with the presynaptic membrane in response to $\text{Ca}^{2+}$ influx, blocking ACh release. The NMJ is structurally intact postsynaptically; the nAChRs and the motor endplate are normal. The problem is purely presynaptic.

2. In myasthenia gravis (postsynaptic failure), ACh vesicles are released normally but find fewer nAChRs. With repeated stimulation, ACh stores are depleted faster than resynthesis can replenish them, so EPP amplitude falls with repetition: decremental response. In botulism (presynaptic failure), the SNARE machinery is cleaved and most vesicles cannot fuse. But $\text{Ca}^{2+}$ entering with each successive action potential accumulates slightly in the terminal (presynaptic $\text{Ca}^{2+}$ does not clear instantly). With rapid stimulation, this accumulated $\text{Ca}^{2+}$ increases the probability that the few remaining functional or partially functional SNARE complexes succeed in releasing a vesicle. The result is an incremental response: CMAP amplitude actually increases with repetitive stimulation. This incremental pattern is the electrophysiological signature of a presynaptic NMJ disorder and distinguishes botulism from MG.

3. Guanidine opens voltage-gated $\text{Ca}^{2+}$ channels and increases $\text{Ca}^{2+}$ influx with each action potential. By raising intracellular $\text{Ca}^{2+}$ in the presynaptic terminal, it increases the probability that any vesicles that are near the release site (perhaps attached by partially intact or non-cleaved SNARE complexes) will fuse and release ACh. It partially compensates for the SNARE defect by raising the $\text{Ca}^{2+}$ concentration available to drive what little fusion can still occur.

**Answer:** Botulism, caused by botulinum toxin cleaving presynaptic SNARE proteins and blocking vesicle fusion. Incremental response occurs because repetitive stimulation accumulates presynaptic $\text{Ca}^{2+}$. Guanidine partially compensates by increasing $\text{Ca}^{2+}$ influx.

---

### Problem 3

A pharmaceutical company develops a novel compound that blocks the slow delayed rectifier potassium current (I$_{Ks}$, encoded by KCNQ1) in cardiac ventricular myocytes. The company hopes to use it as an antiarrhythmic agent. However, in clinical trials, several patients develop torsades de pointes.

1. Explain mechanistically why blocking I$_{Ks}$ would produce a prolonged QT interval.
2. The arrhythmia occurs most often during exercise or emotional stress in these patients, not at rest. Why?
3. A separate cohort of patients who have a pre-existing LQT2 mutation (KCNH2 loss-of-function) are enrolled in the trial. Would you expect this group to be at higher or lower risk for arrhythmia from the new compound compared to patients without a pre-existing channelopathy? Explain.

**Reasoning:**

1. $\text{I}_\text{Ks}$ carries one of the two major outward potassium currents that repolarize the ventricle during Phase 3 of the cardiac action potential. Blocking it reduces the net outward current during Phase 3. With less outward $\text{K}^+$ current available, the membrane potential repolarizes more slowly, extending the duration of the action potential plateau. This prolongs the QT interval, because the QT interval is a direct measure of action potential duration in ventricular myocytes. A prolonged plateau increases the probability of L-type $\text{Ca}^{2+}$ channel reactivation and early afterdepolarizations (EADs), which can trigger premature beats and initiate torsades.

2. $\text{I}_\text{Ks}$ is upregulated by sympathetic stimulation through beta-1 adrenergic receptor activation and downstream cAMP-PKA signaling. Under sympathetic drive (exercise, stress), I$_{Ks}$ normally increases substantially to accelerate repolarization at faster heart rates: this is essential because at high heart rates there is less time between beats, and repolarization must be faster to prevent QT prolongation. If I$_{Ks}$ is blocked, this compensatory upregulation cannot occur. The heart rate increases during exercise, the action potential does not shorten appropriately, and the QT interval actually lengthens relative to the cardiac cycle, dramatically increasing arrhythmia risk. Patients with LQT1 mutations have the same vulnerability: their exercise-triggered arrhythmias are exactly explained by the failure of I$_{Ks}$ upregulation during sympathetic stimulation.

3. Higher risk. Repolarization reserve refers to the redundancy built into cardiac repolarization: multiple outward $\text{K}^+$ currents ($\text{I}_\text{Ks}$, $\text{I}_\text{Kr}$, and others) collectively repolarize the ventricle, so losing one can be partially compensated by the others. A patient with LQT2 has already lost $\text{I}_\text{Kr}$ (the other major delayed rectifier current) from their repolarization reserve. Adding a block of $\text{I}_\text{Ks}$ removes a second compensatory current. The combined defect produces a much greater repolarization impairment than either loss alone. This concept, that patients with pre-existing channelopathies or subclinical variants have reduced repolarization reserve and are disproportionately vulnerable to drugs that block $\text{K}^+$ channels, is a major reason the hERG/LQT2 drug-safety screen is essential but is not sufficient on its own.

**Answer:** Blocking $\text{I}_\text{Ks}$ slows Phase 3 repolarization, prolonging action potential duration and the QT interval. Exercise worsens the effect because sympathetic drive normally upregulates $\text{I}_\text{Ks}$ to shorten the QT at fast heart rates; if $\text{I}_\text{Ks}$ is blocked, this compensation fails. LQT2 patients are at higher risk because they have already lost $\text{I}_\text{Kr}$, their repolarization reserve is depleted, and the additional $\text{I}_\text{Ks}$ block is less tolerated.

---

## Summary

The lipid bilayer's impermeability to ions is not a flaw; it is the essential property that allows the cell to store free energy in the form of electrochemical gradients. But the bilayer alone cannot do anything with those gradients. Channels and pumps are the molecular machinery that create, maintain, and discharge them.

Ion channels provide aqueous pores through which specific ions can cross the membrane by diffusion, driven by the electrochemical gradient. Selectivity arises from the geometry of the selectivity filter: the potassium channel uses backbone carbonyl oxygens precisely positioned to substitute for the hydration shell of $\text{K}^+$ but not $\text{Na}^+$. Gating determines when the channel is open: voltage-gated channels respond to membrane potential, ligand-gated channels respond to neurotransmitters or other ligands, and mechanically gated channels respond to membrane deformation.

The $\text{Na}^+$/$\text{K}^+$ ATPase is the primary engine maintaining the sodium and potassium gradients. It exports three sodium ions and imports two potassium ions per ATP consumed, running continuously to offset the passive leak of these ions through channels. The sodium gradient it maintains is subsequently used to drive secondary active transport of glucose, amino acids, and calcium extrusion. Approximately 20 to 30% of resting ATP consumption in most cells, and up to 70% in neurons, powers this pump.

The action potential is the discharge of the sodium gradient across the neuron's axon. Voltage-gated $\text{Na}^+$ channels open at threshold and drive the regenerative depolarization. $\text{Na}^+$ channel inactivation and the delayed opening of voltage-gated $\text{K}^+$ channels repolarize the membrane. The absolute refractory period imposed by $\text{Na}^+$ channel inactivation enforces the all-or-nothing character and unidirectionality of action potential propagation. Myelination increases propagation velocity by orders of magnitude by restricting active depolarization to the nodes of Ranvier.

At the synapse, the action potential is transduced into a chemical signal: calcium influx triggers SNARE-mediated vesicle fusion and neurotransmitter release. Ionotropic receptors provide the fast, direct channel opening that mediates millisecond-scale synaptic transmission. Metabotropic receptors link neurotransmitters to G protein cascades for slower, amplified neuromodulation.

The clinical anchors demonstrate how a single molecular defect propagates to catastrophic physiology. Long QT syndrome shows that cardiac repolarization depends on the coordinated opening of specific potassium channels; a loss-of-function mutation in one channel isoform reduces repolarization reserve, lengthens the action potential, and creates conditions for fatal arrhythmia. Myasthenia gravis shows that the NMJ, which appears redundant (each vesicle releases far more ACh than needed to trigger a muscle action potential), has a finite safety margin, and autoimmune destruction of nicotinic ACh receptors erodes that margin until transmission fails. In both cases, the clinical examination makes sense only when you understand the channel.
