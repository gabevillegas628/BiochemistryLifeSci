# Chapter 8: Signal Transduction

---

## Opener Questions

Think about these before you read. Come back to them at the end and see if your answer changed.

1. A 45-year-old man returns from a week in rural Bangladesh with profuse, painless, watery diarrhea described as "rice-water stools." He is severely dehydrated despite drinking fluids steadily. Blood cultures are negative. Stool culture grows a curved gram-negative rod. The diarrhea is not due to mucosal invasion or inflammation; biopsies of his intestinal epithelium look normal. The epithelial cells are secreting chloride ions at an uncontrollable rate. What molecular event is driving that secretion, and why can't the cell turn it off?

2. A 67-year-old woman is found to have a 2.8 cm mass in the head of the pancreas. Biopsy confirms pancreatic adenocarcinoma. Genetic sequencing of the tumor reveals a point mutation in codon 12 of the KRAS gene, converting glycine to valine. This mutation is found in over 90% of pancreatic adenocarcinomas. The protein product of KRAS is a GTPase that functions as a molecular switch. How does a single amino acid substitution that impairs GTPase activity lead to uncontrolled cell proliferation?

---

## The Big Picture

A cell inside your body cannot see the outside world. It cannot directly sense that blood glucose is rising after a meal, that a pathogen has breached the skin, that a developing limb bud needs more cells in one region, or that stress hormones are flooding the bloodstream. It is surrounded by a lipid bilayer that, as Chapter 6 established, is an excellent barrier. Signals arrive at the surface of that barrier as molecules, not as text.

Signal transduction is the process by which a chemical signal on the outside of the membrane produces a specific biological response on the inside. The signal itself almost never crosses the membrane. A molecule of epinephrine does not enter the cell and find the enzyme it wants to activate. Instead, it binds a receptor on the outer face of the membrane, that receptor changes shape, and that shape change initiates a cascade of molecular events that amplifies and transmits the signal to its targets inside the cell. The signal is converted, or transduced, from one form to another.

This chapter covers the two major signaling architectures that underlie most of clinical pharmacology: **G protein-coupled receptors (GPCRs)**, which transduce signals through small diffusible messenger molecules, and **receptor tyrosine kinases (RTKs)**, which transduce signals through cascading phosphorylation events. Both systems share a common logic: a ligand binds outside, a conformational change propagates across the membrane, and a molecular switch inside the cell flips from off to on, triggering amplification of the original signal.

The two clinical anchors for this chapter both illustrate the same underlying failure mode, but reach it by completely different routes. In one, a bacterial toxin produces a defect so precise that a single signaling protein in intestinal epithelial cells cannot stop doing its job, with consequences measured in liters of fluid loss per hour. In the other, a single amino acid substitution converts a GTPase that is supposed to shut itself off into one that cannot, and the result drives over 90% of pancreatic cancers and roughly 30% of all human malignancies. The pathology in both cases is not too much signal arriving from outside. It is a signal already inside the cell that has lost the ability to stop. That distinction is the point of this chapter.

---

## Why Cells Need Signals

Multicellular life requires coordination. A liver cell deciding whether to break down glycogen must know what blood glucose looks like right now, not what it looked like when the cell last divided. A T cell deciding whether to proliferate must know whether an antigen-presenting cell is signaling danger nearby. A cardiac myocyte must know when to contract and by how much.

The signaling molecules themselves are diverse: proteins and peptides (insulin, glucagon, growth factors), amino acid derivatives (epinephrine, thyroid hormone), lipids (steroid hormones, prostaglandins), and gases (nitric oxide). What they have in common is that they carry information. Their concentration at any moment encodes a message about the *state of the organism*.

Cells interpret these messages through **receptors**: proteins that bind a specific signaling molecule with high affinity and low promiscuity, and convert that binding event into a change in cellular behavior. The receptor is both the antenna (it detects the signal) and the first transducer (it converts the signal into intracellular language).

The core challenge is physical. Most signaling molecules are polar or charged. They cannot cross the bilayer without a transporter. The cell's solution is to keep most signals outside and build reception machinery into the membrane surface itself. The receptor spans the membrane; the ligand binds the extracellular face; the conformational change propagates to the intracellular face where the actual biochemistry happens.

Three receptor architectures dominate this chapter:

1. **G protein-coupled receptors (GPCRs):** Seven-transmembrane-helix (7TM) receptors coupled to heterotrimeric G proteins inside the cell. G proteins are named for the guanine nucleotides they bind: GTP switches them on, GDP switches them off. The receptor's job is to trigger that exchange; the G protein's job is to carry the signal forward until it hydrolyzes its own GTP and shuts itself down.

2. **Receptor tyrosine kinases (RTKs):** Single-pass transmembrane receptors with an extracellular ligand-binding domain and an intracellular kinase domain. Ligand binding activates the receptor dimer — either by inducing two monomers to come together or by reorienting a constitutive dimer — and the two kinase domains cross-phosphorylate each other, creating docking sites for downstream signaling proteins.

3. **Nuclear receptors:** Intracellular receptors for lipid-soluble ligands (steroid hormones, thyroid hormone, retinoic acid) that act directly as transcription factors. Because their ligands can cross the membrane, the receptor does not need to be at the surface. Covered briefly at the end of this chapter.

---

## G Protein-Coupled Receptors

### Structure and the Seven-Helix Architecture

GPCRs are the largest family of cell-surface receptors in the human genome: roughly 800 genes encode them. They detect an extraordinary range of stimuli, from photons (rhodopsin in rod cells) to odorants (olfactory receptors) to hormones (the $\beta$-adrenergic receptor that epinephrine binds) to neurotransmitters (muscarinic acetylcholine receptors in the heart).

