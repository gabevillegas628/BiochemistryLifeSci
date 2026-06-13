# Chapter 14: Glycogen Metabolism

---

## Opener Questions

Think about these before you read. Come back at the end and see if your answer changed.

1. A 19-year-old man presents after a basketball game with severe leg cramps and dark brown urine. His blood glucose is completely normal. His symptoms resolve after about 30 minutes of rest. He mentions this has happened before during hard exercise, but he has noticed that if he slows down and keeps going for another few minutes, the cramps ease up and he can continue. What enzyme deficiency explains this, and why does his pain improve after pushing through it?

2. A 3-month-old girl presents with poor feeding, severe muscle weakness, and a massively enlarged heart on echocardiogram. Her blood glucose after a 4-hour fast is 74 mg/dL, which is normal. A muscle biopsy under electron microscopy shows glycogen accumulating inside membrane-bound vesicles. Which enzyme is deficient, and why is the glycogen in an unusual compartment rather than free in the cytoplasm?

---

## The Big Picture

Glucose is the cell's preferred immediate fuel, but a cell that tried to stockpile free glucose would face a problem: glucose is osmotically active. Osmotic pressure is the tendency of water to move across a membrane toward a region of higher solute concentration. Every dissolved molecule contributes to it, regardless of how large or small it is. A single glucose molecule and a single protein molecule each count as one particle for osmotic purposes. Pack enough free glucose into a cell to supply several hours of metabolism and water floods in by osmosis, the cell swells, and it lyses. The cell needs a way to store glucose that does not raise osmolarity.

Glycogen is the answer. Glycogen is a branched polymer of glucose: thousands of glucose residues linked together in a form that exerts almost no osmotic pressure. The key is that the entire polymer counts as a single dissolved particle, the same as one free glucose molecule would. One glycogen granule represents thousands of glucose equivalents stored in a single osmotic unit. When the cell needs glucose, it peels the polymer apart one residue at a time.

Two tissues dominate glycogen metabolism, and they use it for completely different purposes.

**The liver stores glycogen as a glucose buffer for the bloodstream.** After a meal, the liver absorbs glucose from the portal circulation and packs it into glycogen. During fasting, it releases glucose by breaking glycogen down, maintaining blood glucose between meals. Liver glycogen is not for the liver's own energy needs: it is for the organism. A well-fed adult has roughly 100-120 g of liver glycogen.

**Muscle stores glycogen as a local fuel reserve.** Muscle glycogen is for the muscle's own use, not for the bloodstream. Muscle lacks a key enzyme that would allow it to export glucose, so its glycogen is a private fuel supply for burst activity. The first several seconds of a maximal sprint run largely on muscle glycogen. A well-fed adult has roughly 400-500 g of glycogen distributed across skeletal muscle, but none of it is collectively accessible to the bloodstream.

Total glycogen stores can sustain roughly 12-16 hours of fasting before they are exhausted. After that, the liver shifts to gluconeogenesis, synthesizing glucose from scratch, to maintain blood glucose. Once muscle glycogen is depleted, it stays depleted in that tissue until glucose or lactate replenishes it from the circulation.

---

## Glycogen Structure

Glycogen is built from glucose units connected by two types of linkages.

**$\alpha$-1,4 linkages** form the main chains: the C1 of one glucose connects to the C4 of the next, creating linear stretches. These are the bonds that glycogen phosphorylase cleaves during breakdown.

**$\alpha$-1,6 linkages** form the branch points: roughly every 8-12 residues, a side chain branches off from the C6 of a chain glucose. These branches themselves branch further, creating a tree-like structure with many tips pointing outward. Each tip is called a non-reducing end.

The branching is not decorative, its function is speed of both glycogen synthesis and breakdown.

The enzyme responsible for breaking glycogen down can only work from the non-reducing end of a chain, removing one glucose at a time (the mechanism is covered in the next section). A linear polymer of 10,000 glucose units would have a single non-reducing end, and a single enzyme molecule would have to make 10,000 successive cuts down that one chain to release all the glucose. A heavily branched polymer has hundreds of non-reducing ends, and hundreds of enzyme molecules can attack simultaneously. Branching maximizes the surface area available for breakdown, which is why muscle glycogen can be mobilized so rapidly during a sprint or during a fight-or-flight response.

---

## Glycogen Synthesis

### Activating Glucose

Glucose cannot be added directly to glycogen. It must first be activated into a form the glycogen synthase enzyme can use.

The starting material, glucose-6-phosphate (from hexokinase or liver glucokinase), is converted to **glucose-1-phosphate** by the enzyme **phosphoglucomutase**. This is reversible, so it also runs in reverse during glycogen breakdown as we'll see.

$$\text{Glucose-6-phosphate} \rightleftharpoons \text{Glucose-1-phosphate}$$

Glucose-1-phosphate then reacts with UTP (uridine triphosphate) via **UDP-glucose pyrophosphorylase**:

$$\text{Glucose-1-phosphate} + \text{UTP} \rightarrow \text{UDP-glucose} + \text{PP}_\text{i} \quad (\Delta G \approx 0 \text{ kJ/mol})$$

The product, **UDP-glucose**, is the activated form of glucose that glycogen synthase will use. The pyrophosphate ($\text{PP}_\text{i}$) released is immediately hydrolyzed by pyrophosphatase:

$$\text{PP}_\text{i} + \text{H}_2\text{O} \rightarrow 2\,\text{P}_\text{i} \quad (\Delta G \approx -33 \text{ kJ/mol})$$

This hydrolysis is highly favorable thermodynamically, and it is what makes the whole activation reaction essentially irreversible. The cell commits one UTP equivalent per glucose unit stored. You can think of UDP-glucose as glucose carrying a charged "handle" that glycogen synthase can grab.

As you might imagine, synthesizing such a complex molecule as Glycogen requires energy, where does this energy come from? It comes from the activation of G6P to form UDP-Glc via the action of Nucleoside Diphosphate Kinase which essentially makes a UTP count as an ATP. We'll see this directly in the next section.


