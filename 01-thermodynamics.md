# Chapter 1: Thermodynamic Principles & Why We Exist

---

## Opener Questions

Think about these before you read. Come back to them at the end and see if your answer changed.

1. A reaction has a negative $\Delta G$ but proceeds extremely slowly at room temperature. Is the reaction happening? What determines whether you can observe it?

2. Cells maintain the ATP/ADP ratio far above equilibrium. Why does this matter for the actual $\Delta G$ of ATP hydrolysis inside a cell, compared to the standard $\Delta G^{\circ'}$ you'd look up in a table?

---

## The Big Picture

Here's a paradox that most biochemistry textbooks resolve too quickly.

The second law of thermodynamics says that entropy, the universe's tendency toward dispersal and disorder, spontaneously increases. Fine. But a cell is one of the most organized structures in the known universe: proteins folded into precise three-dimensional shapes, ion gradients maintained across membranes, thousands of chemical reactions running simultaneously in coordinated fashion. How does life exist without violating the second law?

The usual answer, "cells are open systems that take in energy," is true but unsatisfying. It doesn't actually resolve the paradox. It just defers it.

Here's the resolution that actually works: **the second law applies to the universe, not to any particular corner of it**. Cells are local entropy-decreasing machines. They decrease entropy in themselves, yes, but only by increasing entropy elsewhere, faster, by more than enough to compensate. The heat a cell dissipates, the $\text{CO}_2$ it exhales, the disorder it creates in its environment: all of it exceeds the order it builds internally. The universe's entropy still goes up. We just happen to be a temporary eddy running in the other direction.

The cost of being that eddy is constant. The order in a cell doesn't maintain itself; it decays the moment energy input stops. This is why we have to eat. Every meal is a fresh installment of what you owe the second law. Every catabolic reaction (a reaction that breaks down molecules, releasing stored energy), every ATP hydrolysis, every electron tumbling down the electron transport chain (a series of protein complexes that pass electrons step-by-step to oxygen, releasing energy; covered in detail in a later chapter) is entropy debt repayment. Metabolism isn't incidental to life. It *is* life, thermodynamically speaking.

We'll return to this repeatedly throughout the course. For now, hold onto the framing: the organism is the thermodynamic loophole. The pathways are the mechanism of the loophole.

> **Clinical preview:** In the 1930s, dinitrophenol (DNP) was sold as a weight-loss drug. It worked by punching holes in the thermodynamic machinery: patients burned fuel without capturing the energy as ATP, dissipating it as heat instead. Some lost dramatic amounts of weight. Some died of hyperthermia. DNP is still misused today. We'll come back to the mechanism in detail once we've introduced the electron transport chain (covered in a later chapter), but the principle is already visible here: if you uncouple the cellular machinery that captures thermodynamic work, you don't stop generating heat; you just stop doing anything useful with it.

---

## Part I: Thermodynamic Principles

### Entropy: Universal, Not Local

Entropy is often defined as "disorder," which is intuitive but imprecise. More rigorously, entropy is a measure of the number of microstates available to a system: the number of ways energy and matter can be distributed. The more ways, the higher the entropy. A gas expanding into a vacuum increases entropy because there are vastly more positions available to the molecules. A protein unfolding increases entropy because there are vastly more conformations available to the chain than there are for the folded structure.

The second law says that in any spontaneous process, the total entropy of the universe increases. That's the key word: **universe**. Not system. The universe.

A subsystem can absolutely decrease its own entropy, as long as it dumps even more entropy onto its surroundings. A refrigerator decreases entropy inside its compartment by increasing entropy outside (the heat pump). A cell decreases entropy inside itself by increasing entropy in the environment (heat, $\text{CO}_2$, water). Neither violates the second law because neither operates as an isolated system.

Living organisms are open systems: they exchange both energy and matter with their environment. Open systems can locally decrease entropy indefinitely, as long as they're continuously supplied with an energy source to pay for it. The sun is the original energy source for almost everything alive. We eat the sun's output, directly (through photosynthesis, the conversion of sunlight into chemical energy by plants and microorganisms) or indirectly (eating things that photosynthesize). The moment the energy supply stops: organism dies, order collapses, entropy wins.

This is why you have to eat every day, not just once. The loan has to be continuously repaid.

### Enthalpy, Entropy, and Gibbs Free Energy

Whether a chemical reaction proceeds spontaneously depends on two factors pulling in different directions: the energy change in bonds ($\Delta H$, enthalpy) and the change in disorder ($\Delta S$, entropy). Neither one alone determines the outcome. To see why, we need to be precise about what "the system" and "the surroundings" each contribute to the second law.

**The universe = system + surroundings.** When a reaction runs in a cell, the *system* is the reaction itself (the molecules, the bonds breaking and forming). Everything else (the rest of the cell, the body, the room) is the *surroundings*. The second law says total entropy of the universe must increase for a spontaneous process:

$$\Delta S_{univ} = \Delta S_{sys} + \Delta S_{surr} \geq 0$$

The catch: $\Delta S_{surr}$ is not something we measure directly inside a cell. But we can get at it through enthalpy.

**Enthalpy ($\Delta H_{sys}$)** measures heat flow at constant pressure. A negative $\Delta H_{sys}$ (exothermic) means the reaction releases heat to the surroundings; bonds form, energy is released. A positive $\Delta H_{sys}$ (endothermic) means the reaction absorbs heat from the surroundings.

That heat exchange is exactly what changes the entropy of the surroundings. When the system releases heat $q$ into the surroundings at temperature $T$, the surroundings absorb that heat and their entropy increases:

$$\Delta S_{surr} = \frac{q_{surr}}{T} = \frac{-\Delta H_{sys}}{T}$$

The negative sign is because heat leaving the system ($-\Delta H_{sys}$) is heat entering the surroundings ($+q_{surr}$). An exothermic reaction ($\Delta H_{sys} < 0$) increases $\Delta S_{surr}$; an endothermic reaction decreases it. The surroundings function like a heat reservoir: add energy to them and their microstates increase; remove energy and they decrease.

**Entropy ($\Delta S_{sys}$)** measures the change in dispersal within the reaction itself. A positive $\Delta S_{sys}$ means the products are more disordered than the reactants, meaning more microstates are available. This is generally favored. A negative $\Delta S_{sys}$ means the reaction increases order, which costs something thermodynamically.

**Putting it together.** Substituting $\Delta S_{surr} = -\Delta H_{sys}/T$ into the second law:

$$\Delta S_{univ} = \Delta S_{sys} + \frac{-\Delta H_{sys}}{T} \geq 0$$

Multiply both sides by $-T$ (which flips the inequality):

$$-T\Delta S_{univ} = \Delta H_{sys} - T\Delta S_{sys} \leq 0$$

The left side of this expression is defined as **Gibbs Free Energy** $\Delta G$:

$$\Delta G = \Delta H_{sys} - T\Delta S_{sys}$$

So $\Delta G \leq 0$ for a spontaneous process, which is exactly what the second law requires. This is the key insight: **$\Delta G$ is not a new law of nature. It is the second law, rewritten using only system properties.** Instead of tracking entropy changes in the surroundings directly, $\Delta G$ folds the surroundings' response (via $\Delta H_{sys}$) into a single quantity. When $\Delta G < 0$, the total entropy of the universe is increasing. When $\Delta G > 0$, it would decrease, so the reaction doesn't go spontaneously. Effectively $\Delta G$ is a convinient way we "made up" to answer the question: Does this process increase the entropy of the universe given the starting conditions?

The sign of $\Delta G$ tells you everything about spontaneity:

| $\Delta G$ | Meaning |
|-----------|---------|
| $< 0$ | Reaction is spontaneous (exergonic): $\Delta S_{univ} > 0$, products are favored |
| $> 0$ | Reaction is non-spontaneous (endergonic): $\Delta S_{univ} < 0$, reactants are favored |
| $= 0$ | System is at equilibrium: $\Delta S_{univ} = 0$, no net change |

*Note: the equivalence between the sign of $\Delta G$ and the sign of $\Delta S_{univ}$ holds without qualification because $\Delta G = -T\Delta S_{univ}$, and $T$ in Kelvin is always positive. Multiplying or dividing by a positive number never reverses an inequality, so $\Delta G < 0$ is exactly equivalent to $\Delta S_{univ} > 0$, always, at any temperature.*

A reaction is spontaneous when the combined effect on the universe's entropy is positive. An exothermic reaction helps by increasing $\Delta S_{surr}$. A reaction that increases disorder helps by increasing $\Delta S_{sys}$. Either can compensate for an unfavorable contribution from the other. High temperature amplifies the $T\Delta S_{sys}$ term, which is why some endothermic reactions become spontaneous at high temperatures: the system's entropy gain eventually outweighs the heat drain on the surroundings.

**Critical distinction: spontaneity is not speed.** A negative $\Delta G$ means a reaction is spontaneous: it *must* proceed in the forward direction. This is not optional. If $\Delta G < 0$, the system is not at equilibrium and is thermodynamically compelled toward products, in the same way that water is compelled downhill by gravity. The question is not *whether*; it is only *how fast*.

That distinction creates a cognitive trap. We judge whether a reaction "happens" by whether we can *observe* it happening. If the rate is imperceptibly slow, we see nothing and conclude the reaction doesn't occur. Thermodynamics disagrees. Diamond is thermodynamically unstable relative to graphite ($\Delta G < 0$ for the conversion at room temperature and pressure). My wife's wedding ring is unbeknownst to her converting to graphite right now (though I'll be long gone and forgetten before I get in trouble for it). The activation energy barrier is so large that this conversion takes longer than the current age of the universe, and no human will ever observe it, thankfully for me, but it is occurring, because the thermodynamics **requires** it.

The right way to frame the two questions: thermodynamics asks "in which direction must this proceed?" and $\Delta G$ answers it. Kinetics asks "how long will it take?" and activation energy answers that. Enzymes (biological catalysts) operate entirely in the kinetics domain: they don't change $\Delta G$ or alter which direction a reaction must go. They lower the activation energy barrier, making an already-mandatory reaction fast enough to be biologically useful. We'll build on this in a later chapter.

### Standard Free Energy vs. Actual Free Energy

When you look up the free energy of a reaction in a table, you find $\Delta G^{\circ'}$, the **standard free energy change**, under biochemical standard conditions: 25°C, 1 atm, pH 7.0, all solutes at 1 M concentration, water at 55.5 M (treated as 1 by convention).

The problem: none of these conditions exist inside a cell. Metabolite concentrations are in the micromolar to millimolar range, not 1 M. Temperature is 37°C. Reactant and product ratios are nowhere near 1:1.

The actual free energy change in a cell is:

$$\Delta G = \Delta G^{\circ'} + RT\ln\frac{[\text{products}]}{[\text{reactants}]}$$

where $R$ is the gas constant (0.0083145 kJ/mol·K) and $T$ is temperature in Kelvin. The second term is a correction factor that shifts $\Delta G$ based on actual concentrations, telling you whether a reaction must proceed under the conditions that actually exist, not the conditions in a table.

It is worth pausing on why "standard conditions" are what they are. The answer is exceedingly human: 25°C was the temperature in the lab when the measurements were first made, and 1 atm is the pressure we happen to live under. Standards exist because scientists needed to compare results across different labs, not because those conditions are biologically meaningful. The cell does not care about your textbook's reference state.

So the $\Delta G^{\circ'}$ value we look up is true only under those benchmark conditions: 25°C, 1 M concentrations, 1 atm. What we actually need to know is whether a reaction will proceed at 37°C, under the millimolar substrate concentrations inside a real cell. The second term in the equation provides exactly that correction.

This matters enormously for, as an example, ATP. The standard free energy of ATP hydrolysis is:

$$\text{ATP}^{4-} + \text{H}_2\text{O} \rightarrow \text{ADP}^{3-} + \text{P}_\text{i}^{2-} + \text{H}^+ \qquad \Delta G^{\circ'} = -30.5 \text{ kJ/mol}$$

That's the value in a table. Inside a cell, the actual $\Delta G$ of ATP hydrolysis is approximately $-50$ to $-60$ kJ/mol, nearly twice as large in magnitude. The difference comes entirely from the concentration term.

To see why that matters, consider the limiting case. At equilibrium, $\Delta G = 0$ by definition: the reaction has no thermodynamic driving force. Forward and reverse rates are equal, no net work is done, and ATP hydrolysis becomes as useful for driving cellular reactions as a ball sitting at the bottom of a valley is for generating power. The cell would be dead. Not metaphorically; thermodynamically.

The cell avoids this by never letting the system reach equilibrium. Cells maintain the ATP/ADP ratio far above its equilibrium value, keeping [ATP] high and [ADP] and [$\text{P}_\text{i}$] low. Look at the concentration term: $RT\ln([\text{products}]/[\text{reactants}])$. When products are scarce relative to reactants, that ratio is less than one, its logarithm is negative, and the correction term drives $\Delta G$ further below zero. The further from equilibrium, the more negative $\Delta G$ is, and the harder ATP hydrolysis pulls on whatever reaction it's coupled to.

This is why the cell's energy economy depends so critically on maintaining metabolic flux. It isn't just that ATP hydrolysis has a favorable $\Delta G^{\circ'}$. The cell actively maintains conditions that make the actual $\Delta G$ even more favorable. The moment you stop replenishing ATP (stop eating, stop breathing), those ratios collapse toward equilibrium, and the thermodynamic driving force for cellular work vanishes.

### Coupled Reactions

Many biosynthetic reactions have a positive $\Delta G$; they're thermodynamically unfavorable on their own. Cells get around this by **coupling** unfavorable reactions to favorable ones so that the net $\Delta G$ is negative.

The classic example is the phosphorylation of glucose to glucose-6-phosphate, the first step of glycolysis (the ten-step pathway that breaks glucose down to pyruvate, covered in full in a later chapter):

$$\text{Glucose} + \text{P}_\text{i} \rightarrow \text{Glucose-6-phosphate} + \text{H}_2\text{O} \qquad \Delta G^{\circ'} = +13.8 \text{ kJ/mol}$$

This doesn't go. Thermodynamically prohibited on its own. But cells don't run it alone. They couple it to ATP hydrolysis:

$$\text{ATP} + \text{H}_2\text{O} \rightarrow \text{ADP} + \text{P}_\text{i} \qquad \Delta G^{\circ'} = -30.5 \text{ kJ/mol}$$

To find the net reaction, stack them and cancel species that appear on both sides:

$$
\begin{array}{rcll}
\text{Glucose} + \cancel{\text{P}_\text{i}} & \rightarrow & \text{Glucose-6-phosphate} + \cancel{\text{H}_2\text{O}} & \Delta G^{\circ'} = +13.8 \text{ kJ/mol} \\
\text{ATP} + \cancel{\text{H}_2\text{O}} & \rightarrow & \text{ADP} + \cancel{\text{P}_\text{i}} & \Delta G^{\circ'} = -30.5 \text{ kJ/mol} \\
\hline
\text{Glucose} + \text{ATP} & \rightarrow & \text{Glucose-6-phosphate} + \text{ADP} & \Delta G^{\circ'} = -16.7 \text{ kJ/mol}
\end{array}
$$


The net $\Delta G^{\circ'}$ is negative. The reaction proceeds. The favorable hydrolysis of ATP pulls the unfavorable phosphorylation of glucose along with it.

The requirement for coupling to work: the reactions must be **mechanistically linked**, not just written on the same line. "Mechanistically linked" means they share a chemical intermediate, a molecule that is a product of one reaction and a reactant in the next. In the glucose example, that intermediate is the phosphate group itself: ATP donates it directly to glucose in a single enzymatic step catalyzed by hexokinase. The phosphate doesn't float free into solution and then happen to land on glucose; it is physically handed off within the enzyme's active site. That shared intermediate is what makes the math legitimate. Without it, you're just adding two unrelated reactions on paper and pretending the sum means something.

This rules out a lot of combinations that might look attractive on paper. You can't couple glucose phosphorylation to NADH oxidation just because the $\Delta G$ values would add up favorably: there is no shared intermediate, no enzyme that simultaneously does both, no chemical handshake between them. The math would be fictional.

This principle scales up into entire pathways. Glycolysis, for example, is ten sequential reactions, each coupled to the next through shared intermediates: the product of reaction 1 is the substrate for reaction 2, and so on down the line. Thermodynamically, you can treat the whole pathway as one coupled system, summing all ten $\Delta G$ values to get the net driving force. The pathway functions like a single elaborate enzyme that converts glucose to pyruvate, even though it's actually ten different enzymes running in sequence. The intermediates are what chain them together into one coherent thermodynamic unit.

This is the logic of the entire cellular energy economy. ATP hydrolysis is the favorable reaction that drives almost everything unfavorable: ion transport against gradients, biosynthesis of macromolecules, mechanical work of muscle contraction. The cell is a coupling machine. The pathways are the coupling mechanisms.

### ATP: The Right Framing

ATP is commonly described as having "high-energy phosphate bonds," implying that energy is stored in the phosphoanhydride bond itself and released when it breaks. This framing is wrong, and it leads to confusion later.

Bond breaking *costs* energy, always. You don't get energy from breaking bonds. You get energy from the fact that the bonds formed in the products are more stable than the bonds broken in the reactants. The thermodynamic favorability of ATP hydrolysis comes from several sources working together:

**Electrostatic repulsion.** ATP carries 4 negative charges at physiological pH, clustered on the phosphate tail. These charges repel each other. Hydrolysis separates ADP and $\text{P}_\text{i}$, relieving that repulsion.

**Resonance stabilization.** $\text{P}_\text{i}$ (inorganic phosphate) has several resonance structures that distribute its negative charges, making it more stable than the phosphate group when it was part of ATP. The products are more resonance-stabilized than the reactants.

**Increased entropy.** One molecule (ATP) becomes two ($\text{ADP} + \text{P}_\text{i}$), plus a proton is released. More molecules, more dispersal, higher entropy. All of this is favored.

**Decreased solvation of reactants.** The hydration shells around ATP are less favorable than those around the separated products.

None of this is about the bond itself being "high energy." The bond is a normal covalent bond. What's high energy is the *context*: the fact that the molecule carrying that bond is in an unstable, charge-repulsive state relative to its hydrolysis products.

Think of ATP not as a battery storing energy in its bonds, but as a **loaded spring**: a molecule held in a metastable state by the cell's continuous metabolic work, ready to release free energy when it relaxes to a more stable configuration. The cell's job is to keep the spring loaded. Metabolism is the act of loading it.

---

## Part II: Chemical Principles

### pH and the Hydrogen Ion

Water ionizes slightly:

$$\text{H}_2\text{O} \rightleftharpoons \text{H}^+ + \text{OH}^-$$

The equilibrium constant for this is (it has been measured):

$$K_w = [\text{H}^+][\text{OH}^-] = 1.0 \times 10^{-14} \text{ at 25°C}$$

That means that in pure water, $[\text{H}^+] = [\text{OH}^-] = 1.0 \times 10^{-7}$ M. That's a useful baseline, but the notation is awkward: negative exponents everywhere. pH cleans this up:

$$\text{pH} = -\log[\text{H}^+]$$

Pure water: pH = $-\log[10^{-7.0}]=7.0$ (neutral). Values below 7 are acidic ($[\text{H}^+] > 10^{-7}$ M), above 7 are basic ($[\text{H}^+] < 10^{-7}$ M).

Blood pH is maintained between 7.35 and 7.45, a narrow window. This matters because virtually every protein in the body has ionizable groups (more on that later) whose charge state depends on pH. Enzyme active sites are sensitive to pH for the same reason. Hemoglobin's oxygen-binding affinity is pH-dependent (the Bohr effect, covered in Chapter 3). Even a shift of 0.1 pH units in blood represents a nearly 30% change in $[\text{H}^+]$; the log scale compresses large concentration changes into small pH changes, which is worth internalizing.

The clinical significance: when blood pH falls below 7.35 (acidosis) or rises above 7.45 (alkalosis), protein function is disrupted. Severe acidosis (pH < 7.1) is life-threatening. The body maintains blood pH with extraordinary precision, and we'll see exactly how shortly.

### Acids, Bases, and pKa

A **Brønsted-Lowry acid** is a proton donor. A **Brønsted-Lowry base** is a proton acceptor. An acid-base reaction is just a proton transfer:

$$HA \rightleftharpoons \text{H}^+ + A^-$$

The equilibrium constant for this dissociation is $K_a$:

$$K_a = \frac{[\text{H}^+][A^-]}{[HA]}$$

A large $K_a$ means the acid dissociates readily, a strong acid that sits mostly as $A^-$ at equilibrium. A small $K_a$ means it barely dissociates, a weak acid that mostly stays as $HA$.

Just like pH, we take the negative log:

$$pK_a = -\log K_a$$

Low $pK_a$ = strong acid. High $pK_a$ = weak acid. Hydrochloric acid has a $pK_a$ of about $-7$; it's essentially fully dissociated in water. Acetic acid has $pK_a = 4.75$. The carboxyl groups of amino acids have $pK_a$ values around 2-4; their amino groups around 9-10. These numbers matter when we get to protein structure in a later chapter.

The key question $pK_a$ answers: **at a given pH, is this molecule protonated or not?** Here's the intuition: when pH = $pK_a$, the molecule is exactly 50% protonated (HA) and 50% deprotonated ($A^-$). When pH < $pK_a$, the protonated form dominates. When pH > $pK_a$, the deprotonated form dominates.

This single rule will carry you through most of biochemistry. A carboxyl group with $pK_a = 3.5$ at physiological pH 7.4? pH >> $pK_a$, so it's almost entirely deprotonated ($\text{COO}^-$, negatively charged). An amino group with $pK_a = 9.0$ at pH 7.4? pH < $pK_a$, so it's mostly protonated ($\text{NH}_3^+$, positively charged). Charge state determines reactivity, binding interactions, and solubility.

### Henderson-Hasselbalch

The Henderson-Hasselbalch equation comes directly from the $K_a$ expression. Start with what we already have:

$$K_a = \frac{[\text{H}^+][A^-]}{[HA]}$$

Solve for $[\text{H}^+]$:

$$[\text{H}^+] = K_a \cdot \frac{[HA]}{[A^-]}$$

Take the negative log of both sides. Recall that $\log(a \cdot b) = \log a + \log b$, so the right side splits into two terms:

$$-\log[\text{H}^+] = -\log K_a + \left(-\log\frac{[HA]}{[A^-]}\right)$$

$$-\log[\text{H}^+] = -\log K_a - \log\frac{[HA]}{[A^-]}$$

Substitute $\text{pH} = -\log[\text{H}^+]$ and $pK_a = -\log K_a$, and flip the log fraction:

$$\text{pH} = pK_a + \log\frac{[A^-]}{[HA]}$$

That's it. No new assumptions, just algebra on the equilibrium expression you already know. What it tells you: given the $pK_a$ of an acid and the pH of the solution, you can calculate the ratio of deprotonated to protonated form, and vice versa.

**Working with it intuitively:**

- When pH = $pK_a$: $\log\frac{[A^-]}{[HA]} = 0$, so $[A^-] = [HA]$, a 50/50 mixture
- When pH = $pK_a + 1$: $[A^-]/[HA] = 10$ (90% deprotonated)
- When pH = $pK_a - 1$: $[A^-]/[HA] = 0.1$ (90% protonated)

Each pH unit away from $pK_a$ shifts the ratio by a factor of 10. Two units away: factor of 100. The equation is a precision tool for what the intuitive rule approximates.

**Even more intuitively.** You don't need to solve the equation to know which form dominates. Start from:

$$\text{pH} = pK_a + \log\frac{[A^-]}{[HA]}$$

Rearrange:

$$\log\frac{[A^-]}{[HA]} = \text{pH} - pK_a$$

Now the sign does all the work. If $\text{pH} > pK_a$, the right side is positive, so $\log([A^-]/[HA]) > 0$, which means $[A^-]/[HA] > 1$, meaning deprotonated form dominates. If $\text{pH} < pK_a$, the right side is negative, so $\log([A^-]/[HA]) < 0$, which means $[A^-]/[HA] < 1$, meaning protonated form dominates. If $\text{pH} = pK_a$, the right side is zero, the log is zero, and $[A^-] = [HA]$ exactly.

The rule you use in your head ("pH above pKa means deprotonated") isn't a shortcut or an approximation. It is exactly what the equation says.

**MCAT application:** You'll be given a molecule with a known $pK_a$ and asked what form it's in at physiological pH, or how much a pH shift changes the protonation ratio. The Henderson-Hasselbalch equation is the tool. More often, you can answer without solving the equation: if pH is more than 2 units above $pK_a$, it's overwhelmingly deprotonated. If pH is more than 2 units below $pK_a$, it's overwhelmingly protonated. The math confirms what the intuition says.

### pKa Is Not Fixed: Environmental Effects

The $pK_a$ values listed in any table are measured in dilute aqueous solution, where the only environment around the ionizable group is water. Treat those numbers as baselines, not constants. The actual $pK_a$ of a group depends on its local chemical environment, and that environment can shift the apparent $pK_a$ by several units.

You already know one version of this from organic chemistry. Chloroacetic acid ($pK_a = 2.86$) is a stronger acid than acetic acid ($pK_a = 4.75$) because the electronegative chlorine withdraws electron density through the bond, destabilizing the protonated form and making it easier to donate a proton. The covalent environment shifted the $pK_a$ by nearly two units.

The same logic applies through space, via electrostatics. A nearby positive charge destabilizes a protonated (also positively charged) group, because like charges repel. That repulsion makes it thermodynamically easier for the group to give up its proton, which lowers its apparent $pK_a$. A nearby negative charge does the opposite: it stabilizes the protonated form through electrostatic attraction, making it harder to deprotonate, which raises the apparent $pK_a$.

A concrete example: histidine has an imidazole side chain with a $pK_a$ of about 6.0 in free solution. If a positively charged group, such as a protonated lysine, is held in close proximity, the apparent $pK_a$ of the histidine drops. The protonated $His^{+}$ is now destabilized by its positively charged neighbor, so it loses its proton more readily, at a lower pH than it otherwise would shifting the $pK_a$ of a histidine from, say, 6.0 to 4.5 and you have fundamentally changed its behavior at physiological pH: it is now almost entirely deprotonated where it otherwise would have been partially protonated. Interestingly this is what make Histidine such a versitile amino acid in enzyme active sites as we'll come to see.

For now, the mechanism of proximity doesn't matter. What matters is the principle: **the ionization state of a group is determined not just by the solution pH and its baseline $pK_a$, but by every charged group in its vicinity.** We will return to this in detail when we discuss protein structure and enzyme active sites, where these shifts are not incidental but precisely engineered by the three-dimensional arrangement of residues. Active sites exploit local electrostatic environments to hold groups in unusual ionization states that would be impossible in free solution, and that is a large part of how enzymes achieve their catalytic power.

### Buffers

A **buffer** resists changes in pH when acid or base is added. It does this by containing both a weak acid (HA) and its conjugate base ($A^-$) in significant amounts, so that added $\text{H}^+$ gets absorbed by the base ($A^- + \text{H}^+ \rightarrow HA$) and added $\text{OH}^-$ gets absorbed by the acid ($HA + \text{OH}^- \rightarrow A^- + \text{H}_2\text{O}$).

Buffers work best when pH is close to the $pK_a$ of the buffering pair, specifically within ±1 pH unit. Here's why, shown directly from Henderson-Hasselbalch.

Set $\text{pH} = pK_a$ and substitute into the equation:

$$pK_a = pK_a + \log\frac{[A^-]}{[HA]}$$

$$0 = \log\frac{[A^-]}{[HA]}$$

$$10^{0} = 10^{\log\frac{[A^-]}{[HA]}}$$

$$1=\frac{[A^-]}{[HA]}$$

$$[HA] = [A^-]$$

When pH equals $pK_a$, the acid and its conjugate base are present in equal concentrations. This is the point of maximum buffering capacity, because both species are simultaneously at their highest relative abundance. The buffer has the most $A^-$ available to absorb incoming $\text{H}^+$ ($A^- + \text{H}^+ \rightarrow HA$) and the most $HA$ available to absorb incoming $\text{OH}^-$ ($HA + \text{OH}^- \rightarrow A^- + \text{H}_2\text{O}$) at the same time. Move the pH away from $pK_a$ in either direction and one species depletes while the other accumulates, leaving the buffer able to resist changes in only one direction. When pH is far from $pK_a$, the buffer is nearly exhausted on one side and has little capacity left.

**The blood's main buffer: the bicarbonate system.**

$$\text{CO}_2 + \text{H}_2\text{O} \rightleftharpoons \text{H}_2\text{CO}_3 \rightleftharpoons \text{H}^+ + \text{HCO}_3^-$$

The effective $pK_a$ of this system is 6.1. Blood pH is 7.4. That's 1.3 units above $pK_a$, which means the ratio $[\text{HCO}_3^-]/[\text{CO}_2]$ is about 20:1, so the bicarbonate (deprotonated) form vastly predominates. Sounds like a weak buffer since it's far from $pK_a$. So why does it work?

Because this system is **open**. $\text{CO}_2$ is a gas and is continuously exhaled by the lungs. If blood pH drops (acidosis), more $\text{H}^+$ is present, which drives the equilibrium left, producing more $\text{CO}_2$. The respiratory system detects the pH drop, increases breathing rate, and blows off the excess $\text{CO}_2$. If blood pH rises (alkalosis), breathing slows, $\text{CO}_2$ accumulates, $\text{H}^+$ is regenerated, and pH falls back. The lungs are a $\text{CO}_2$ valve that the body uses to tune blood pH in real time.

The kidneys handle slower, longer-term adjustments by excreting or retaining $\text{H}^+$ and $\text{HCO}_3^-$.

This is why the bicarbonate system is effective despite its $pK_a$ being 1.3 units away from blood pH. The buffering capacity isn't just chemical; it's physiological. The whole respiratory system is recruited to keep this buffer functional.

The bicarbonate system dominates in blood plasma. Inside cells, the story is different. The primary intracellular buffer is the phosphate system ($\text{H}_2\text{PO}_4^- / \text{HPO}_4^{2-}$, $pK_a = 6.8$), which sits closer to intracellular pH (~7.2) and is present in high concentrations inside cells. The kidneys also rely heavily on phosphate to buffer urine. Proteins, including hemoglobin in red blood cells, contribute substantially to buffering in both compartments, since their ionizable side chains absorb protons across a wide pH range. No single system handles everything; different compartments use different tools.

---

## When It Breaks

### DNP: Uncoupling the Machine

In 1933, researchers discovered that dinitrophenol (DNP) caused dramatic weight loss. By the mid-1930s, it was being sold in diet pills across the United States. Patients lost weight quickly. They also developed cataracts, peripheral neuropathy, agranulocytosis, and some died of hyperthermia.

The mechanism is thermodynamically elegant and physiologically brutal.

DNP is a lipid-soluble weak acid with a $pK_a$ around 4. At physiological pH, it exists mostly in its deprotonated form ($\text{DNP}^-$). But because it's lipid-soluble, it can cross the inner mitochondrial membrane in either protonated or deprotonated form. Here's what it does: it picks up a proton on the acidic side of the mitochondrial membrane (the intermembrane space, where protons accumulate during electron transport), carries the proton across the membrane, drops it on the basic side (the mitochondrial matrix), and then diffuses back to do it again.

DNP is a **proton shuttle**. It short-circuits the proton gradient.

The proton gradient across the inner mitochondrial membrane is the energy source for ATP synthesis. Normally, protons can only re-enter the matrix through ATP synthase, and that flow drives ATP production. DNP bypasses ATP synthase entirely: protons flood back across the membrane through DNP without producing any ATP. The energy of the gradient is dissipated entirely as heat.

So what happens? The mitochondria respond by burning more fuel, faster, trying to maintain the gradient. They can't. No matter how much glucose or fat is oxidized (broken down by losing electrons to oxygen, releasing energy), none of the energy is captured as ATP; it all becomes heat. Metabolic rate increases dramatically. Body temperature rises. At high enough doses, core temperature rises to levels that denature proteins, and the patient dies.

From a thermodynamic perspective: every living organism is already running a controlled uncoupling. We're thermodynamically inefficient by design: not all the energy released by fuel oxidation becomes ATP; a substantial fraction is deliberately released as heat to maintain body temperature. DNP just turns the dial all the way up, eliminating the useful work entirely.

DNP is still used illegally today, purchased online, and deaths continue to occur. The mechanism hasn't changed.

### Metabolic Acidosis and Alkalosis

Normal blood pH: 7.35-7.45. Outside this range, the body is in trouble.

**Acidosis** (pH < 7.35) can arise from:
- Diabetic ketoacidosis: accumulation of ketone bodies (acetoacetate, beta-hydroxybutyrate, and acetone: weak acids produced from fat breakdown when glucose is unavailable, covered in a later chapter) in uncontrolled diabetes
- Lactic acidosis: excess lactate produced when oxygen-deprived tissues run glycolysis without oxygen (anaerobic glycolysis, covered in a later chapter)
- Respiratory failure: $\text{CO}_2$ accumulates when lungs can't exhale it, driving blood pH down via the bicarbonate equilibrium
- DNP toxicity: uncoupling drives futile cycling that generates lactate and disrupts mitochondrial function, causing a mixed metabolic and respiratory acidosis

**Alkalosis** (pH > 7.45) can arise from:
- Hyperventilation: blowing off too much $\text{CO}_2$, pulling the bicarbonate equilibrium toward $\text{HCO}_3^-$ formation and reducing $[\text{H}^+]$
- Vomiting: loss of gastric acid removes $\text{H}^+$ from the body
- Certain diuretics (drugs that increase urine output) that cause loss of $\text{H}^+$

Why does pH matter so much? Protein function. Every enzyme in the body has amino acid side chains in its active site with specific ionization states required for catalysis (we'll see exactly what this looks like in a later chapter). Hemoglobin's affinity for oxygen changes with pH; acidosis shifts the oxygen-dissociation curve, affecting delivery to tissues (covered in a later chapter). Ion channel gating is pH-sensitive. Cytoskeletal dynamics are pH-dependent.

Small pH shifts have large functional consequences because the Henderson-Hasselbalch relationship is steep near physiological pH: a 0.1-unit pH change shifts protonation ratios of molecules with $pK_a$ near 7 by 25% or more. The body does not have much room to drift.

---

## The MCAT Angle

The MCAT tests thermodynamics and acid-base chemistry repeatedly. The patterns worth recognizing:

**$\Delta G$ and spontaneity:** You'll be given a $\Delta G^{\circ'}$ value and asked whether a reaction proceeds under cellular conditions. Remember that $\Delta G^{\circ'}$ is not $\Delta G$; the actual free energy depends on concentrations. A reaction with a slightly positive $\Delta G^{\circ'}$ might be spontaneous inside a cell if reactant concentrations are high and product concentrations are low. The question is always about the actual $\Delta G$, not the table value.

**The kinetics trap:** Questions will describe a thermodynamically favorable reaction ($\Delta G < 0$) that proceeds slowly or not at all. The answer is almost always: the activation energy barrier is high, and an enzyme (or catalyst) is needed to lower it. Never confuse thermodynamic spontaneity with kinetic feasibility.

**ATP hydrolysis under cellular conditions:** If asked to calculate $\Delta G$ for ATP hydrolysis in a cell, you need the cellular concentrations of ATP, ADP, and $\text{P}_\text{i}$, not just $\Delta G^{\circ'}$. The cellular $\Delta G$ is approximately $-50$ to $-60$ kJ/mol, roughly twice the standard value.

**Henderson-Hasselbalch, dominant form at physiological pH:** Given a molecule's $pK_a$ and told the pH is 7.4, the question is usually: what charge does this group carry? The quick answer: if $pK_a < 7.4$, it's deprotonated (negatively charged carboxyl groups, neutral amines). If $pK_a > 7.4$, it's protonated (neutral carboxyl groups, positively charged ammonium groups). The equation gives you the exact ratio if needed.

**Le Chatelier applied to free energy:** "What happens to $\Delta G$ as product accumulates?" As product accumulates, the ratio in $RT\ln\frac{[\text{products}]}{[\text{reactants}]}$ increases, making $\Delta G$ less negative (or more positive). The reaction slows thermodynamically. This is why product removal (e.g., by subsequent reactions in a pathway) keeps early reactions running: it maintains a large negative $\Delta G$ throughout.

---

## Worked Problems

### Problem 1: Spontaneity vs. Speed

A reaction has $\Delta H^{\circ'} = -20$ kJ/mol and $\Delta S^{\circ'} = -50$ J/mol·K. At 37°C (310 K):

(a) Calculate $\Delta G^{\circ'}$.
(b) Is the reaction spontaneous under standard conditions?
(c) The reaction proceeds at a rate of approximately one event per year in the absence of a catalyst. What does this tell us?

**Solution:**

(a)

$$\Delta G^{\circ'} = \Delta H^{\circ'} - T\Delta S^{\circ'} = -20{,}000 \text{ J/mol} - (310 \text{ K})(-50 \text{ J/mol} \cdot \text{K})$$

$$= -20{,}000 + 15{,}500 = -4{,}500 \text{ J/mol} = -4.5 \text{ kJ/mol}$$

(b) $\Delta G^{\circ'} < 0$, so yes, spontaneous under standard conditions. The reaction must proceed in the forward direction; products are thermodynamically required.

(c) A rate of one event per year means the reaction is thermodynamically mandatory but kinetically invisible. It is occurring; we simply cannot observe it. The activation energy barrier is so large that the rate is negligible on any biologically relevant timescale. This is the situation enzymes evolved to solve: they don't change $\Delta G$ or make mandatory reactions more mandatory. They lower the activation energy barrier so that a reaction the thermodynamics already requires actually proceeds fast enough to be useful.

---

### Problem 2: Coupled Reactions

Reaction A: $$X \rightarrow Y \quad \Delta G^{\circ'} = +22 \text{ kJ/mol}$$

Reaction B: $$\text{ATP} + \text{H}_2\text{O} \rightarrow \text{ADP} + \text{P}_\text{i} \quad \Delta G^{\circ'} = -30.5 \text{ kJ/mol}$$

(a) Can reaction A proceed on its own under standard conditions?
(b) If reaction A is mechanistically coupled to ATP hydrolysis, what is the net $\Delta G^{\circ'}$?
(c) What is required for this coupling to actually work?

**Solution:**

(a) $\Delta G^{\circ'} = +22$ kJ/mol $> 0$, so reaction A is thermodynamically unfavorable under standard conditions. Reactant X is favored at equilibrium.

(b) The coupled reaction is simply the sum:

$$X + \text{ATP} + \text{H}_2\text{O} \rightarrow Y + \text{ADP} + \text{P}_\text{i}$$

$$\Delta G^{\circ'} = +22 + (-30.5) = -8.5 \text{ kJ/mol}$$

The coupled reaction is spontaneous under standard conditions.

(c) Mechanistic linkage. The reactions must share a chemical intermediate or be catalyzed by an enzyme that physically connects the two processes, for example by transferring the phosphate group from ATP directly to X rather than hydrolyzing ATP in solution and hoping the energy somehow carries over. Writing two reactions on the same line doesn't couple them. The chemistry has to be connected.

---

### Problem 3: Henderson-Hasselbalch and the Bicarbonate System

Carbonic acid ($\text{H}_2\text{CO}_3$) has an effective $pK_a$ of 6.1 in blood (accounting for the $\text{CO}_2/\text{H}_2\text{CO}_3$ equilibrium). Normal blood pH is 7.4.

(a) Calculate the ratio $[\text{HCO}_3^-]/[\text{CO}_2]$ in normal blood.
(b) A patient develops metabolic acidosis and blood pH drops to 7.1. How does this change the ratio?
(c) The patient's breathing rate increases. Why does this compensate for the acidosis?

**Solution:**

(a) Apply Henderson-Hasselbalch:

$$7.4 = 6.1 + \log\frac{[\text{HCO}_3^-]}{[\text{CO}_2]}$$

$$\log\frac{[\text{HCO}_3^-]}{[\text{CO}_2]} = 1.3$$

$$\frac{[\text{HCO}_3^-]}{[\text{CO}_2]} = 10^{1.3} \approx 20$$

At normal blood pH, there are roughly 20 bicarbonate ions for every molecule of dissolved $\text{CO}_2$.

(b) At pH 7.1:

$$7.1 = 6.1 + \log\frac{[\text{HCO}_3^-]}{[\text{CO}_2]}$$

$$\log\frac{[\text{HCO}_3^-]}{[\text{CO}_2]} = 1.0$$

$$\frac{[\text{HCO}_3^-]}{[\text{CO}_2]} = 10$$

The ratio drops from ~20 to 10. The acidosis has shifted the equilibrium toward the protonated form ($\text{CO}_2$). Relatively more $\text{CO}_2$ is present and less $\text{HCO}_3^-$; the buffer has been partially consumed.

(c) Increased breathing rate exhales more $\text{CO}_2$ from the blood. The bicarbonate equilibrium:

$$\text{CO}_2 + \text{H}_2\text{O} \rightleftharpoons \text{H}^+ + \text{HCO}_3^-$$

When $[\text{CO}_2]$ drops (because it's being exhaled), the equilibrium shifts left, consuming $\text{H}^+$ to regenerate $\text{CO}_2$ and water. Blood $[\text{H}^+]$ decreases, pH rises back toward normal. The lungs are using $\text{CO}_2$ excretion as a lever to control blood pH in real time.

---

## Opener Questions Revisited

Return to the questions from the beginning:

**1. A reaction has a negative $\Delta G$ but proceeds extremely slowly at room temperature. What's missing?**

Nothing is missing from the thermodynamics. $\Delta G < 0$ means the reaction is spontaneous and must proceed in the forward direction; that is already determined. What the question is really asking is why we cannot *observe* it proceeding. The answer is kinetics: the activation energy barrier between reactants and products is large, so even though the reaction must occur, it does so at a rate that is unmeasurable on a human timescale. What is absent is a catalyst (in biology, an enzyme) to lower that barrier and make the rate biologically useful. Spontaneity and speed are completely independent. The thermodynamics is settled; the kinetics is the bottleneck.

**2. Cells maintain the ATP/ADP ratio far above equilibrium. Why does this matter for the actual $\Delta G$ of ATP hydrolysis inside a cell?**

The actual $\Delta G$ of any reaction depends on the concentrations of reactants and products via:

$$\Delta G = \Delta G^{\circ'} + RT\ln\frac{[\text{products}]}{[\text{reactants}]}$$

For ATP hydrolysis, the "products" are ADP and $\text{P}_\text{i}$. Cells keep [ATP] high and [ADP] and [$\text{P}_\text{i}$] low, far from equilibrium, which keeps the concentration ratio $\frac{[\text{ADP}][\text{P}_\text{i}]}{[\text{ATP}]}$ small, making the logarithm term large and negative. This makes the actual $\Delta G$ significantly more negative than $\Delta G^{\circ'}$ alone. The cellular $\Delta G$ of ATP hydrolysis is approximately $-50$ to $-60$ kJ/mol, vs. $-30.5$ kJ/mol under standard conditions. The cell is exploiting metabolic flux to maximize the thermodynamic driving force of its energy currency.

---

*Chapter 2: Protein Composition & Structure*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*

---

## Problem Set

**Problem 1.**
A reaction has $\Delta H^{\circ'} = +12$ kJ/mol and $\Delta S^{\circ'} = +60$ J/mol·K.

(a) Calculate $\Delta G^{\circ'}$ at 37°C (310 K).

(b) Is the reaction spontaneous under standard conditions at this temperature?

(c) At what temperature (in Kelvin) does this reaction become thermodynamically neutral (i.e., $\Delta G^{\circ'} = 0$)? What does it mean for spontaneity below versus above this temperature?

---

**Problem 2.**
Consider the two-step biosynthetic pathway below:

$$\text{Reaction 1: } A \rightarrow B \quad \Delta G^{\circ'} = +18 \text{ kJ/mol}$$

$$\text{Reaction 2: } B + \text{ATP} + \text{H}_2\text{O} \rightarrow C + \text{ADP} + \text{P}_\text{i} \quad \Delta G^{\circ'} = -25 \text{ kJ/mol}$$

(a) Can Reaction 1 proceed spontaneously on its own under standard conditions?

(b) Calculate the net $\Delta G^{\circ'}$ for the overall conversion of $A$ to $C$.

(c) A student argues: "It doesn't matter whether these reactions share an intermediate — the math still works out." Explain why this student is wrong.

---

**Problem 3.** *(Synthesis)*
Inside a resting muscle cell, the concentrations of ATP, ADP, and inorganic phosphate ($\text{P}_\text{i}$) are approximately 8 mM, 0.9 mM, and 1.0 mM, respectively. The standard free energy of ATP hydrolysis is $\Delta G^{\circ'} = -30.5$ kJ/mol. $R = 0.008314$ kJ/mol·K; $T = 310$ K.

(a) Calculate the actual $\Delta G$ of ATP hydrolysis under these cellular conditions.

(b) During intense exercise, ATP falls to 6 mM, ADP rises to 2 mM, and $\text{P}_\text{i}$ rises to 4 mM. Recalculate $\Delta G$ under these conditions and compare it to part (a). In which direction does the actual free energy of hydrolysis move, and why?

(c) A student claims that the cell should just make ATP concentrations as high as possible to maximize the thermodynamic driving force for ATP hydrolysis. Identify the flaw in this reasoning using the $\Delta G$ equation.

---

**Problem 4.**
For each of the following scenarios, predict the sign of $\Delta H$, $\Delta S$, and $\Delta G$ (or state that it is indeterminate from the information given). Briefly justify each answer.

(a) A protein unfolds in hot water. The unfolded chain is far more flexible than the folded structure, and heat is absorbed from the surroundings.

(b) Two ions of opposite charge, initially far apart in solution, come together to form a tight ion pair. No heat is exchanged with the surroundings.

(c) A single ATP molecule is hydrolyzed to ADP and $\text{P}_\text{i}$ inside a cell at 37°C. (Consider both the standard conditions contribution and the concentration term.)

---

**Problem 5.** *(Synthesis)*
The pKa of lactic acid is 3.86. During a sprint, lactic acid is produced in muscle cells (intracellular pH ≈ 7.2) and is exported into blood plasma (pH 7.4).

(a) Using the Henderson-Hasselbalch relationship, determine the ratio of lactate ($A^-$) to lactic acid ($HA$) at pH 7.2 and at pH 7.4. You do not need to compute exact numbers — a qualitative comparison using the rule of signs is sufficient.

(b) In both compartments, which form dominates overwhelmingly? What does this mean for the charge on the molecule that is actually transported across the plasma membrane?

(c) Blood pH can fall to 7.1 during severe lactic acidosis. A physician worries that this will disrupt enzyme function. Explain the molecular basis of this concern, connecting blood pH, protein side-chain pKa values, and enzyme active-site chemistry.

---

**Problem 6.** *(Synthesis)*
Dinitrophenol (DNP) is a lipid-soluble weak acid with a pKa of approximately 4. It can cross the inner mitochondrial membrane in both its protonated ($\text{DNPH}$) and deprotonated ($\text{DNP}^-$) forms.

(a) At the pH of the mitochondrial intermembrane space (approximately 6.7), is DNP predominantly protonated or deprotonated? Justify using the pH vs. pKa relationship.

(b) At the pH of the mitochondrial matrix (approximately 7.9 under normal conditions), is DNP predominantly protonated or deprotonated?

(c) Using your answers to (a) and (b), explain the thermodynamic logic of how DNP acts as a proton shuttle across the inner mitochondrial membrane. In one sentence, state the consequence for ATP synthesis and explain why weight loss results.

---

**Problem 7.**
The bicarbonate buffering system in blood has an effective pKa of 6.1.

(a) A patient hyperventilates due to a panic attack, blowing off excess $\text{CO}_2$. Predict what happens to blood pH. Use the bicarbonate equilibrium to show your reasoning.

(b) A second patient has been vomiting severely for 48 hours, losing significant gastric acid ($\text{HCl}$). Predict the direction of blood pH change and identify whether this is a respiratory or metabolic disturbance.

(c) The bicarbonate system's pKa (6.1) is 1.3 units below normal blood pH (7.4), yet it is the dominant blood buffer. Why does this system buffer effectively despite being far from its pKa? What feature of this buffer system compensates for the poor chemical positioning?

---

**Problem 8.** *(Synthesis)*
A medicinal chemist synthesizes a drug that strongly inhibits an enzyme with $\Delta G^{\circ'} = -45$ kJ/mol for its catalyzed reaction. A colleague objects: "This drug will prevent a thermodynamically favorable reaction from occurring, which should be impossible — thermodynamics says it must proceed." Evaluate this objection. Is the colleague correct that thermodynamics prevents the drug from working? What principle does the drug actually exploit, and what does this tell you about the relationship between $\Delta G$ and the observable rate of a reaction?

---

## References

1. Berg JM, Tymoczko JL, Gatto GJ, Stryer L. *Biochemistry*, 9th ed. W.H. Freeman; 2019.
2. Nelson DL, Cox MM. *Lehninger Principles of Biochemistry*, 8th ed. W.H. Freeman; 2021.
3. Atkins P, de Paula J. *Physical Chemistry for the Life Sciences*, 2nd ed. Oxford University Press; 2011.
4. Grundlingh J, Dargan PI, El-Zanfaly M, Wood DM. 2,4-Dinitrophenol (DNP): a weight loss agent with significant acute toxicity and risk of death. *J Med Toxicol*. 2011;7(3):205–212. doi:10.1007/s13181-011-0162-6
5. Miranda EJ, McIntyre IM, Parker DR, Gary RD, Logan BK. Two deaths attributed to the use of 2,4-dinitrophenol. *J Anal Toxicol*. 2006;30(3):219–222. doi:10.1093/jat/30.3.219
6. Nicholls DG, Ferguson SJ. *Bioenergetics 4*. Academic Press; 2013. [Standard reference for oxidative phosphorylation and uncoupling.]
7. Alberty RA. Thermodynamics of biochemical reactions at specified pH. *J Biol Chem*. 2005;280(39):33142–33150. doi:10.1074/jbc.M502115200
8. Hammes GG. Multiple conformational changes in enzyme catalysis. *Biochemistry*. 2002;41(26):8221–8228. doi:10.1021/bi0260839
9. Rawn JD. *Biochemistry*. Neil Patterson; 1989. [Classic treatment of the bicarbonate buffer system and acid–base physiology.]
10. Stewart PA. Modern quantitative acid-base chemistry. *Can J Physiol Pharmacol*. 1983;61(12):1444–1461. doi:10.1139/y83-207
11. Davenport HW. *The ABC of Acid-Base Chemistry*, 6th ed. University of Chicago Press; 1974. [Foundational treatment of Henderson–Hasselbalch applied to clinical acid–base balance.]
12. de Bold AJ. Atrial natriuretic factor: a hormone produced by the heart. *Science*. 1985;230(4727):767–770. [Context: pH homeostasis and its systemic hormonal regulation.]