Despite this diversity of ligands, all GPCRs share the same basic architecture: a single polypeptide chain that crosses the membrane seven times as $\alpha$-helices. The seven helices pack together in a bundle, with the extracellular surface presenting a binding pocket for the ligand and the intracellular surface presenting a docking surface for the G protein. The extracellular loops that connect the helices help form the ligand-binding site; the intracellular loops, particularly the third one, contact the G protein directly.

When no ligand is bound, the receptor is in a low-activity conformation. The ligand-binding pocket is accessible but unoccupied. When the agonist binds, it stabilizes a different conformational state of the helix bundle, one in which the intracellular face of the receptor has a distinctly different shape. That shape change is what allows the G protein to bind and be activated.

### The G Protein: A Molecular Switch

The **heterotrimeric G protein** is a three-subunit complex: $\text{G}_\alpha$, $\text{G}_\beta$, and $\text{G}_\gamma$. The $\beta$ and $\gamma$ subunits are tightly associated and function as a unit ($\text{G}_{\beta\gamma}$). The key player for the on/off switch is $\text{G}_\alpha$, and the switch logic is simple: $\text{G}_\alpha$ bound to GDP is off; $\text{G}_\alpha$ bound to GTP is on.

In the resting state, $\text{G}_\alpha$-GDP is associated with $\text{G}_{\beta\gamma}$ and the whole complex sits at the inner face of the plasma membrane, loosely coupled to the receptor. The three subunits together keep each other inactive. When an agonist-bound receptor contacts $\text{G}_\alpha$, it acts as a **guanine nucleotide exchange factor (GEF)**: it catalyzes the release of GDP from $\text{G}_\alpha$. GTP binds in its place (GTP is abundant in the cytoplasm), and $\text{G}_\alpha$-GTP undergoes a conformational change that causes it to dissociate from both the receptor and $\text{G}_{\beta\gamma}$.

The $\text{G}_{\alpha\beta\gamma}$ complex is held at the membrane by covalent lipid modifications on $\text{G}_\alpha$ and $\text{G}_\gamma$ (see Chapter 6) — neither is a transmembrane protein, but both are tethered to the inner leaflet by lipid tails. So when $\text{G}_\alpha$-GTP dissociates from the receptor, it does not drift into the cytoplasm; it slides laterally along the inner leaflet until it finds its downstream target, called the **effector**. The freed $\text{G}_{\beta\gamma}$ dimer, also still membrane-associated, has effector targets of its own.

The signal terminates by an intrinsic mechanism built into $\text{G}_\alpha$ itself: it is a **GTPase**. $\text{G}_\alpha$-GTP slowly hydrolyzes its own bound GTP to GDP, producing $\text{G}_\alpha$-GDP. Once GDP replaces GTP, $\text{G}_\alpha$ returns to its off conformation, reassociates with $\text{G}_{\beta\gamma}$, and the complex docks back at the receptor, ready for the next round.

The GTPase activity of $\text{G}_\alpha$ is the built-in timer of this system. The duration of signaling is determined by how long GTP remains bound, which is determined by the hydrolysis rate. This is not a trivial design choice. A signal that cannot turn itself off is pathological. Cholera toxin, as we will see, exploits exactly this point.

### The cAMP Pathway: $\text{G}_s$ and Adenylyl Cyclase

Different G protein subtypes couple to different effectors. The best-studied pathway uses $\text{G}_s$ (the "s" stands for stimulatory) and its effector, **adenylyl cyclase**.

Adenylyl cyclase is an enzyme embedded in the plasma membrane. Its substrate is ATP. When activated by $\text{G}_{\alpha s}$-GTP, it converts ATP to **cyclic AMP (cAMP)** and inorganic pyrophosphate ($\text{PP}_i$):

$$\text{ATP} \xrightarrow{\text{adenylyl cyclase}} \text{cAMP} + \text{PP}_i$$

Pyrophosphate does not accumulate. It is immediately cleaved by **inorganic pyrophosphatase**, a ubiquitous enzyme, into two inorganic phosphates:

$$\text{PP}_i \xrightarrow{\text{pyrophosphatase}} 2\,\text{P}_i$$

This second reaction is highly favorable, and its coupling to the first is a recurring strategy in biochemistry. The adenylyl cyclase reaction on its own is only modestly favorable. But by immediately consuming its product ($\text{PP}_i$), the cell pulls the equilibrium far to the right — the cAMP synthesis reaction becomes effectively irreversible. You will see this pattern repeatedly in metabolism: whenever a biosynthetic reaction releases pyrophosphate, rapid hydrolysis of that pyrophosphate is what commits the reaction to completion. The cell is not just making cAMP; it is spending two phosphate bonds' worth of driving force to ensure that cAMP production cannot easily reverse.