### Initiation: Glycogenin

Glycogen synthase has a fundamental limitation: it can only extend an existing chain. It cannot start a new one from scratch (*de novo*). Every glycogen granule therefore requires a **primer**, a short starter chain that glycogen synthase can extend. That primer is synthesized by a protein called **glycogenin**.

Glycogenin is a self-glucosylating enzyme. It catalyzes its own modification by transferring a glucose from UDP-glucose onto the hydroxyl group of a specific tyrosine residue (Tyr194 in humans), forming an O-glycosidic bond between the tyrosine and the C1 of glucose. This is the seed of the new granule. Glycogenin then continues extending that chain, adding glucose residues one at a time via $\alpha$-1,4 linkages, until the chain reaches about 7-8 residues. At that length, glycogen synthase can bind and take over elongation.

Glycogenin remains covalently attached to the reducing end of the finished granule, buried at its core. Each mature glycogen granule contains one glycogenin molecule at its center, which means, interestingly, that although we refer to glycogen as having a reducing end, in practice glycogen is technically a non-reducing sugar!

### Adding to the Chain

**Glycogen synthase** transfers glucose from UDP-glucose onto the non-reducing end of an existing chain, forming a new $\alpha$-1,4 linkage and releasing UDP:

$$\text{UDP-glucose} + \text{glycogen}_{(n)} \rightarrow \text{glycogen}_{(n+1)} + \text{UDP}$$

Starting from Glucose 6 phosphate and following it thorough its addition to Glycogen produces the following balanced process:

$$
\begin{array}{rcl}
\text{G6P} & \rightleftharpoons & \cancel{\text{G1P}} \\
\cancel{\text{G1P}} + \cancel{\text{UTP}} & \rightarrow & \cancel{\text{UDP-Glc}} + \cancel{\text{PP}_\text{i}} \\
\cancel{\text{PP}_\text{i}} + \text{H}_2\text{O} & \rightarrow & 2\,\text{P}_\text{i} \\
\cancel{\text{UDP}} + \text{ATP} & \rightarrow & \cancel{\text{UTP}} + \text{ADP} \\
\cancel{\text{UDP-Glc}} + \text{glycogen}_{(n)} & \rightarrow & \text{glycogen}_{(n+1)} + \cancel{\text{UDP}} \\
\hline
\text{G6P} + \text{H}_2\text{O} + \text{ATP} + \text{glycogen}_{(n)} & \rightarrow & \text{glycogen}_{(n+1)} + 2\,\text{P}_\text{i} + \text{ADP}
\end{array}
$$

The net cost for adding one glucose to glycogen is one ATP equivalent, consumed by NDP kinase to regenerate UTP from UDP. The thermodynamic driving force comes from two reactions: PPi hydrolysis ($\Delta G^{\circ'} \approx -19$ kJ/mol), which is what makes the activation of UDP-glucose essentially irreversible, and the glycogen synthase step itself ($\Delta G^{\circ'} \approx -13.4$ kJ/mol). Notice that G6P's phosphate ester is never broken: the phosphate from G6P travels through G1P, into UDP-glucose, into UDP, and back into UTP via NDP kinase, completing a catalytic cycle. Both Pi in the net reaction come from that single PPi hydrolysis step, not from G6P.

### Creating Branches

Once a growing chain reaches about 11 residues, **branching enzyme** (also called glycosyl-4,6-transferase) transfers a 6-7 residue segment from the end of the chain and reattaches it via an $\alpha$-1,6 linkage at a position at least 4 residues back from the nearest existing branch point. This creates a new branch tip that glycogen synthase can extend and that branching enzyme can branch again later.

The net cost: one UTP (really ATP) per glucose residue added to glycogen. The branching reaction itself does not require additional energy input.

---

## Glycogen Breakdown

### Phosphorolysis, Not Hydrolysis

The conceptually important thing about glycogen breakdown is that glycogen phosphorylase does not use water to cleave glucose. It uses inorganic phosphate. This is called **phosphorolysis**, and the distinction matters for ATP accounting.

**Glycogen phosphorylase** cleaves the terminal glucose from a non-reducing end, using $\text{P}_\text{i}$ as the nucleophile:

$$\text{Glycogen}_{(n)} + \text{P}_\text{i} \rightarrow \text{Glycogen}_{(n-1)} + \text{Glucose-1-phosphate}$$

Glycogen phosphorylase is a **processive** enzyme: once it binds to a non-reducing end, it does not release the chain between cleavages. It stays bound and walks inward along the chain, releasing one glucose-1-phosphate after another without having to rebind for each cut. The alternative would be a **distributive** enzyme, which releases its substrate after every catalytic event and must find and rebind the chain anew each time. Distributive behavior has a kinetic cost: each rebinding event takes time, and under the urgency of a fight-or-flight response that delay compounds quickly across thousands of glucose units. Processivity eliminates that overhead. Combined with the branched structure of glycogen providing hundreds of simultaneous non-reducing ends, a cell can flood the cytoplasm with glucose-1-phosphate almost instantly when demand spikes.

Phosphorylase does not run indefinitely on a single chain. It stalls when it reaches about 4 residues from a branch point (discussed in the next section), at which point it dissociates and finds another available non-reducing end.

The product is **glucose-1-phosphate**, not free glucose. Phosphoglucomutase then converts glucose-1-phosphate to glucose-6-phosphate, which enters glycolysis at the second step, bypassing hexokinase.

It is tempting to conclude from this that glycogen-derived glucose produces a bonus ATP compared to free glucose, since hexokinase is skipped at breakdown. There is no free lunch here. The full accounting shows the opposite: storing glucose as glycogen and then retrieving it actually costs one net ATP compared to using free glucose directly.

| Step(s)| Direct glycolysis | Via glycogen |
|---|---|---|
| Hexokinase (synthesis) | −1 ATP | −1 ATP |
| NDP kinase (synthesis) | — | −1 ATP |
| PFK-1 | −1 ATP | −1 ATP |
| 2× PGK + 2× PK | +4 ATP | +4 ATP |
| **Net (to pyruvate)** | **+2 ATP** | **+1 ATP** |

The hexokinase step is bypassed at breakdown, which is why glycolysis from G6P returns +3 ATP rather than +2. But that gain is exactly canceled by the extra ATP spent during synthesis (the NDP kinase step that regenerates UTP from UDP). The net is +1 ATP per glucose via glycogen versus +2 ATP directly, a roughly 3.5% reduction in total yield when you account for the full oxidation of glucose. That is the price of storage: the cell pays a small energetic overhead to keep glucose in a rapidly mobilizable, osmotically inert form.

### The Debranching Problem

Phosphorylase has a limitation: it can only cleave $\alpha$-1,4 linkages, and it stalls 4 residues away from a branch point. The structure it leaves is called a **limit dextrin**. Without help, phosphorylase cannot proceed further.

**Debranching enzyme** solves this with two catalytic activities built into a single protein:

**Transferase activity:** moves the 3 terminal residues from a stub onto the free end of another chain via an $\alpha$-1,4 linkage, exposing the single branch-point glucose that is connected by an $\alpha$-1,6 bond.

**Glucosidase activity:** cleaves that $\alpha$-1,6 linkage, releasing the branch-point glucose as **free glucose**, not glucose-1-phosphate.

That distinction matters. Free glucose must be phosphorylated by hexokinase before entering glycolysis, at a cost of one ATP. Branch-point glucoses represent roughly 1 in 10 residues in glycogen, so about 10% of glycogen glucose costs one ATP to re-enter glycolysis. The remaining 90% is recovered as glucose-1-phosphate via phosphorolysis, no ATP required. Overall glycogen mobilization is still highly efficient, but not quite as ATP-free as phosphorolysis alone would suggest.

### Tissue Divergence at Glucose-6-Phosphate

After phosphorylase and debranching enzyme finish their work, glucose-6-phosphate (from the ~90% phosphorolytic fraction) reaches a decision point that differs by tissue:

**In muscle:** there is no glucose-6-phosphatase. Glucose-6-phosphate proceeds directly into downstream metabolic pathways like glycolysis or the PPP, we cannot convert it back to free gluclose. Remember muscles are selfish.

**In liver:** **glucose-6-phosphatase**, located in the endoplasmic reticulum membrane, removes the phosphate group, releasing free glucose into the bloodstream. This single enzyme is what makes liver glycogen useful as a blood glucose buffer. Only tissues with glucose-6-phosphatase (primarily liver, and to a minor extent kidney and intestinal epithelium) can contribute to blood glucose from glycogen.

---

## Regulation

Glycogen synthesis and breakdown are reciprocally regulated so that both cannot run simultaneously. Running synthesis and breakdown at the same time would accomplish nothing except wasting the ATP and UTP spent on synthesis. The regulation operates at two levels:
1. Hormonal signals (course adjustment) set the global state based on whole-body glucose status
2. Allosteric signals fine-tune the local response based on the energy status of the individual cell.

### Covalent Regulation: Phosphorylation

Glycogen Phosphorylase exists as a homodimer, both subunits can exists in either the phosphorylated or unphosphorylated state (S14 in humans). The phosphorylated state of phosphorylase is referred to as **phosphorylase *a***, the unphosphorylated form is **phosphorylase *b***. Additionally, like all allosterically regulated enzymes, phosphorylase can exist in either the R state or T state. 

- **phosphorylase *a*** favors the active R state
- **phosphorylase *b*** favors the inactive T state

The conversion from the ***a*** form to the ***b*** form is hormonally controlled. *However*, **phosphorylase *a*** can be "coaxed" into adopting the T state and **phosphorylase *b*** the R state locally via allosteric regulation. These are the two levels of regulation: Hormonally controlled phosphorylation "primes" phosphorylase to be either more or less active (***a*** vs ***b*** form) but local signals inside the cell can override that depending on local conditions.

Glycogen synthase exists as a homotetramer. Unlike phosphorylase, which has a single key phosphorylation site (Ser14), each synthase subunit carries multiple serine residues that can be phosphorylated by several different kinases. The cumulative phosphorylation state of the enzyme determines its activity. The dephosphorylated form is referred to as **synthase I** (for *independent* — it is active without requiring any additional co-factors), and the phosphorylated form is **synthase D** (for *dependent* — it requires glucose-6-phosphate to show any significant activity). You might wonder why synthase doesn't use the a/b naming like phosphorylase. The reason is that for phosphorylase, the phosphorylated form is the active one (phosphorylase *a*). For synthase it is the opposite — dephosphorylation activates it. Calling the active dephosphorylated synthase "synthase a" would contradict the logic students already learned for phosphorylase, so the I/D naming was adopted to avoid that confusion.

- **Synthase I** is the active form
- **Synthase D** is the less active form, but can be partially rescued by glucose-6-phosphate

The conversion from **synthase I** to **synthase D** is hormonally controlled, driven by phosphorylation at multiple sites. *However*, **synthase D** can be "coaxed" back toward activity by high intracellular concentrations of glucose-6-phosphate, which acts as a local allosteric activator. This mirrors the two-level logic seen in phosphorylase: hormones set the global phosphorylation state, but local metabolite concentrations can modulate activity on top of that.

Both glycogen synthase and glycogen phosphorylase are regulated by phosphorylation, but in opposite directions:

**Glycogen phosphorylase:** phosphorylation at Ser14 converts the less active **phosphorylase b** to the more active **phosphorylase a**. Phosphorylation turns it on.