cAMP is a **second messenger**: a small, diffusible intracellular signal molecule generated in response to the extracellular first messenger (the hormone). The cell produces it rapidly in large quantities and degrades it rapidly (by **phosphodiesterase**, which hydrolyzes cAMP to 5'-AMP) when signaling needs to stop. The ratio of production to degradation sets the intracellular cAMP concentration at any moment.

cAMP's primary target in most cells is **protein kinase A (PKA)**, also called cAMP-dependent protein kinase. In the absence of cAMP, PKA is a heterotetramer: two regulatory (R) subunits and two catalytic (C) subunits. The R subunits block the active sites of the C subunits. When cAMP concentrations rise, two cAMP molecules bind each R subunit, causing the R subunits to release the C subunits. The free catalytic subunits are now active: they phosphorylate serine and threonine residues on downstream target proteins (of which there are dozens), altering their activity.

This architecture produces **signal amplification** at multiple steps:

- One hormone molecule activates one receptor.
- One receptor, while occupied by hormone, activates many G protein molecules (the receptor is a catalyst for the GEF reaction; it can activate G proteins repeatedly as long as hormone is bound).
- Each $\text{G}_{\alpha s}$-GTP activates one adenylyl cyclase molecule, but that enzyme rapidly synthesizes many cAMP molecules.
- cAMP activates PKA, which phosphorylates many substrate molecules per second.

A single epinephrine molecule binding a $\beta$-adrenergic receptor in a liver cell can ultimately activate millions of glycogen phosphorylase molecules within seconds. That is the power of a cascade, its amplification effect.

### The $\text{G}_i$ Pathway: Inhibitory Signaling

Not all GPCR signaling is stimulatory. $\text{G}_i$ (inhibitory) couples the receptor to adenylyl cyclase, but in the opposite direction: $\text{G}_{\alpha i}$-GTP inhibits adenylyl cyclase, reducing cAMP production.

The physiological logic becomes clear in the heart. The $\beta$-adrenergic receptor (activated by epinephrine) uses $\text{G}_s$ to increase cAMP in cardiac myocytes, which increases heart rate and contractility. The muscarinic acetylcholine receptor (activated by the vagus nerve) uses $\text{G}_i$ to decrease cAMP in the same cells, slowing heart rate. Two inputs, opposing outputs, same second messenger. The cell integrates both signals by summing the rates of cAMP synthesis and degradation.

Pertussis toxin, from Bordetella pertussis (whooping cough), permanently activates $\text{G}_i$ by ADP-ribosylating the $\text{G}_{\alpha i}$ subunit in a way that prevents GDP release. With $\text{G}_i$ locked in its GDP-bound off state, the inhibitory brake on adenylyl cyclase is removed. In airway epithelial cells, this contributes to the excessive mucus secretion and impaired ciliary clearance characteristic of whooping cough.

### The $\text{G}_q$ Pathway: Phospholipase C, IP3, and DAG

A third major arm uses $\text{G}_q$, which activates **phospholipase C (PLC)**, an enzyme that cleaves the membrane phospholipid phosphatidylinositol 4,5-bisphosphate ($\text{PIP}_2$) into two products:

1. **Inositol trisphosphate ($\text{IP}_3$):** A soluble second messenger released into the cytoplasm. $\text{IP}_3$ diffuses to the endoplasmic reticulum, where it binds $\text{IP}_3$ receptors (ligand-gated calcium channels). These channels open, releasing $\text{Ca}^{2+}$ from the ER lumen into the cytoplasm. The rise in cytoplasmic $\text{Ca}^{2+}$ activates many downstream targets, including the $\text{Ca}^{2+}$-binding protein calmodulin, which in turn activates calmodulin-dependent kinases.

2. **Diacylglycerol (DAG):** Remains in the membrane. Together with $\text{Ca}^{2+}$, DAG activates **protein kinase C (PKC)**, a serine/threonine kinase with broad substrate specificity and roles in cell proliferation, differentiation, and survival.

This pathway is used by vasopressin (to drive water reabsorption in the kidney), thrombin (to trigger platelet aggregation), and many neurotransmitters. The simultaneous release of two second messengers from one PLC cleavage event is an elegant design: $\text{IP}_3$ mobilizes calcium from a stored pool without waiting for extracellular calcium to enter, and DAG stays membrane-associated to recruit and activate PKC there.

### Terminating the GPCR Signal

Activating a receptor is only half the problem. A signal that cannot be turned off is as dangerous as no signal at all. The cholera case makes that point forcefully. Termination of GPCR signaling happens at every level of the cascade, and the mechanisms are worth knowing because they are the targets of a large fraction of clinical pharmacology.

**At the ligand level:** The simplest shutoff is hormone dissociation. When epinephrine leaves the $\beta$-adrenergic receptor, the receptor returns to its inactive conformation and stops activating $\text{G}_s$. No hormone, no signal. How long the hormone stays bound is determined by the receptor's affinity for it: the $K_d$ from Chapter 3, which reflects the ratio of the off-rate to the on-rate. A receptor with a low $K_d$ holds its ligand tightly and signals for longer; a receptor with a high $K_d$ releases its ligand quickly and signals briefly. This is why the duration of a hormonal response partly reflects how long the hormone persists in circulation, and why adrenaline responses are short-lived while steroid hormone effects last hours.

**At the receptor level:** Prolonged or repeated stimulation triggers **desensitization**, a process that reduces the receptor's ability to signal even while hormone is still present. The key players are **G protein-coupled receptor kinases (GRKs)**, which phosphorylate serine and threonine residues on the intracellular loops and C-terminus of the activated receptor. This phosphorylation does two things. It directly reduces the receptor's affinity for $\text{G}_\alpha$. More importantly, it creates docking sites for **$\beta$-arrestin**.

$\beta$-arrestin binding physically occludes the $\text{G}_\alpha$ docking surface and prevents any further G protein activation; this is the primary desensitization mechanism. But $\beta$-arrestin does more than just block. It also acts as a scaffold that recruits clathrin and adaptor proteins to the receptor, targeting it for endocytosis and pulling it off the membrane entirely. The receptor is internalized in a clathrin-coated vesicle and either recycled back to the surface (resensitization) or degraded (downregulation). Long-term exposure to a drug or hormone can deplete the surface receptor pool entirely, which is one molecular basis for drug tolerance.

**At the second messenger level:** Once $\text{G}_\alpha$ has dissociated from the receptor, its intrinsic GTPase activity terminates its own signal as described above. But the second messengers it generated must also be cleared. cAMP is hydrolyzed to inactive 5'-AMP by **phosphodiesterase (PDE)**, the enzyme that caffeine and theophylline inhibit, which is why those compounds amplify and prolong cAMP-dependent signaling. $\text{IP}_3$ is rapidly dephosphorylated by specific phosphatases. Cytoplasmic $\text{Ca}^{2+}$ is pumped back into the ER by SERCA pumps (Chapter 7) and extruded from the cell by plasma membrane calcium ATPases. These degradation and clearance steps are not passive decay; they are active processes that set the duration of the downstream signal.

Termination is layered: ligand, receptor, G protein, and second messenger are all cleared independently, giving the cell multiple brakes operating in parallel. Losing any one of them individually tends to prolong rather than abolish signaling, which is why loss-of-termination mutations are generally gain-of-function phenotypes, and why so many disease states involve failure of one of these checkpoints rather than failure of the signal itself.

---

## Receptor Tyrosine Kinases

### Structure and Activation

The second major signaling architecture uses a completely different mechanism. **Receptor tyrosine kinases (RTKs)** are single-pass transmembrane proteins with three domains: an extracellular ligand-binding domain, a single transmembrane helix, and an intracellular kinase domain.

The kinase domain is the active component. It catalyzes the transfer of the terminal phosphate of ATP to the hydroxyl group of tyrosine residues on substrate proteins. In the resting state, the kinase domain is inactive.

Activation requires the two kinase domains to be brought into the correct proximity and orientation, which is achieved through **dimerization**. For receptors that exist as monomers at rest, the ligand drives this directly: it bridges two monomers, forcing them together. Some ligands are themselves dimers and bring two receptor monomers together directly; others bind one receptor and induce a conformational change that exposes a dimerization interface. For receptors that are constitutive dimers (the insulin receptor being the key example), the two subunits are already joined by disulfide bonds and ligand binding instead reorients the dimer into an active configuration. In both cases the result is the same: two kinase domains held in proximity, poised to activate each other.

Once two kinase domains are held in proximity, each one phosphorylates its partner. The key target is a tyrosine residue within a stretch of the kinase domain called the **activation loop**. In the unphosphorylated, resting state, this loop folds directly into the active site cleft and physically blocks it, preventing substrate proteins from entering. The kinase is inactive not because it lacks catalytic machinery, but because its own activation loop is sitting in the way.

When dimerization brings two kinase domains face to face, each kinase can reach the activation loop of its partner. That activation loop tyrosine is the one target accessible even in the inactive conformation, because it is already positioned near the catalytic residues rather than having to compete for entry into a blocked active site. Each kinase phosphorylates the other's activation loop tyrosine in what is called **trans-autophosphorylation**: trans because it is across (kinase A phosphorylates kinase B, not itself), auto because it is the same type of protein phosphorylating itself as a class.

Once the activation loop tyrosine is phosphorylated, the negatively charged phosphate group destabilizes the loop's position in the active site and it swings out, opening the catalytic cleft to external substrates. The activated kinase then phosphorylates additional tyrosine residues in the intracellular tail of the receptor, creating the docking sites that recruit downstream signaling proteins.

These phosphotyrosine residues serve as docking sites. Intracellular signaling proteins that contain **SH2 domains** (Src Homology 2 domains) or PTB domains recognize and bind specific phosphotyrosine-containing sequences. Different phosphorylation sites recruit different downstream proteins, which is how one RTK can simultaneously activate multiple parallel signaling pathways.

### Ras: The GTPase Switch of RTK Signaling

The most important immediate downstream target of many RTKs is **Ras**, a small GTPase that functions by the same switch logic as the $\text{G}_\alpha$ subunits described above: Ras-GDP is off, Ras-GTP is on.

Ras is not a transmembrane protein. It is a small protein (21 kDa) anchored to the inner leaflet of the plasma membrane by a lipid modification. The connection between the RTK and Ras involves two adapter proteins:

1. **Grb2:** An adapter protein with an SH2 domain that binds a specific phosphotyrosine on the activated RTK, and two SH3 domains that constitutively bind a proline-rich sequence on a second adapter, Sos.

2. **Sos:** A guanine nucleotide exchange factor (GEF) for Ras. When Grb2 brings Sos to the membrane (where Ras lives), Sos catalyzes the exchange of GDP for GTP on Ras, converting it to the active Ras-GTP form.

The chain of events is: ligand binds RTK $\rightarrow$ receptor dimerizes and autophosphorylates $\rightarrow$ Grb2-Sos complex is recruited to the phosphorylated receptor $\rightarrow$ Sos activates Ras by catalyzing GDP-to-GTP exchange $\rightarrow$ Ras-GTP activates downstream kinase cascades.

Ras terminates its own signal by hydrolyzing GTP to GDP, returning to the Ras-GDP off state. But unlike $\text{G}_\alpha$, Ras has very weak intrinsic GTPase activity. It requires a **GTPase-activating protein (GAP)** to accelerate hydrolysis to a physiologically useful rate. The GEF activity of SOS drives the on transition; the GAP drives the off transition.

### The MAPK Cascade

Ras-GTP activates a three-kinase amplification cascade:

$$\text{Ras-GTP} \rightarrow \text{Raf} \rightarrow \text{MEK} \rightarrow \text{ERK}$$

Ras-GTP recruits and activates **Raf** (a serine/threonine kinase) at the membrane. Active Raf phosphorylates and activates **MEK** (a dual-specificity kinase that phosphorylates both serine/threonine and tyrosine residues). Active MEK phosphorylates and activates **ERK** (extracellular signal-regulated kinase). Active ERK can phosphorylate substrates in the cytoplasm, and some ERK molecules translocate into the nucleus, where they phosphorylate transcription factors that drive expression of genes controlling cell growth and division.

The cascade structure produces massive amplification. One activated Ras molecule can activate multiple Raf molecules; each Raf molecule activates multiple MEK molecules; each MEK molecule activates multiple ERK molecules. A single growth factor molecule binding at the surface can produce a flood of activated ERK inside the cell within minutes.

This is the pathway that drives cell proliferation in response to growth factors and is the primary downstream arm of EGFR-family receptors. It is also the pathway hijacked in approximately 30% of all human cancers, overwhelmingly through mutations in Ras. But Ras/MAPK is not the only output RTKs produce. A second major downstream arm, used by a different receptor in response to a different metabolic question, reaches completely different targets.

### The Insulin Receptor and the PI3K/Akt Pathway

The insulin receptor is the RTK the body uses to answer the question: is there fuel available right now? When blood glucose rises after a meal, the pancreas releases insulin. Insulin binds the receptor's extracellular subunits, triggers the conformational change and trans-autophosphorylation described above, and the activated kinase domains phosphorylate a set of intracellular docking proteins called **insulin receptor substrates (IRS proteins)**, primarily IRS-1.

IRS-1 is not a kinase and it is not Grb2. It is a large scaffolding protein with no intrinsic enzymatic activity. Its job is to collect the phosphorylation signal from the receptor and relay it to a specific effector: **phosphoinositide 3-kinase (PI3K)**. PI3K has an SH2 domain that binds the phosphotyrosine residues on IRS-1, bringing it to the membrane. Once there, PI3K phosphorylates the membrane lipid phosphatidylinositol 4,5-bisphosphate ($\text{PIP}_2$) at the 3-position of the inositol ring, producing phosphatidylinositol 3,4,5-trisphosphate ($\text{PIP}_3$):

$$\text{PIP}_2 \xrightarrow{\text{PI3K}} \text{PIP}_3$$

$\text{PIP}_3$ is a lipid second messenger that stays embedded in the inner leaflet of the membrane. It serves as a landing platform. Two kinases that carry a **pleckstrin homology (PH) domain** recognize $\text{PIP}_3$ and are recruited to the membrane together: **Akt** (also called PKB, protein kinase B) and $\text{PIP}_3$ dependent kinase **PDK1**. PDK1 phosphorylates and activates Akt. Active Akt then phosphorylates a wide range of targets that collectively shift cellular metabolism toward fuel storage and growth:

- **GLUT4 translocation:** Akt phosphorylates a GTPase-activating protein called AS160, which normally holds GLUT4 vesicles tethered in the cytoplasm by keeping the Rab GTPases that control vesicle docking in their inactive GDP-bound state. Phosphorylation of AS160 releases the tether, and GLUT4 vesicles fuse with the plasma membrane, dramatically increasing glucose uptake into muscle and fat cells. This is the primary mechanism by which insulin lowers blood glucose, and failure of this step is the central functional defect producing hyperglycemia in type 2 diabetes (see below).
- **Glycogen synthesis:** Akt phosphorylates and inactivates glycogen synthase kinase-3 (GSK-3), which normally phosphorylates and inhibits glycogen synthase. By shutting off the inhibitor's inhibitor, Akt promotes glycogen synthesis.
- **mTOR activation:** Akt activates the mTOR complex, a master regulator of protein synthesis and cell growth. This connects nutrient availability to anabolic signaling.
- **Gluconeogenesis suppression:** Akt phosphorylates FOXO transcription factors, excluding them from the nucleus and suppressing expression of gluconeogenic enzymes in the liver.

Termination of PI3K/Akt signaling depends critically on the lipid phosphatase **PTEN**, which removes the 3-phosphate from $\text{PIP}_3$, converting it back to $\text{PIP}_2$ and depleting the membrane landing platform for Akt. PTEN is one of the most commonly mutated tumor suppressor genes in human cancer: loss of PTEN means $\text{PIP}_3$ accumulates constitutively, Akt is permanently active, and cells grow without the normal metabolic controls. The parallel to oncogenic Ras mutation is exact: one pathway produces constitutive proliferative signaling by locking a GTPase on; the other does it by removing the phosphatase that clears the lipid second messenger.

**When the insulin receptor pathway fails: type 2 diabetes and insulin resistance**

In type 2 diabetes, the insulin receptor itself is usually intact and insulin is present, often in excess. The failure is downstream, at IRS-1. In the setting of chronic overnutrition and obesity, adipose tissue and the liver release elevated levels of free fatty acids and inflammatory cytokines such as TNF-$\alpha$ and IL-6. These signals activate inflammatory kinases inside insulin-target cells, particularly JNK and IKK. These kinases phosphorylate IRS-1 on serine residues.

This matters because the insulin receptor communicates with IRS-1 through tyrosine phosphorylation. Serine phosphorylation of IRS-1 by the inflammatory kinases physically interferes with the receptor's ability to phosphorylate IRS-1 on tyrosine. The result is that insulin binds the receptor, the receptor activates, the kinase domains are active and ready to signal, but IRS-1 cannot receive the signal. PI3K is never recruited. $\text{PIP}_3$ does not accumulate. Akt does not translocate. GLUT4 stays tethered in the cytoplasm. Blood glucose does not fall despite rising insulin levels. The cell is not incapable of responding to insulin in principle; it has been specifically disconnected from the signal at one molecular node.

This reframes type 2 diabetes as a signaling disease rather than simply a metabolic one. The treatment logic follows directly: if the problem is inflammatory kinase activity blocking IRS-1, then reducing the inflammatory stimulus (weight loss, exercise) or enhancing downstream Akt activity by other means (metformin activates AMPK, which has converging effects on glucose metabolism) can partially restore the signal without fixing the receptor itself.

---

## When It Breaks

### Cholera: The G Protein Stuck On

*Vibrio cholerae* causes cholera not by invading intestinal epithelial cells but by releasing a toxin that permanently activates the G protein that drives chloride secretion.

Intestinal epithelial cells normally control fluid secretion partly through the CFTR chloride channel (Chapter 7). One of the signals that drives CFTR opening is cAMP, which activates PKA, which phosphorylates CFTR and keeps it open. This pathway is normally regulated: when the signaling molecule (VIP, vasoactive intestinal peptide) is no longer present, the G protein turns off, adenylyl cyclase returns to basal activity, phosphodiesterase degrades cAMP, PKA is inactivated, and CFTR closes.

Cholera toxin is taken up by intestinal epithelial cells and delivers an enzymatic subunit into the cytoplasm. That subunit has one job: it catalyzes the **ADP-ribosylation** of $\text{G}_{\alpha s}$. ADP-ribosylation is the covalent attachment of an ADP-ribose group, cleaved from $\text{NAD}^+$, onto a residue of the target protein. The modification adds a bulky, negatively charged group that physically blocks the GTPase active site, preventing GTP hydrolysis. With GTP hydrolysis blocked, $\text{G}_{\alpha s}$ cannot return to the GDP-bound off state. It remains permanently active, permanently driving adenylyl cyclase, permanently flooding the cell with cAMP.

With cAMP continuously elevated, PKA is permanently active. PKA phosphorylates CFTR, holding it open. CFTR pumps chloride continuously into the intestinal lumen. Sodium follows chloride into the lumen, drawn by the charge imbalance. Water follows them both, drawn by the resulting osmotic gradient. The intestine cannot absorb fluid fast enough to keep pace with this chloride-driven secretion. The result is up to 20 liters per day of isotonic fluid loss, with the characteristic rice-water appearance (mucus and epithelial cells suspended in clear isotonic fluid, not blood, because the mucosa is not inflamed or invaded).

Death from untreated cholera is death from dehydration and electrolyte imbalance, not from infection per se. Oral rehydration therapy works by exploiting a separate sodium-glucose cotransporter (SGLT1) that does not require cAMP signaling and remains functional. Glucose in the oral rehydration solution drives sodium absorption through SGLT1, and water follows. The cAMP machinery is still locked on, but this parallel pathway compensates.

The toxin is also a teaching tool. Because cholera toxin specifically locks $\text{G}_{\alpha s}$-GTP in place, it is used in research to permanently activate cAMP signaling in cell culture systems. Pertussis toxin does the same to $\text{G}_{\alpha i}$, but from the other direction: it locks $\text{G}_{\alpha i}$ in the GDP-bound off state, preventing inhibitory signaling and effectively removing the brake on adenylyl cyclase.

### Oncogenic Ras: The GTPase Switch Stuck On

Recall that Ras turns itself off by hydrolyzing GTP to GDP. The intrinsic hydrolysis rate is slow; the GAP protein **NF1 (neurofibromin)** dramatically accelerates it by supplying a catalytic arginine residue to the active site of Ras, stabilizing the transition state for hydrolysis.

The most common Ras mutations in cancer are point mutations at codon 12 (glycine to valine or aspartate) and codon 13 (glycine to aspartate). The glycine at position 12 sits in the P-loop of the GTPase domain, adjacent to the catalytic water molecule and in direct contact with the attacking arginine of the GAP protein. Substituting valine or aspartate at this position creates steric clash: the bulkier side chain prevents the GAP's arginine from entering the active site in the correct geometry. The intrinsic hydrolysis rate of Ras is already very slow; without GAP assistance, it becomes negligibly slow. Ras remains GTP-bound and active essentially indefinitely.

A cell expressing oncogenic Ras-G12V behaves as though growth factor receptors are permanently activated. Raf is constitutively active. MEK is constitutively active. ERK is constitutively active. The transcription factors driving cell division are always on. The cell proliferates without needing growth factor signals.

KRAS mutations (a specific Ras isoform encoded by the KRAS gene) are found in over 90% of pancreatic adenocarcinomas, approximately 45% of colorectal cancers, and roughly 30% of lung adenocarcinomas. KRAS-G12D (glycine to aspartate) is the single most common driver mutation in human cancer. For decades, oncogenic Ras was considered "undruggable" because the protein has no obvious pocket for a small molecule to bind. Recent work has found inhibitors that specifically target the KRAS-G12C variant (cysteine, in lung cancer) by covalently occupying a pocket that only exists when Ras is in the GDP-bound off state, trapping it there. This represents one of the most significant advances in targeted oncology in years.

---

## Nuclear Receptors: Lipid-Soluble Signals Cross the Membrane

Not all signals require cell-surface receptors. Lipid-soluble ligands, specifically steroid hormones (cortisol, aldosterone, estrogen, testosterone, progesterone), thyroid hormone, vitamin D, and retinoic acid, can diffuse across the bilayer and bind intracellular receptors.

**Nuclear receptors** are transcription factors that are inactive until bound by their ligand. In the unliganded state, many nuclear receptors are held in the cytoplasm by chaperone complexes or are bound to DNA but associated with corepressor complexes that silence gene expression. Ligand binding causes a conformational change in the ligand-binding domain that releases the chaperones or exchanges corepressors for coactivators. The activated receptor (or receptor-ligand complex) either translocates to the nucleus or changes its activity if already there, binding specific DNA sequences called **hormone response elements (HREs)** and driving transcription of target genes.

The response is slower than GPCR or RTK signaling (hours rather than seconds to minutes) because the output is altered gene expression rather than enzyme phosphorylation. But the effects are more sustained and can fundamentally reprogram cell behavior.

Glucocorticoids (cortisol and synthetic analogs like prednisone) act through glucocorticoid receptors (GRs). Unliganded GR is sequestered in the cytoplasm by heat shock proteins. Cortisol binding causes the heat shock proteins to dissociate; the GR-cortisol complex translocates into the nucleus and regulates hundreds of genes involved in inflammation, metabolism, and immune function. This mechanism underlies both the therapeutic effects of corticosteroids (suppressing inflammation) and their side effects at high doses (hyperglycemia, immunosuppression, osteoporosis, adrenal insufficiency).

---

## Signal Integration and Termination

A cell is not a machine that executes one signal at a time. At any moment, a cell is receiving dozens of different signals simultaneously. The signaling pathways described above do not operate in isolation: they crosstalk, converge, and inhibit each other. PKA phosphorylates substrates that affect RTK signaling. ERK phosphorylates and inhibits upstream components of its own pathway (negative feedback). $\text{Ca}^{2+}$ released by the $\text{G}_q$ pathway modulates ion channels that affect membrane potential, which in turn affects voltage-gated calcium channels.

The outcome is integration: the cell's behavioral response reflects the sum and product of all incoming signals, not just the loudest one.

Equally important is termination. Every step in every signaling pathway must be reversible:

- **Receptor inactivation:** Agonist-bound GPCRs are phosphorylated by G protein-coupled receptor kinases (GRKs) on their intracellular loops, reducing their ability to activate G proteins. Arrestin then binds the phosphorylated receptor, further blocking G protein coupling and targeting the receptor for endocytosis. This is the mechanism of **desensitization**: the cell becomes less responsive to prolonged stimulation.

- **G protein self-termination:** $\text{G}_{\alpha}$-GTP hydrolyzes GTP to GDP, terminating its own activity. Regulators of G protein signaling (RGS proteins) accelerate this hydrolysis.

- **Second messenger degradation:** Phosphodiesterase hydrolyzes cAMP; IP3 is dephosphorylated by phosphatases; calcium is pumped back into the ER by SERCA pumps (Chapter 7) and out of the cell by plasma membrane calcium ATPases.

- **Phosphatase action:** Every phosphorylation event in the RTK/Ras/MAPK cascade is reversed by specific phosphatases. Protein tyrosine phosphatases (PTPs) remove phosphate from tyrosine residues. The phosphatase PTEN removes the phosphate from the lipid second messenger $\text{PIP}_3$, terminating PI3K signaling (a pathway downstream of RTKs not covered in detail here, but critical for insulin signaling and cancer).

Loss of termination mechanisms is as pathogenic as constitutive activation. Mutations in PTEN are among the most common in human cancer. Loss of NF1 (the Ras GAP) causes neurofibromatosis, characterized by benign nerve sheath tumors driven by constitutive Ras activation in the absence of mutations in Ras itself.

---

## The MCAT Angle

Signal transduction appears on the MCAT primarily in two contexts: receptor pharmacology (agonists, antagonists, and what happens downstream) and cellular responses to hormones and growth factors. The reasoning pattern is always the same: identify the receptor type, trace the signal through the cascade, and predict what happens when you add, remove, or mutate a component.

**GPCR pharmacology questions** typically present a drug or hormone and ask you to trace the downstream effect. Know which receptor subtypes ($\text{G}_s$, $\text{G}_i$, $\text{G}_q$) couple to which second messengers (cAMP up, cAMP down, IP3/DAG/Ca$^{2+}$) and which downstream kinase (PKA, PKC). Know that cAMP activates PKA, which phosphorylates its targets. Know that epinephrine on $\beta$-adrenergic receptors raises cAMP; epinephrine on $\alpha_2$-adrenergic receptors lowers cAMP (via $\text{G}_i$). Know that the heart speeds up with $\beta$-stimulation and slows down with muscarinic stimulation, and that both effects converge on cAMP in cardiac myocytes.

**The GTPase switch logic** is heavily tested. Both G proteins and Ras are GTP/GDP switches. Both are activated by GEFs (which promote GTP loading) and inactivated by GAPs (which promote GTP hydrolysis). Cholera toxin locks $\text{G}_{\alpha s}$ on by blocking GTPase activity. Oncogenic Ras mutations lock Ras on by the same mechanism. A constitutively active mutation is one that stays GTP-bound. A loss-of-function mutation in a GAP has the same effect as a constitutively active mutation in the GTPase itself, because the brake is gone.

**Feedback and cross-talk questions** ask about what happens downstream when you perturb one component. If you add a phosphodiesterase inhibitor (like caffeine or theophylline), cAMP rises because degradation is blocked even if synthesis is unchanged. If you add a constitutively active adenylyl cyclase, cAMP rises even without receptor activation. If you knock out a phosphatase, signaling is prolonged. Always trace the logic from perturbation to downstream consequence.

**Nuclear receptor questions** typically ask about lipid-soluble hormone signaling. The key features: the receptor is intracellular, the ligand crosses the membrane, and the response is transcriptional (slow, hours, sustained). Contrast with peptide hormone signaling through GPCRs: the receptor is at the surface, the ligand does not cross the membrane, and the response can be rapid (seconds to minutes).

---

## Worked Problems

**Problem 1**

A researcher treats cells with an antibody that permanently crosslinks and dimerizes the epidermal growth factor receptor (EGFR, an RTK) even in the absence of EGF. She observes increased ERK phosphorylation and cell proliferation. She then adds a selective MEK inhibitor and the ERK phosphorylation returns to baseline, but the cells continue to proliferate slowly. She considers two explanations: (1) a parallel pathway downstream of the receptor does not require MEK; (2) MEK inhibition was incomplete. She tests cells expressing a constitutively active Raf mutant and finds that these cells do not proliferate when MEK is inhibited at the same dose. What does this tell her about the two explanations?

*Working through it:*

Start with what the crosslinking antibody is doing. Crosslinking the RTK mimics ligand binding by forcing dimerization, triggering autophosphorylation and activating all downstream pathways. The MEK inhibitor blocks the ERK arm. If explanation 1 is correct (parallel pathway independent of MEK), then cells expressing constitutively active Raf should also continue proliferating despite MEK inhibition, because the parallel pathway is downstream of the receptor and does not require Raf or MEK. But they do not: constitutively active Raf cells stop proliferating when MEK is inhibited at the same dose. This rules out a Raf-independent parallel pathway and is more consistent with explanation 2, incomplete MEK inhibition. The crosslinked-receptor cells may be generating more signal than the constitutively active Raf cells (because the receptor also activates other pathways like PI3K), lowering the effective inhibitor concentration needed. To test this definitively, she should titrate the MEK inhibitor to ensure complete inhibition and check whether proliferation is fully abolished.

**Problem 2**

Caffeine inhibits phosphodiesterase. A patient with asthma is treated with theophylline (same mechanism). At therapeutic doses, theophylline causes bronchodilation in the airway smooth muscle. Epinephrine also causes bronchodilation by activating $\beta_2$-adrenergic receptors on airway smooth muscle. Explain the mechanism of each and predict whether combining the two at half doses would produce more, less, or the same effect as either alone at full dose.

*Working through it:*

Epinephrine mechanism: epinephrine binds the $\beta_2$-adrenergic receptor (GPCR, $\text{G}_s$-coupled) $\rightarrow$ $\text{G}_{\alpha s}$ activates adenylyl cyclase $\rightarrow$ cAMP rises $\rightarrow$ PKA is activated $\rightarrow$ PKA phosphorylates myosin light-chain kinase (inactivating it) and other targets, reducing smooth muscle contractility $\rightarrow$ bronchodilation.

Theophylline mechanism: inhibits phosphodiesterase, which is the enzyme that degrades cAMP to 5'-AMP. Blocking degradation raises cAMP independently of whether synthesis is increased. The downstream effect (PKA activation, smooth muscle relaxation) is the same.

Both drugs raise cAMP, but by different mechanisms: one increases production, the other decreases degradation. Combining them at half dose of each would be expected to produce a greater-than-additive (synergistic) effect, because the two mechanisms reinforce each other. Epinephrine raises cAMP by stimulating synthesis; theophylline prevents that cAMP from being destroyed. The net cAMP level when both are present simultaneously would be substantially higher than from either mechanism alone at half dose. This is why combination bronchodilator therapy can be effective at doses that would individually be subtherapeutic.

**Problem 3**

A loss-of-function mutation in the RGS12 gene (RGS proteins are GAPs for $\text{G}_\alpha$ subunits) is found in a subset of patients with a particular disease characterized by chronic overactivation of pain signaling pathways that use $\text{G}_q$-coupled receptors in dorsal root ganglion neurons. Explain the molecular mechanism connecting RGS12 loss-of-function to chronic pain, tracing the pathway from receptor to cellular output.

*Working through it:*

RGS12 accelerates GTP hydrolysis by $\text{G}_{\alpha q}$. Without RGS12, $\text{G}_{\alpha q}$-GTP accumulates because it cannot hydrolyze GTP fast enough to terminate signaling on its own. $\text{G}_{\alpha q}$-GTP activates phospholipase C, which cleaves $\text{PIP}_2$ to IP3 and DAG. IP3 binds ER receptors and releases $\text{Ca}^{2+}$ into the cytoplasm. Elevated intracellular $\text{Ca}^{2+}$ activates calmodulin-dependent kinases and PKC (activated by DAG plus $\text{Ca}^{2+}$). In dorsal root ganglion neurons, sustained $\text{Ca}^{2+}$ elevation and kinase activity lower the threshold for action potential firing, sensitize TRPV1 and other nociceptive channels, and increase the release of pro-pain neurotransmitters (substance P, glutamate). The net result is a lower pain threshold and enhanced transmission of pain signals, a state called central and peripheral sensitization. The same molecular mechanism underlies why phospholipase C inhibitors have been explored as analgesics: by damping the $\text{G}_q$ pathway output, they could restore normal pain thresholds in sensitized neurons.

---

## Summary

Signal transduction converts extracellular chemical information into intracellular behavioral changes without letting the signal itself cross the membrane. The two major architectures are GPCRs, which use heterotrimeric G proteins and second messengers (cAMP, IP3/DAG/Ca$^{2+}$) to transduce signals, and RTKs, which use receptor dimerization, autophosphorylation, and kinase cascades (Ras $\rightarrow$ Raf $\rightarrow$ MEK $\rightarrow$ ERK) to do the same.

Both systems use GTPase switches: $\text{G}_\alpha$ in the GPCR system, Ras in the RTK system. Both switches are activated by GEFs and inactivated by GAPs. Cholera toxin locks $\text{G}_{\alpha s}$ on by ADP-ribosylating and impairing its GTPase activity, producing constitutive cAMP signaling and massive intestinal fluid secretion. Oncogenic Ras mutations impair GAP-assisted GTP hydrolysis, locking Ras on and driving constitutive proliferative signaling in cancer.

Signal termination is as important as initiation. Phosphodiesterases, phosphatases, GRKs, arrestins, RGS proteins, and GAPs all contribute to turning the signal off. Loss of any termination mechanism can be as oncogenic as constitutive activation of a positive effector.

Nuclear receptors provide a parallel system for lipid-soluble ligands: the ligand crosses the membrane, binds an intracellular receptor that is itself a transcription factor, and the response is transcriptional and slow.

The unifying principle is that cells are not passive recipients of signals; they are sophisticated information processors that amplify, integrate, and terminate signals at every step.