**Glycogen synthase:** phosphorylation at multiple sites converts the active form (sometimes called **synthase I**, for insulin-stimulated or independent of AMP) to the less active form (sometimes called **synthase D**, for AMP-dependent or glucose-6-phosphate-dependent). Phosphorylation turns it off.

The enzyme that phosphorylates phosphorylase b is **phosphorylase kinase**, which is itself activated by phosphorylation (via PKA) and by calcium. The enzyme that dephosphorylates both phosphorylase a and inactive synthase (restoring the basal, glycogen-synthesizing state) is **protein phosphatase 1 (PP1)**.

A second kinase that phosphorylates glycogen synthase is worth knowing: **glycogen synthase kinase 3 (GSK-3)**. GSK-3 phosphorylates synthase at multiple sites, pushing it toward the inactive D form. What makes GSK-3 interesting is how insulin shuts it off. Insulin activates a kinase cascade (PI3K → Akt) that culminates in Akt phosphorylating and inactivating GSK-3. With GSK-3 off, synthase is no longer being driven toward the D form, and PP1 can tip the balance toward the active I form. This is a large part of why insulin promotes glycogen synthesis: not by directly activating synthase, but by removing the brake that GSK-3 applies to it.

### The Hormonal Cascade

**Glucagon** (acting on liver) and **epinephrine** (acting on liver and muscle) signal through G-protein coupled receptors. Binding activates adenylyl cyclase, which generates cAMP. cAMP activates **protein kinase A (PKA)**. PKA then phosphorylates two targets simultaneously:

- **Phosphorylase kinase** (note, glcogen phosphorylase is *not* a targer of PKA) is phosphorylated and activated. Active phosphorylase kinase phosphorylates phosphorylase b, converting it to phosphorylase a which now favors the more active R state and Glycogen will begin to be phosphorylized producing G1P.

- **Glycogen synthase** is phosphorylated directly by PKA (and by phosphorylase kinase at a separate site), converting it from the active **I form** to the inactive **D form** preventing glycogen synthesis.

The signal is amplified at each step: one glucagon molecule activates adenylyl cyclase repeatedly, generating many cAMP molecules; each cAMP activates PKA; each active PKA phosphorylates many phosphorylase kinase molecules; each active phosphorylase kinase phosphorylates many phosphorylase b molecules. By the time the signal reaches glycogen phosphorylase, the original hormonal event has been amplified many thousandfold.

**Insulin** reverses this. Insulin activates phosphodiesterase (which degrades cAMP) and activates PP1 (which dephosphorylates the pathway). PP1 dephosphorylates phosphorylase a (inactivating it) and dephosphorylates glycogen synthase (activating it). Glycogen synthesis is turned on; breakdown is turned off.

### Allosteric Regulation

Hormonal regulation responds to whole-organism signals (a drop in blood glucose triggering glucagon release, for instance). Allosteric regulation responds to local conditions inside the individual cell, without waiting for any signal from outside.

**In muscle, AMP activates phosphorylase b directly.** AMP rises when ATP is being consumed rapidly, because adenylate kinase converts two ADP to one ATP plus one AMP. High AMP signals a cell in energy deficit. It allosterically activates phosphorylase b, bypassing the need for the full hormonal cascade. ATP and glucose-6-phosphate are allosteric inhibitors of phosphorylase b, signaling that energy is already adequate. This means a vigorously contracting muscle cell can activate its own glycogen breakdown from the inside, through the consequences of its own energy consumption, without epinephrine arriving from outside.

**In liver, free glucose inhibits phosphorylase a allosterically.** After a meal, portal blood glucose rises. Glucose binds to liver phosphorylase a at an allosteric site and triggers a conformational change that exposes the enzyme's phosphorylated serine, making it a better substrate for PP1. PP1 dephosphorylates phosphorylase a, converting it to the inactive b form. At the same time, PP1 activates glycogen synthase. Rising blood glucose is therefore a direct signal to the liver to stop breaking down glycogen and start storing it, without requiring insulin to act immediately. This glucose-sensing mechanism is liver-specific: muscle phosphorylase a does not respond to glucose this way, which makes physiological sense because muscle glycogen is not about blood glucose regulation.

### Calcium Coordinates Contraction with Fuel Mobilization

**Phosphorylase kinase** contains a **calmodulin** subunit as part of its structure. Calmodulin binds calcium and is activated by it. When a motor neuron fires and triggers muscle contraction, calcium floods from the sarcoplasmic reticulum into the cytoplasm (Recall the $G_{\alpha q}$ DAG/IP3 cascade from chapter 8). That calcium activates calmodulin, which activates phosphorylase kinase, which converts phosphorylase b to active phosphorylase a. Glycogen breakdown starts at the same instant as contraction, triggered by the same calcium signal, without waiting for epinephrine to arrive.

The logic: the act of contracting is itself the signal to mobilize fuel. The muscle does not need to wait for a hormonal signal to know it is working.

---

## When It Breaks: Glycogen Storage Diseases

Glycogen storage diseases (GSDs) are inherited disorders of glycogen synthesis or degradation. They are categorized by the affected enzyme and, historically, by a Roman numeral assigned in the order of discovery. Each one illustrates what happens when a single step in the pathway is blocked, and each one follows directly from the biochemistry.

### Von Gierke Disease (Type I): No Glucose-6-Phosphatase

The deficiency is in **glucose-6-phosphatase**, the liver endoplasmic reticulum enzyme that removes the phosphate group from glucose-6-phosphate to release free glucose into the blood. Without it, the liver can break down glycogen all the way to glucose-6-phosphate but cannot take the final step.

The consequences follow directly:

**Severe fasting hypoglycemia.** Liver glycogen cannot contribute to blood glucose. Blood glucose falls rapidly when feeding stops. Infants with Von Gierke disease cannot sustain blood glucose through even a few hours of fasting, and before the disease was understood and treated, many died of hypoglycemia overnight.

**Hepatomegaly.** Glucose-6-phosphate and glycogen accumulate inside liver cells (G6P has nowhere to go, and its accumulation drives continued glycogen synthesis), enlarging the liver substantially.

**Lactic acidosis.** Backed-up glucose-6-phosphate is shunted into glycolysis, producing excess pyruvate and lactate. Blood lactate is chronically elevated.

**Hyperuricemia and gout.** The accumulated G6P drives flux through the pentose phosphate pathway, generating excess ribose-5-phosphate that feeds purine synthesis and ultimately uric acid production. Additionally, during hypoglycemic episodes, ATP consumption rises and nucleotide catabolism accelerates, further producing uric acid. Gout presenting in a child or young adult is an important diagnostic clue.

**Hyperlipidemia.** Excess acetyl-CoA (from glycolysis running on backed-up G6P) is diverted into fatty acid and triglyceride synthesis, elevating blood triglycerides and cholesterol.

Management is dietary: frequent small meals, uncooked cornstarch (a slowly digested starch that acts as a slow-release glucose source overnight), and avoidance of fasting. Liver transplant is curative because the transplanted liver carries normal glucose-6-phosphatase.

### Pompe Disease (Type II): No Lysosomal Acid Maltase

Pompe disease is mechanistically distinct from every other glycogen storage disease because the deficient enzyme, **acid alpha-glucosidase (GAA)**, is a lysosomal enzyme. Lysosomes normally degrade glycogen sequestered during autophagy. When GAA is absent or severely reduced, glycogen accumulates inside lysosomes throughout the body, visible on electron microscopy as glycogen packed inside membrane-bound vesicles.

Because cytoplasmic glycogen metabolism is entirely intact, **blood glucose is completely normal**. This is the key clinical distinguishing feature: no hypoglycemia, no hepatomegaly from cytoplasmic glycogen backup, but progressive accumulation of lysosomal glycogen in cardiac and skeletal muscle.

In the **infantile form**, the lysosomal glycogen load accumulates rapidly in cardiac muscle, causing massive cardiomegaly. Affected infants present within the first months of life with hypotonia (floppy baby), cardiomegaly visible on chest X-ray, and respiratory failure from diaphragm and intercostal muscle weakness. Without treatment, infantile Pompe disease is fatal by the second year of life from cardiac failure. Cardiac muscle is disproportionately affected because of its exceptionally high rate of autophagy under constant mechanical stress.

The **late-onset form** has some residual GAA activity and presents in adults as slowly progressive limb-girdle myopathy, often misdiagnosed as muscular dystrophy for years. Diaphragm weakness is the eventual life-limiting problem.

Enzyme replacement therapy with recombinant GAA is available and substantially changes the prognosis of infantile Pompe disease when started early.

### McArdle Disease (Type V): No Muscle Glycogen Phosphorylase

McArdle disease is a deficiency of the muscle-specific isoform of glycogen phosphorylase. The liver isoform is entirely normal. Blood glucose regulation is intact. Only muscle is affected.

Patients present with **exercise intolerance**: cramping, stiffness, and pain during intense or sustained exercise, beginning within the first few minutes of vigorous effort. With severe or prolonged overexertion, muscle cells are damaged enough to release myoglobin into the bloodstream, causing myoglobinuria (burgundy-colored urine) and, in serious episodes, renal failure.

Two clinical features are distinctive:

**Normal fasting glucose.** Liver phosphorylase is normal, so hepatic glycogenolysis and blood glucose regulation are unaffected.

**The second wind phenomenon.** After approximately 7-10 minutes of moderate exercise, many McArdle patients notice an abrupt improvement: cramping eases, heart rate normalizes, and exercise becomes tolerable. The second wind is not a repair of anything. It occurs because hepatic glucose output (from intact liver glycogenolysis) and fatty acid release from adipose tissue have increased enough to supply the muscle with circulating fuel. The muscle was starved of its local glycogen fuel at the onset of exercise; once blood-borne glucose and fatty acids arrive in sufficient quantity, the demand can be met through those alternative routes instead. The second wind is the moment circulation catches up.

The **ischemic forearm exercise test** is the classic diagnostic maneuver. The patient squeezes a hand dynamometer while a blood pressure cuff occludes blood flow. In normal individuals, venous lactate rises (glycolysis is running in the ischemic muscle). In McArdle patients, lactate does not rise (without glycogenolysis, there is no local glucose to feed glycolysis), but ammonia rises normally (the purine nucleotide cycle, which generates ammonia from AMP, is intact). This pattern of absent lactate rise with a normal ammonia rise is the diagnostic fingerprint of muscle glycogen phosphorylase deficiency.

---

## The MCAT Angle

Glycogen metabolism appears on the MCAT primarily in three forms.

**The regulation cascade.** You should be able to trace the full hormonal sequence from glucagon or epinephrine binding to activated glycogen phosphorylase a, naming each component: hormone binds GPCR, adenylyl cyclase activated, cAMP produced, PKA activated, phosphorylase kinase phosphorylated and activated, phosphorylase b phosphorylated to phosphorylase a. Simultaneously, glycogen synthase is phosphorylated and inactivated. Questions often ask about the effect of PKA activation on glycogen synthase, or what happens if phosphodiesterase is inhibited.

**Liver versus muscle distinctions.** Know that muscle cannot export glucose (no glucose-6-phosphatase), while liver can. Know that muscle phosphorylase b is allosterically activated by AMP (energy sensing) while liver phosphorylase a is allosterically inhibited by glucose (glucose sensing). A question may present a patient with a deficiency in one tissue but not the other and ask you to predict the clinical consequences.

**Phosphorolysis and ATP accounting.** The MCAT occasionally asks why glycogen is an efficient fuel source. The answer is phosphorolysis: glycogen phosphorylase uses $\text{P}_\text{i}$ rather than water, releasing glucose-1-phosphate that enters glycolysis at the second step without requiring the ATP that hexokinase would normally spend. This saves one ATP per glucose residue recovered by phosphorylase. Branch-point glucoses are the exception: released as free glucose, they require hexokinase and cost one ATP.

**Glycogen storage diseases.** The MCAT distinguishes the major GSDs by their clinical signature. Von Gierke: severe fasting hypoglycemia, lactic acidosis, hepatomegaly, normal muscle. Pompe: cardiomegaly and myopathy, normal glucose, lysosomal glycogen accumulation. McArdle: exercise-induced cramping, normal fasting glucose, second wind phenomenon. Pompe is the one lysosomal GSD and the one with cardiac involvement.

---

## Worked Problems

### Problem A

A 19-year-old cross-country runner presents to student health after interval training with severe leg cramping. She reports this happens regularly with intense effort but never on easy runs. A venous blood sample drawn immediately after a brief stair-climbing test shows undetectable lactate; her training partner's lactate is 2.8 mmol/L. Her ammonia rises normally after the same test.

(a) What enzyme deficiency explains her presentation?

(b) She asks why easy runs cause no symptoms. Explain in terms of fuel use.

(c) During a 90-minute easy run, would you expect her blood glucose to fall more, less, or about the same compared to a classmate with normal enzyme function? Explain.

**Answer:**

(a) McArdle disease: deficiency of the muscle-specific isoform of glycogen phosphorylase. She cannot mobilize muscle glycogen. During high-intensity exercise, muscle glycolysis is starved of its local glucose substrate, ATP production cannot keep pace with demand, and cramping results. The absent lactate rise on ischemic forearm exercise confirms the defect is in local muscle glycogenolysis (no G1P produced, so glycolysis cannot run, so no lactate), while the normal ammonia rise confirms the purine nucleotide cycle is intact and that the muscle was genuinely working.

(b) Easy running relies primarily on fatty acid oxidation and circulating blood glucose, with local glycogen contributing modestly. At low exercise intensity, ATP demand is low enough that blood-borne fuels can fully sustain it without significant dependence on local glycogen mobilization. High-intensity intervals demand ATP faster than blood-borne fuels can supply it, and normal muscle bridges this gap with local glycogen breakdown. Since she cannot access her glycogen, the deficit shows up only when intensity is high enough that circulating fuels cannot keep pace.

(c) Her blood glucose would fall more during prolonged exercise than her classmate's. Because she cannot use muscle glycogen, her muscles rely more heavily on circulating blood glucose throughout the run. The increased peripheral uptake of blood glucose accelerates glucose consumption from the circulation. Her liver glycogen is normal and will compensate via hepatic glycogenolysis and eventually gluconeogenesis, but the demand placed on circulating glucose is higher than in a person whose muscles are drawing on their own local glycogen reserves as well. In practice, McArdle patients can experience symptomatic hypoglycemia during prolonged exercise.

---

### Problem B

A 3-month-old infant presents with poor feeding and profound hypotonia. Echocardiogram shows the heart is massively enlarged, with septal hypertrophy and poor contractile function. Blood glucose after a 4-hour fast is 76 mg/dL. A muscle biopsy shows glycogen accumulation inside membrane-bound vesicles. Genetic testing reveals a homozygous nonsense mutation in the GAA gene.

(a) Why is blood glucose normal despite massive glycogen accumulation?

(b) What compartment is the glycogen accumulating in, and why does that compartment accumulate glycogen when GAA is absent?

(c) Why is cardiac muscle affected so severely in the infantile form?

**Answer:**

(a) The GAA gene encodes acid alpha-glucosidase, a lysosomal enzyme. Pompe disease blocks only the lysosomal pathway for glycogen clearance. Cytoplasmic glycogen metabolism, including glycogen phosphorylase, debranching enzyme, and glucose-6-phosphatase, is entirely intact. The liver continues to break down and synthesize cytoplasmic glycogen normally and maintains blood glucose appropriately. Blood glucose is normal because the enzyme deficiency does not touch the cytoplasmic glycogenolytic pathway.

(b) Glycogen is accumulating inside lysosomes. Lysosomes perform autophagy, a process by which cells engulf and degrade portions of their own cytoplasm, including glycogen granules. Inside the lysosome, acid alpha-glucosidase normally hydrolyzes the glycogen. Without GAA, glycogen that enters lysosomes cannot be degraded. It accumulates inside the lysosomal membrane, appearing as membrane-enclosed vesicles on electron microscopy.

(c) Cardiac muscle operates under constant mechanical stress and has an unusually high rate of autophagy compared to most tissues, reflecting the continuous need to turn over damaged proteins and organelles in a cell that never stops working. When lysosomal glycogen clearance is blocked, cardiac myocytes accumulate glycogen faster than other cell types. The physical accumulation of glycogen within lysosomes disrupts the contractile machinery, stiffens and enlarges the cells, and impairs force generation, ultimately producing the progressive dilated cardiomyopathy seen in infantile Pompe disease.

---

### Problem C

A researcher adds epinephrine simultaneously to isolated liver cells and isolated muscle cells and measures glycogen phosphorylase activity and glycogen synthase activity over 15 minutes. Ten minutes into the experiment, she adds 10 mM glucose to the liver cells.

(a) What happens to glycogen phosphorylase activity in both cell types after epinephrine? Describe the mechanism in each tissue.

(b) What happens to glycogen synthase activity in both cell types? State the enzyme responsible for the change.

(c) After glucose is added to liver cells, what happens to phosphorylase a activity in liver? Would the same response occur in muscle cells? Why or why not?

**Answer:**

(a) Glycogen phosphorylase activity increases in both cell types. Epinephrine binds $\beta$-adrenergic receptors, activating adenylyl cyclase via a Gs protein, raising cAMP, and activating PKA. PKA phosphorylates phosphorylase kinase, activating it. Active phosphorylase kinase then phosphorylates phosphorylase b to produce the more active phosphorylase a. This cascade operates in both tissues. In muscle, there is an additional mechanism: the epinephrine-driven calcium release (via IP3 signaling) directly activates phosphorylase kinase through its calmodulin subunit even before the cAMP cascade fully activates. In muscle, the vigorous contraction triggered by epinephrine also generates AMP from rapid ATP consumption, allosterically activating phosphorylase b independent of phosphorylation. In liver, these calcium and AMP contributions are much smaller; the PKA cascade is dominant.

(b) Glycogen synthase activity decreases in both cell types. PKA directly phosphorylates glycogen synthase at multiple serine residues, converting it from the active dephosphorylated form to the less active phosphorylated form. Phosphorylase kinase also phosphorylates glycogen synthase at a separate site. The net result is reciprocal regulation: breakdown is turned on and synthesis is turned off by the same cascade.

(c) In liver cells, phosphorylase a activity would decrease after glucose addition. Free glucose is an allosteric inhibitor of liver phosphorylase a: glucose binds to the active site (the same site that normally binds the glucose product released during glycogenolysis) and induces a conformational change that exposes the Ser14 phosphorylation site, making it a better substrate for protein phosphatase 1. PP1 dephosphorylates phosphorylase a, converting it to the less active phosphorylase b. The same PP1 then activates glycogen synthase. Rising blood glucose signals the liver to switch from breakdown to storage automatically. This response would not occur in muscle cells. Muscle phosphorylase a does not have the same glucose-responsive allosteric site. Muscle phosphorylase responds to AMP, ATP, and glucose-6-phosphate, not to circulating glucose. The liver is designed to sense blood glucose; the muscle is designed to sense its own energy status. These are different jobs, and the regulatory machinery reflects that.

---

## Opener Questions Revisited

**1. Young man with exercise-induced cramps, dark urine, and a second wind.**

The patient has McArdle disease: deficiency of the muscle-specific isoform of glycogen phosphorylase. His muscle cannot break down glycogen during exercise, so glycolysis is starved of local glucose and ATP production falls rapidly during intense effort. Cramping is the result of inadequate ATP.

Dark urine after extreme exertion is myoglobinuria, caused by muscle breakdown (rhabdomyolysis) during episodes of severe ischemic demand. The kidneys filter myoglobin from the blood, producing the characteristic color.

The second wind occurs around 7-10 minutes of continued moderate exercise, when hepatic glycogenolysis and fatty acid mobilization from adipose tissue have ramped up enough to supply fuel to the muscle via the circulation. The cramps ease not because anything in the muscle has recovered, but because blood-borne glucose and fatty acids have caught up to the demand. The liver isoform of glycogen phosphorylase is completely normal, so hepatic glycogenolysis functions correctly and blood glucose is maintained.

**2. Infant with cardiomegaly and normal blood glucose.**

The infant has Pompe disease (GSD Type II), caused by deficiency of lysosomal acid alpha-glucosidase (GAA). Glycogen accumulating inside lysosomes throughout the body is visible as membrane-bound vesicles on electron microscopy, confirming that the accumulation is lysosomal rather than cytoplasmic.

Blood glucose is normal because cytoplasmic glycogen metabolism is intact. Only the lysosomal clearance pathway is blocked. Cardiac muscle is disproportionately affected in the infantile form because of its high autophagy rate under constant contractile stress: lysosomal glycogen accumulates faster in cardiac cells than in most other tissues, eventually disrupting contractile function and producing the massive cardiomegaly seen here.

---

*Chapter 15 turns from glucose storage to fat mobilization. Beta-oxidation is the pathway that takes stored fatty acids and converts them back to acetyl-CoA, the same two-carbon unit the TCA cycle runs on. The accounting connects directly to everything we have already built.*

---

*This chapter is part of a free, openly licensed course companion for Biochemistry for Life Sciences (694:395) at Rutgers University. Licensed under CC BY-NC-SA 4.0.*

---

## Problem Set

**Problem 1.**
Glycogen is a branched polymer. A hypothetical organism synthesizes glycogen with a deficiency of branching enzyme, producing essentially linear chains.

(a) How would the rate of glycogen mobilization during an epinephrine surge be affected compared to normal? Explain using the logic of enzyme access.

(b) Andersen disease (GSD Type IV) is caused by a true branching enzyme deficiency. Patients develop progressive liver cirrhosis, despite the fact that glycogen synthesis is not eliminated, merely altered in structure. Why would accumulation of abnormal, nearly unbranched glycogen chains lead to liver failure?

(c) If a muscle cell tried to store the same number of glucose equivalents as free glucose dissolved in the cytoplasm rather than as glycogen, estimate roughly what would happen to the osmolarity of the cell. Why would this be incompatible with cell survival?

---

**Problem 2.**
The activation of glucose for glycogen synthesis requires UDP-glucose rather than a simple phosphorylated glucose.

(a) Write the reaction catalyzed by UDP-glucose pyrophosphorylase. Identify both substrates and both products.

(b) The overall activation reaction (glucose-1-phosphate to UDP-glucose) has a small favorable free energy change by itself. The reaction is made essentially irreversible in cells by a second enzymatic step. What is that step, and why does it drive the synthesis of UDP-glucose forward?

(c) Glycogenin is described as the primer for new glycogen granules. What chemical group on glycogenin accepts the first glucose, and what type of bond is formed? If a muscle cell somehow lost all of its glycogenin protein, what would happen to its ability to synthesize glycogen?

---

**Problem 3.**
Glycogen phosphorylase uses inorganic phosphate to cleave glucose from glycogen, releasing glucose-1-phosphate rather than free glucose.

(a) Trace the subsequent fate of a glucose residue released by glycogen phosphorylase in muscle. Name each enzymatic step up to the point of entry into glycolysis. Compare the ATP cost of this route with the ATP cost of starting from free blood glucose taken up by the same muscle cell.

(b) Roughly 10% of glycogen residues are branch-point glucoses, released as free glucose by the glucosidase activity of debranching enzyme. Why does recovering these residues cost an additional ATP compared to residues released by phosphorylase?

(c) A genetic variant of glycogen phosphorylase has been discovered in which the active site cannot bind inorganic phosphate and instead uses water as the nucleophile, releasing free glucose. Predict the metabolic consequence in terms of ATP yield per glycogen glucose compared to the normal enzyme.

---

**Problem 4.**
Glucagon is released from pancreatic alpha cells during fasting and acts primarily on the liver.

(a) Trace the complete signaling cascade from glucagon binding to its receptor to the appearance of active glycogen phosphorylase a in a hepatocyte. Name each enzyme activated and state whether each activation step involves covalent modification (phosphorylation) or allosteric change.

(b) At the same time this cascade activates glycogen phosphorylase, what happens to glycogen synthase? Name the enzyme responsible and state whether synthase is more active or less active after glucagon signaling.

(c) Glucagon binds one receptor on one hepatocyte, yet thousands of glycogen phosphorylase molecules become active within seconds. Explain the mechanism of signal amplification at each step of the cascade.

---

**Problem 5.**
Liver and muscle use glycogen for different purposes, and their regulation reflects these differences.

(a) Free glucose allosterically inhibits liver phosphorylase a but has no effect on muscle phosphorylase a. Explain the physiological rationale for this tissue-specific difference. What would go wrong if muscle phosphorylase a were inhibited by blood glucose the same way liver phosphorylase a is?

(b) AMP allosterically activates muscle phosphorylase b but has little regulatory effect on liver phosphorylase b. What does rising AMP signal in a muscle cell, and why is it appropriate for this signal to trigger local glycogen breakdown?

(c) A physician suspects Von Gierke disease (G6Pase deficiency) in a 6-month-old infant but notes that the hypoglycemia during a supervised fast, while present, is less severe than expected. The family reports that the mother breastfeeds frequently. Laboratory analysis shows the infant's kidney has normal glucose-6-phosphatase activity. Propose a mechanism for partial compensation.

---

**Problem 6.** *(Synthesis)*
Von Gierke disease (GSD Type I) is caused by glucose-6-phosphatase deficiency in the liver.

(a) Explain why Von Gierke patients develop chronic lactic acidosis. Begin with the direct consequence of G6Pase deficiency and follow the logic through to lactate production.

(b) Von Gierke patients develop hyperuricemia and are at risk for gout even in childhood. Propose two mechanistically distinct pathways by which G6Pase deficiency increases uric acid production.

(c) Von Gierke patients are managed with frequent meals and uncooked cornstarch given at bedtime. Cooked starch does not work as well for overnight glucose maintenance. Propose why raw, uncooked cornstarch has a sustained glucose-releasing effect that cooked starch lacks.

---

**Problem 7.** *(Synthesis)*
Two children are referred to a metabolic genetics clinic. Child A has severe fasting hypoglycemia, hepatomegaly, elevated blood lactate, and completely normal muscle strength and exercise tolerance. Child B has a normal fasting glucose, no hepatomegaly, severe leg cramping during gym class with episodes of dark urine after intense activity, and improvement of symptoms after continuing to exercise at lower intensity.

(a) Propose the most likely diagnosis for each child and identify the deficient enzyme in each case.

(b) An ischemic forearm exercise test is performed on both children and on a control. In the control, venous lactate rises threefold and ammonia rises twofold. In Child A, lactate rises threefold and ammonia rises twofold. In Child B, lactate does not rise but ammonia rises normally. Explain this pattern for each child. What does Child A's normal lactate rise tell you about the location of the metabolic defect?

(c) Child B's father reports that as a young athlete he had several episodes of dark urine after intense sports in his 20s, but he has had no symptoms in his 40s and exercises only at low intensity now. Why might his symptoms have become less prominent as he aged and reduced his exercise intensity, given that his enzyme deficiency has not changed?

---

**Problem 8.** *(Synthesis)*
A researcher treats isolated hepatocytes with a drug that constitutively activates phosphodiesterase (the enzyme that degrades cAMP).

(a) Predict the phosphorylation state of glycogen phosphorylase and glycogen synthase in these cells after 10 minutes. Trace your reasoning through the signaling cascade.

(b) What would you expect to happen to glycogen content in these cells over the subsequent hour? Explain.

(c) The researcher then adds glucagon at 1000-fold the normal physiological concentration to these drug-treated cells. Would you expect a glycogenolytic response? Explain why or why not.

---

## References

1. Roach PJ, Depaoli-Roach AA, Hurley TD, Tagliabracci VS. Glycogen and its metabolism: some new developments and old themes. Biochem J. 2012;441(3):763-787.

2. Chou JY, Jun HS, Mansfield BC. Glycogen storage disease type I and G6Pase-β deficiency: etiology and therapy. Nat Rev Endocrinol. 2010;6(12):676-688.

3. Kishnani PS, Steiner RD, Bali D, et al. Pompe disease diagnosis and management guideline. Genet Med. 2006;8(5):267-288.

4. Vissing J. McArdle disease. Curr Neurol Neurosci Rep. 2014;14(10):489.

5. Greenberg CC, Jurczak MJ, Danos AM, Brady MJ. Glycogen branches out: new perspectives on the role of glycogen metabolism in the integration of metabolic pathways. Am J Physiol Endocrinol Metab. 2006;291(1):E1-8.

6. Johnson LN. Glycogen phosphorylase: control by phosphorylation and allosteric effectors. FASEB J. 1992;6(6):2274-2282.

7. Preisler N, Vissing J. Exercise-related problems in McArdle disease. J Inherit Metab Dis. 2015;38(3):545-552.

8. Arabshahi A, Ruzicka FJ, Geeganage S, Frey PA. Standard free energies for uridylyl group transfer by hexose-1-P uridylyltransferase and UDP-hexose synthase and for the hydrolysis of uridine 5'-phosphoimidazolate. Biochemistry. 1996;35(11):3426-3428.
