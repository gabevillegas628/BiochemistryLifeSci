# Chapter 2: Protein Composition & Structure

---

## Opener Questions

Think about these before you read. Come back to them at the end and see if your answer changed.

1. A protein is denatured by heating, then slowly cooled. Under what conditions would you expect it to refold correctly, and what does that tell you about where the structural information is stored?

2. Sickle cell disease is caused by a single amino acid substitution in hemoglobin: glutamate is replaced by valine at position 6 of the beta chain. Glutamate carries a negative charge at physiological pH; valine is nonpolar and hydrophobic. Without knowing anything else about the molecular mechanism, predict what this substitution might do to the protein's behavior and explain your reasoning.

---

## The Big Picture

There is one principle that organizes all of protein biochemistry: **structure determines function**. It sounds obvious until you take it seriously. A protein's amino acid sequence determines its three-dimensional shape, and its three-dimensional shape determines what it can do. Change the shape and you change the function. Change it enough and you destroy the function entirely. Change one amino acid in the wrong place, you die.

Sickle cell disease will be the through-line for this chapter. It is caused by a single NUCLEOTIDE mutation in the gene encoding hemoglobin's beta chain, which changes ONE amino acid out of 147, which changes the surface chemistry of the protein in a small but specific region, which causes hemoglobin molecules to polymerize under low-oxygen conditions, which distorts red blood cells into rigid crescents that clog small vessels and rupture prematurely. One letter in three billion. One amino acid. A cascade of molecular consequences that ends in a painful, life-shortening disease.

By the end of this chapter you will be able to explain, at the molecular level, exactly how that happens. To get there, you need to understand what proteins are made of, what forces hold them together, how they fold, and what happens when folding goes wrong.

---

## The Chemical Foundation: Forces That Shape Proteins

Before we talk about amino acids or protein structure, we need to establish the vocabulary of forces. Proteins are held together by the same physical forces that govern all of chemistry and physics, but proteins use these forces in a specific hierarchy: some forces provide the scaffold, others provide the driving force for folding, and others provide the precision that makes molecular recognition possible.

### Covalent Bonds

Covalent bonds are the strongest force in a protein and the least interesting for understanding folding. They provide the backbone. Every protein chain is a covalent polymer: amino acids linked end-to-end by peptide bonds (discussed in detail in the next section), with a bond energy of roughly 350 kJ/mol.

A point worth making explicitly, because it connects directly to Chapter 1: peptide bond hydrolysis is thermodynamically favorable ($\Delta G^{\circ'} \approx -10$ to $-20$ kJ/mol). Proteins are NOT thermodynamically stable in water; they are metastable. The amino acids they are made from are the lower-energy state. What makes proteins functionally stable is kinetics: the uncatalyzed half-life for peptide bond hydrolysis at physiological pH and temperature is on the order of hundreds to thousands of years. The thermodynamics says it must happen; the activation energy barrier says not in any timeframe that matters without a catalyst. This is the diamond argument from Chapter 1, applied to your own proteins. Proteases, the enzymes that hydrolyze peptide bonds (on purpose), are how cells make this thermodynamically mandatory reaction occur on a biologically useful timescale when they actually need to degrade a protein.

For the purposes of protein folding, the practical consequence is that peptide bonds do not break and reform during folding. The primary structure is fixed. Folding is a search over conformational space with the covalent backbone as an unchanging scaffold.

The one interesting exception is the **disulfide bond**, formed between two cysteine residues when their sulfhydryl groups (-SH) are oxidized. Disulfide bonds have a bond energy of about 200 kJ/mol and are reversible: they can be broken by reducing agents (such as $\beta$-mercaptoethanol or dithiothreitol) and reformed under oxidizing conditions. Disulfide bonds are common in extracellular proteins and in proteins secreted into oxidizing environments. Inside most cells, the cytoplasm is reducing, and disulfide bonds are rare. This distinction matters for the Anfinsen experiment, which we will cover shortly.

### Hydrogen Bonds

A hydrogen bond forms between a hydrogen atom covalently bonded to an electronegative atom (oxygen or nitrogen, the hydrogen bond donor) and another electronegative atom (the hydrogen bond acceptor). In proteins, the most important donors are backbone N-H groups and side chain O-H and N-H groups; the most important acceptors are backbone C=O groups and side chain oxygen and nitrogen atoms.

$$\underbrace{C=O^{\delta -}}_{\text{acceptor}} \;\cdots\; \underbrace{^{\delta +}H-N}_{\text{donor}}$$

Individual hydrogen bonds are weak: 2 to 30 kJ/mol, compared to 350 kJ/mol for a covalent bond. This weakness is a feature, not a bug. Hydrogen bonds are strong enough to provide structural stability but weak enough to be broken and reformed, which is necessary for protein function and for the folding process itself. A hydrogen bond is also highly directional: the donor, hydrogen, and acceptor must be approximately linear for the interaction to be strong. This directionality is what makes hydrogen bonds so useful for building the precise, repeating geometries of secondary structures.

The collective power of hydrogen bonds is easy to underestimate. A typical protein has hundreds of backbone hydrogen bonds. Each one contributes modestly; together they provide substantial stability. More importantly, hydrogen bonds with water compete with intramolecular hydrogen bonds: an unfolded protein forms hydrogen bonds with surrounding water molecules, and folding requires displacing those water-protein hydrogen bonds and replacing them with intramolecular ones. The net stability gain from folding is actually quite small (often only 20 to 60 kJ/mol total for the entire protein), which is why proteins are surprisingly fragile and easily denatured.

### Ionic Interactions

Oppositely charged groups attract each other electrostatically. In proteins, the relevant charged groups are the ionizable side chains discussed in Chapter 1: positively charged lysine, arginine, and histidine; negatively charged aspartate and glutamate. When two oppositely charged side chains are in close proximity, they form a **salt bridge**, contributing 4 to 80 kJ/mol depending on the local environment.

That range is large because ionic interaction strength depends critically on the local dielectric constant. Water has a high dielectric constant (it shields charges from each other), so ionic interactions at the protein surface, where residues are in contact with water, are relatively weak. Inside the hydrophobic core, the dielectric constant is much lower, so any ionic interaction that forms there is much stronger. This is also why burying a charged residue in the hydrophobic core without a counterion is destabilizing: the charge is no longer shielded by water, and the electrostatic energy is enormously unfavorable.

Recall from Chapter 1 that charged state depends on pH. A salt bridge between Asp and Lys exists only if Asp is deprotonated and Lys is protonated, which is true at physiological pH for both. Changing the pH, or altering the local electrostatic environment enough to shift a side chain's apparent pKa, can break a salt bridge and destabilize the protein. This is one reason why extreme pH denatures proteins.

### Hydrophobic Interactions

Hydrophobic interactions are the dominant driving force for protein folding, and they are the most conceptually subtle of the five forces because they are not really "bonds" at all. No attractive force pulls nonpolar groups together. What happens instead is that water is forced away from them.

Water is a highly structured liquid. When a nonpolar molecule is dissolved in water, water molecules form ordered, cage-like structures (clathrate structures) around it to maintain their hydrogen bonding network without including the nonpolar solute. This ordering decreases the entropy of the water. When two nonpolar groups come together and their combined surface area in contact with water decreases, some of those ordered water molecules are released back into bulk solvent, increasing their entropy substantially. The thermodynamic driving force is the increase in $\Delta S_{surr}$, exactly as in Chapter 1: the hydrophobic effect is entropy-driven.

This has an important consequence for temperature. Most proteins unfold at high temperatures. But some proteins actually become more stable at moderately elevated temperatures, which makes no intuitive sense if you think of folding as driven by attractive interactions. It makes perfect sense if you recognize that the hydrophobic effect (an entropy-driven force) becomes stronger as temperature increases, because $T \Delta S$ grows with $T$. Only when you get hot enough that the protein's covalent structure begins to be disrupted does denaturation win.

The hydrophobic effect explains the basic architecture of nearly every soluble protein: a densely packed hydrophobic core of nonpolar residues buried away from water, surrounded by a surface where charged and polar residues interact with the aqueous environment. This inside-out architecture is not a design choice; it is thermodynamic necessity.

### Van der Waals Forces

Van der Waals forces arise from transient, induced dipoles. Even electrically neutral atoms fluctuate in their electron distribution, and when two atoms are very close together, the fluctuating dipole in one induces a complementary dipole in the other, creating a weak, transient attractive interaction. Each individual van der Waals interaction is negligibly small: roughly 0.4 kJ/mol. But a folded protein contains thousands of such close contacts in its packed interior, and they add up.

Van der Waals forces drop off rapidly with distance (as $r^{-6}$) and become repulsive at very short range when electron clouds overlap. This means they require precise geometric complementarity to be effective. The atoms have to be neither too far apart nor too close. This is why the hydrophobic core of a protein is not a loosely aggregated glob of nonpolar residues but a tightly packed, geometrically precise structure where every atom fits snugly against its neighbors. Van der Waals forces are responsible for that precision.

### Summary

| Force | Strength (kJ/mol) | Reversible? | Primary role |
|---|---|---|---|
| Covalent (peptide bond) | ~350 | No | Backbone scaffold |
| Disulfide bond | ~200 | Yes (reduction) | Tertiary stabilization, extracellular proteins |
| Hydrogen bond | 2-30 | Yes | Secondary structure, active sites |
| Ionic interaction | 4-80 | Yes | Salt bridges, active sites, DNA binding |
| Hydrophobic interaction | variable | Yes | Primary driving force for folding |
| Van der Waals | ~0.4 each | Yes | Core packing precision |

No single force explains protein structure. The covalent backbone defines the sequence; hydrophobic interactions drive collapse; hydrogen bonds enforce geometry; ionic interactions and van der Waals forces provide specificity and stability. Everything else in this chapter is an elaboration of how these forces cooperate.

---

## The Amino Acids

### General Structure

Every amino acid shares the same core: a central **alpha-carbon** bonded to four groups at pH 7: an amino group ($-NH_{3}^{+}$), a carboxyl group ($-COO^{-}$), a hydrogen atom, and a variable **side chain** (also called the R group). The side chain is what makes each amino acid chemically distinct. In the twenty standard amino acids found in proteins, the R group ranges from a single hydrogen atom (glycine) to a large aromatic ring system (tryptophan).

At physiological pH, the free amino group is protonated as shown above and the carboxyl group is deprotonated (also as shown above). The amino acid exists as a **zwitterion**: it carries both a positive and a negative charge simultaneously but is electrically neutral overall. This is a direct application of Henderson-Hasselbalch from Chapter 1: the alpha-amino group has a pKa around 9 to 10 (so it is protonated at pH 7.4), and the alpha-carboxyl group has a pKa around 2 (so it is deprotonated at pH 7.4).

All amino acids used in proteins (except glycine) have four chemically distinct groups bonded to the alpha-carbon, making it a **chiral center**. All amino acids in proteins are the L-configuration. This is not a biochemical accident; it has profound consequences for protein structure, as we will see.

An aside: why are all amino acids in proteins the L-configuration? This is one of the many unsatisfying answers you will encounter in biochemistry: because that is the way it is, and we are stuck with it. Using both L- and D-amino acids would have required a completely parallel set of stereospecific enzymes; the ribosome, the aminoacyl-tRNA synthetases, and virtually every metabolic enzyme are exquisitely L-specific. Once L-amino acids became established early in the history of life, the entire enzymatic machinery organized around them, making any change prohibitively costly. This is what biologists call a **frozen accident**: locked in not because it was optimal, but because it was good enough, and the cost of changing it exceeded any conceivable benefit. That is the real lesson of Darwin's natural selection, more so than Herbert Spencer's "survival of the fittest": evolution doesn't produce the best solution, it produces a solution that was fit enough to survive.

### The Peptide Bond

Amino acids are linked into chains by **peptide bonds**, formed when the carboxyl group of one amino acid reacts with the amino group of the next in a condensation reaction that releases water. The resulting chain is a **polypeptide**.

What makes the peptide bond remarkable is its partial double-bond character. Resonance delocalization allows the nitrogen's lone pair to be shared with the adjacent carbonyl carbon, which gives the C-N bond about 40% double-bond character. The consequence is that the six atoms involved in the peptide bond unit ($C_\alpha-CO-NH-C_\alpha$) are locked into a single plane. Rotation around the peptide bond itself is severely restricted.

This has a structural implication that cannot be overstated: the rigid planarity of the peptide bond limits where the backbone can go. The only free rotations in the backbone are around the bond from the alpha-carbon to the nitrogen (the phi angle, $\phi$) and from the alpha-carbon to the carbonyl carbon (the psi angle, $\psi$). Not all combinations of phi and psi are sterically allowed, which is why proteins adopt specific secondary structures rather than collapsing into arbitrary tangles.

Peptide bonds exist almost exclusively in the *trans* configuration, with the two alpha-carbons on opposite sides of the C-N bond. The *cis* configuration places the side chains of adjacent residues close together, which creates steric clash that costs roughly 8 kJ/mol. The exception is proline, where *cis* and *trans* isomers are nearly equal in energy because proline's cyclic structure creates steric strain in both configurations.

The chain always has a free amino group at one end (the **N-terminus**) and a free carboxyl group at the other (the **C-terminus**). By convention, sequences are written and numbered from N to C.

### The Twenty Amino Acids

Rather than listing all twenty alphabetically, which is how every student memorizes them and forgets them by the next week, we group them by side chain chemistry. The chemistry of the side chain determines where an amino acid ends up in a folded protein, how it behaves at physiological pH, and what role it can play in enzymatic catalysis.

#### Nonpolar and Aliphatic

**Glycine (Gly, G):** The smallest amino acid; its side chain is a single hydrogen atom. Because glycine has no real side chain, it has the most conformational flexibility of any amino acid. It is also the only amino acid that is not chiral. Glycine is found wherever the backbone needs to make a tight turn that would be sterically blocked by any larger side chain.

**Alanine (Ala, A):** A methyl group. Small, nonpolar, and ubiquitous. Alanine is the default nonpolar residue; when protein chemists want to eliminate a side chain without dramatically changing the backbone, they often substitute alanine.

**Valine (Val, V), Leucine (Leu, L), Isoleucine (Ile, I):** Branched aliphatic chains of increasing size. All three are strongly hydrophobic and are the primary residents of the hydrophobic core. Leucine is the most commonly occurring amino acid in protein cores. Valine is the amino acid that replaces glutamate in sickle hemoglobin; its hydrophobicity is the entire problem.

**Proline (Pro, P):** Unique in that its side chain loops back and forms a covalent bond with the backbone nitrogen, incorporating the nitrogen into a five-membered ring. The result is that proline has no backbone N-H group and therefore cannot donate a hydrogen bond from the backbone. This eliminates proline from most regular secondary structures. More critically, the ring rigidly constrains the phi angle, introducing a fixed kink into the polypeptide chain. Proline is a helix breaker and a chain-direction changer. It is commonly found at the end of helices and at turns between secondary structure elements.

**Methionine (Met, M):** Contains a sulfur atom in its side chain but is overall nonpolar and mildly hydrophobic. Methionine is also notable as the initiator amino acid: all proteins in eukaryotes begin synthesis with methionine, though this first residue is often cleaved after translation.

#### Aromatic

**Phenylalanine (Phe, F):** A benzene ring. Purely hydrophobic, large, and a common core resident. Aromatic rings can also engage in pi-stacking interactions (favorable face-to-face or edge-to-face arrangements of ring systems), which contribute to stability at protein-protein and protein-ligand interfaces.

**Tyrosine (Tyr, Y):** A phenol group: a benzene ring with a hydroxyl substituent. The hydroxyl group makes tyrosine capable of hydrogen bonding, so it can appear on protein surfaces as well as in the core. Tyrosine has a pKa around 10 for its hydroxyl group, so it is protonated (neutral) at physiological pH but can donate protons in enzyme active sites under the right conditions. Tyrosine is also a common site of phosphorylation in signal transduction pathways.

**Tryptophan (Trp, W):** The largest amino acid, with a bicyclic indole ring system. Tryptophan can both hydrogen bond (via the N-H of the indole) and engage in pi-stacking. It is strongly hydrophobic overall. Tryptophan absorbs ultraviolet light at 280 nm, which is why protein concentration is routinely measured at A$_{280}$.

#### Polar, Uncharged

**Serine (Ser, S) and Threonine (Thr, T):** Both carry a hydroxyl group: the side chain is a small alcohol. Both can hydrogen bond, and both are common sites of **phosphorylation** by protein kinases (covered in a later chapter on signal transduction). Because their hydroxyl groups are good nucleophiles at physiological pH, serine and threonine frequently appear in enzyme active sites.

**Cysteine (Cys, C):** The sulfhydryl group (-SH) makes cysteine chemically unusual. In reducing environments (the cytoplasm), cysteine exists as the free thiol. In oxidizing environments (the endoplasmic reticulum, extracellular space), two cysteine residues can be oxidized to form a disulfide bond (-S-S-). Disulfide bonds dramatically stabilize proteins that are secreted from cells and must function in environments less controlled than the cytoplasm. Cysteine is also a nucleophile and metal-binding ligand in many enzyme active sites.

**Asparagine (Asn, N) and Glutamine (Gln, Q):** Both carry amide groups, which can donate and accept hydrogen bonds but do not ionize at any physiological pH. Asparagine and glutamine are common sites of **glycosylation** (attachment of carbohydrate chains), particularly on extracellular proteins. They can be thought of as the non-ionizing versions of aspartate and glutamate.

#### Positively Charged (Basic)

**Lysine (Lys, K):** The epsilon-amino group on a long, flexible four-carbon chain has a pKa of about 10.5. At physiological pH 7.4, it is fully protonated and carries a positive charge. Lysine is strongly hydrophilic and almost always on the protein surface. Its positive charge makes it an ideal binding partner for negatively charged molecules: DNA phosphate groups, acidic lipids, phosphorylated substrates. Lysine is also a common site of ubiquitination, acetylation, and other post-translational modifications.

**Arginine (Arg, R):** The guanidinium group has a pKa above 12. Arginine is essentially always positively charged at any biological pH. The guanidinium group is planar and can form multiple hydrogen bonds simultaneously, making arginine an especially effective binder of phosphate groups and carboxylate groups. Where lysine is a single positive charge on a flexible tether, arginine is a flat, multi-dentate positive group. Many enzyme active sites use arginine specifically to grip phosphate-containing substrates.

**Histidine (His, H):** The imidazole side chain has a pKa of approximately 6.0 in free solution, and this is what makes histidine biochemically unique. At pH 7.4, histidine is just above its pKa, meaning it sits near the 50/50 boundary between protonated (positively charged, His$^+$H) and deprotonated (neutral, His) forms. A small shift in local pH or a change in nearby electrostatic environment (as discussed in Chapter 1) can push histidine from one form to the other. This makes histidine the only amino acid that can act as both an acid and a base at physiological pH, which is why it appears in the active site of an enormous fraction of all enzymes. When you encounter an enzyme mechanism in a later chapter and there is a histidine doing the proton-shuffling, this is why.

#### Negatively Charged (Acidic)

**Aspartate (Asp, D) and Glutamate (Glu, E):** Both carry a carboxylate group with a pKa around 3.5 to 4.5. At physiological pH 7.4, both are fully deprotonated and carry a negative charge. Both are strongly hydrophilic and almost always at the protein surface or in enzyme active sites. The difference between them is one methylene group: aspartate has a two-carbon side chain, glutamate has a three-carbon side chain. This difference in reach matters in specific binding and catalytic contexts. Glutamate is the amino acid at position 6 in normal hemoglobin beta chains; its negative charge is what keeps hemoglobin molecules from sticking to each other.

### Ionizable Side Chains: Connecting Back to Chapter 1

The side chain pKa values listed above are measured in free solution. As discussed at the end of Chapter 1, local electrostatic environments inside proteins can shift apparent pKa values substantially, sometimes by 2 to 3 units. The histidine in a given enzyme active site might have an apparent pKa of 7.5 rather than 6.0 because a nearby negative charge stabilizes the protonated form. The cysteine that acts as a nucleophile in a different enzyme might have its apparent pKa shifted from 8.3 down to 4 or lower by nearby positive charges and hydrogen bond donors, making it a much better nucleophile at physiological pH than a free cysteine in solution.

The Henderson-Hasselbalch equation applies directly:

$$\text{pH} = pK_a + \log\frac{[A^-]}{[HA]}$$

Given a side chain's apparent pKa and the local pH, you can determine its protonation state. The entire logic from Chapter 1 transfers here intact. What changes in proteins is that the pKa is not the textbook value; it is whatever the local environment has shifted it to. This is one of the central ways enzymes achieve their catalytic power: by precisely arranging side chains to create unusual charge states that could not exist in free solution.

**Reference table: all twenty amino acids**

| Amino Acid | 3-letter | 1-letter | Group | Charge at pH 7.4 | Ionizable Side Chain | Side Chain pKa |
|---|---|---|---|---|---|---|
| Glycine | Gly | G | Nonpolar, aliphatic | Neutral | No | — |
| Alanine | Ala | A | Nonpolar, aliphatic | Neutral | No | — |
| Valine | Val | V | Nonpolar, aliphatic | Neutral | No | — |
| Leucine | Leu | L | Nonpolar, aliphatic | Neutral | No | — |
| Isoleucine | Ile | I | Nonpolar, aliphatic | Neutral | No | — |
| Proline | Pro | P | Nonpolar, aliphatic | Neutral | No | — |
| Methionine | Met | M | Nonpolar, aliphatic | Neutral | No | — |
| Phenylalanine | Phe | F | Aromatic | Neutral | No | — |
| Tyrosine | Tyr | Y | Aromatic | Neutral | Yes | ~10.5 |
| Tryptophan | Trp | W | Aromatic | Neutral | No | — |
| Serine | Ser | S | Polar, uncharged | Neutral | No | — |
| Threonine | Thr | T | Polar, uncharged | Neutral | No | — |
| Cysteine | Cys | C | Polar, uncharged | Neutral | Yes | ~8.3 |
| Asparagine | Asn | N | Polar, uncharged | Neutral | No | — |
| Glutamine | Gln | Q | Polar, uncharged | Neutral | No | — |
| Lysine | Lys | K | Basic | Positive (+1) | Yes | ~10.5 |
| Arginine | Arg | R | Basic | Positive (+1) | Yes | ~12.5 |
| Histidine | His | H | Basic | Mostly neutral* | Yes | ~6.0 |
| Aspartate | Asp | D | Acidic | Negative (−1) | Yes | ~3.9 |
| Glutamate | Glu | E | Acidic | Negative (−1) | Yes | ~4.1 |

*Histidine is ~90% deprotonated (neutral) at pH 7.4 given its pKa of 6.0, but sits close enough to physiological pH that small environmental shifts can push it either way. This is what makes it uniquely useful in enzyme active sites.

---

## Levels of Protein Structure

The three-dimensional organization of a protein is described at four levels, each building on the one below.

### Primary Structure

The **primary structure** of a protein is its amino acid sequence, written from the N-terminus to the C-terminus. It is the only level of structure *directly* specified in the genetic code: each codon maps to one amino acid, and the ribosome strings them together in order. But "directly" is doing a lot of work in that sentence. As Anfinsen demonstrated, the primary sequence is sufficient to determine how a protein folds, which means all higher-order structure is ultimately encoded in DNA too, just indirectly, through the rules of chemistry and thermodynamics. AlphaFold made the same argument computationally: given only a sequence, it predicts structure with near-experimental accuracy. The gene encodes more than a string of amino acids; it encodes a shape. We just could not read it that way until recently.

$$
\underbrace{H_{3}N^{+}}_{\text{N-terminus}}-\overset{\substack{R_1 \\ |}}{C_\alpha} - CO - NH - \overset{\substack{R_2 \\ |}}{C_\alpha} - CO - NH - \cdots - NH - \overset{\substack{R_n \\ |}}{C_\alpha} - \underbrace{COO^{-}}_{\text{C-terminus}}
$$

Primary structure is where the sickle cell mutation lives. In normal hemoglobin (HbA), position 6 of the beta chain reads: Val-His-Leu-Thr-Pro-**Glu**-Glu. In sickle hemoglobin (HbS), it reads: Val-His-Leu-Thr-Pro-**Val**-Glu. One substitution, position 6, glutamate to valine. Everything that follows from it, the polymerization, the sickling, the disease, is a consequence of that single change in primary structure.

### Secondary Structure

**Secondary structure** refers to regular, repeating local structures stabilized by hydrogen bonds between backbone groups. Note what is not involved: side chains. Secondary structure is purely a backbone phenomenon, driven by the geometry of the polypeptide chain and the hydrogen bonding potential of backbone C=O and N-H groups.

#### The Alpha Helix

The **alpha helix** is a right-handed coil in which the backbone spirals around a central axis. Each residue advances the helix 1.5 Angstroms along the axis and rotates it 100 degrees, giving 3.6 residues per complete turn. The stabilizing hydrogen bonds run parallel to the helix axis, connecting the carbonyl oxygen of residue $i$ to the amide nitrogen of residue $i+4$. Every backbone C=O and every backbone N-H in the interior of the helix is hydrogen bonded.

The side chains project outward and downward from the helix axis, away from the core of the helix. This means side chains do not determine whether a helix forms; what matters is whether the backbone can adopt the phi/psi angles required ($\phi \approx -57°$, $\psi \approx -47°$). Proline cannot, which is why proline breaks helices. Very large side chains may also introduce steric clash between adjacent residues and destabilize helical geometry.

A useful property of some helices is the **amphipathic helix**, in which hydrophobic residues cluster on one face and hydrophilic residues on the other, like a log with a wet side and a dry side. This organization is common in membrane-spanning helices (the hydrophobic face contacts the lipid bilayer) and in helices that form coiled-coil structures at protein-protein interfaces.

#### The Beta Sheet

The **beta sheet** consists of extended polypeptide strands (beta strands) laid side by side, held together by hydrogen bonds between the backbone groups of adjacent strands. In a beta strand, the backbone is nearly fully extended, and the side chains alternate above and below the plane of the sheet on successive residues.

Beta sheets come in two flavors. In an **antiparallel** beta sheet, adjacent strands run in opposite directions (one N-to-C, the next C-to-N). The hydrogen bonds are linear and strong. In a **parallel** beta sheet, adjacent strands run in the same direction. The hydrogen bonds are slightly angled and somewhat weaker. Antiparallel sheets are more stable and more common, but both are found in proteins.

Beta sheets are not flat; they are pleated. The alternating side chains project above and below the plane, and the backbone alternates slightly above and below as well. Looking at a beta sheet edge-on, it has a gentle corrugated appearance.

#### Loops and Turns

The secondary structure elements that connect helices and strands are **loops** (irregular regions) and **turns** (short, defined reversals of chain direction). Loops are not structureless or unimportant. They are typically at the protein surface, where they are in contact with solvent, and they are often the most variable parts of a protein sequence across related proteins. They are also disproportionately represented at binding sites and active sites, where their flexibility and surface exposure make them ideal for molecular recognition.

A specific type of turn, the **beta turn**, uses four residues to reverse the chain direction by 180 degrees. Beta turns often connect the two strands of an antiparallel beta sheet and commonly contain glycine (for flexibility) or proline (for its fixed phi angle, which helps enforce the turn geometry).

### Tertiary Structure

**Tertiary structure** is the complete three-dimensional arrangement of all atoms in a single polypeptide chain: how the helices, sheets, turns, and loops are packed together in three-dimensional space. This is the level of structure at which proteins become individual molecular machines with specific shapes, specific surfaces, and specific functions.

The organizing principle of tertiary structure is the **hydrophobic core**. As a polypeptide folds, the dominant thermodynamic force is the hydrophobic effect: nonpolar side chains are driven to the interior, away from water, while charged and polar side chains are pushed to the surface. The result is a protein with a densely packed, nonpolar interior and a hydrophilic exterior in contact with aqueous solvent. Van der Waals interactions fine-tune the packing of the core; hydrogen bonds and ionic interactions provide additional stability and precision.

Many large proteins are organized into **domains**: discrete structural units that fold independently and often have distinct functions. A single polypeptide might contain a DNA-binding domain, a catalytic domain, and a regulatory domain, each folding into its own compact structure and connected by flexible linker regions. Domains can sometimes be swapped between proteins, mixed, and matched, which has been an important mechanism of evolutionary diversification.

Now the sickle cell mechanism becomes clear. At position 6 of the beta chain, glutamate (negatively charged, hydrophilic) normally sits on the surface of the hemoglobin subunit, in contact with water, in the energetically appropriate environment for a charged residue. In HbS, valine (nonpolar, hydrophobic) sits at the same position. A hydrophobic residue on a protein's surface is exposed to water, which it dislikes thermodynamically. The protein cannot bury it internally without a major conformational rearrangement, so it remains exposed. This creates a small hydrophobic **sticky patch** on the surface of the HbS subunit. There is a complementary hydrophobic pocket on another part of the hemoglobin molecule, and in the deoxygenated conformation of HbS, that pocket is exposed. The sticky patch on one HbS molecule fits into the exposed pocket of another, and polymerization begins. The full clinical consequences are covered in the section on pathology below.

### The Anfinsen Experiment: Sequence Determines Structure

In the 1950s and 1960s, Christian Anfinsen at the NIH asked a simple but profound question: where is the information for protein folding stored? Is it in the amino acid sequence, or does it require some external biological machinery to guide the process? Is there a "secret sauce" to the process, as it were.

His experimental subject was ribonuclease A (RNase A), a small enzyme of 124 amino acids that cleaves RNA and whose structure is stabilized by four disulfide bonds.

Anfinsen denatured RNase A completely using two reagents simultaneously: urea at high concentration (which disrupts hydrogen bonds, ionic interactions, and hydrophobic interactions, unfolding the protein) and beta-mercaptoethanol (which reduces the four disulfide bonds to free thiols thus breaking the S-S bridges). The result was a fully unfolded, enzymatically inactive protein with eight free cysteine residues.

He then removed both denaturants by dialysis, allowing the protein to experience physiological conditions again.

RNase A refolded spontaneously. Enzymatic activity returned to essentially 100%. The four disulfide bonds reformed, and crucially, they reformed in exactly the correct pairing of the eight cysteines (only when he removed the urea first though, *why might that be?*). There are 105 possible ways to pair eight cysteines into four disulfide bonds, but only one of those pairings is the native structure. The protein found it, without any external guidance, every time.

The control experiment made the point even sharper. If Anfinsen removed only the urea (leaving beta-mercaptoethanol in solution, so disulfide bonds could not reform), the protein refolded its backbone but formed with scrambled, incorrect disulfide bonds and was essentially inactive. When he then removed the beta-mercaptoethanol from this scrambled form, allowing disulfide bond shuffling to occur, the protein found its correct disulfide arrangement and recovered full activity. The correct disulfide bonds are not just correct by chance; they are the thermodynamically stable ones, determined entirely by the amino acid sequence.

The conclusion is unambiguous: **the three-dimensional structure of a protein is determined entirely by its amino acid sequence**. No external template, no cellular machinery, no additional information is required. The sequence encodes the fold. This is sometimes called the thermodynamic hypothesis of protein folding: the native state is the conformation of minimum Gibbs free energy, and folding is simply the thermodynamically mandatory descent to that minimum.

This is Chapter 1 again. Folding is spontaneous because $\Delta G < 0$ for the transition from unfolded to native state under physiological conditions. The native state is not merely preferred; it is thermodynamically required. If you denature a protein and restore physiological conditions, the second law of thermodynamics does the rest.

### Why Doesn't Folding Take Forever? The Energy Funnel

The Anfinsen experiment raises a question that took decades to answer: if the native state is determined by a thermodynamic minimum, and the protein must find that minimum among an astronomical number of possible conformations, why does folding happen in microseconds to seconds rather than the lifetime of the universe?

This is **Levinthal's paradox**, posed by Cyrus Levinthal in 1969. Consider a protein of 100 amino acids. If each residue can adopt three backbone conformations (a dramatic simplification: the number is much larger), there are $3^{100} \approx 5 \times 10^{47}$ possible conformations. Molecular motions occur on the timescale of $10^{-13}$ seconds, so the protein can sample conformations at roughly $10^{13}$ per second. To search all conformations randomly would take:

$$\frac{5 \times 10^{47}}{10^{13}} = 5 \times 10^{34} \text{ seconds} \approx 10^{27} \text{ years}$$

The universe is approximately $1.4 \times 10^{10}$ years old. Random search is not the answer.

The resolution is the **energy funnel**. Protein folding is not a random search of conformational space; it is a biased, progressive descent toward lower free energy. The funnel metaphor: imagine a wide, irregular funnel with the top rim representing all possible unfolded conformations (high energy, high entropy, many states) and the narrow bottom representing the native state (low energy, low entropy, one state). The protein does not wander randomly across the rim looking for the drain; it slides downhill.

The key early event is **hydrophobic collapse**: within microseconds of encountering physiological conditions, hydrophobic residues aggregate together to minimize water contact. This collapses the chain from an extended random coil to a compact, partially structured globule, immediately reducing the accessible conformational space from astronomical to manageable. The chain has not found the native state yet, but it is in the right neighborhood.

From this compact intermediate, secondary structure forms progressively, and tertiary contacts develop. Each stabilizing interaction constrains the remaining degrees of freedom, further narrowing the search. The funnel guides the protein not by a single mandatory path but by thermodynamic gradient: the next conformation is more likely to be slightly more stable than slightly less stable, so the trajectory is downhill on average even if it is noisy.

The funnel is not perfectly smooth. There are local minima, partially folded intermediates that are more stable than the unfolded state but less stable than the native state, into which a protein can get kinetically trapped. This is where **chaperone proteins** become important. In rare and catastrophic cases, a protein can settle into an alternative stable conformation that is thermodynamically competitive with the native state but biologically useless or actively toxic. Prion diseases are the most striking example: the misfolded prion protein ($PrP^{Sc}$) is nearly as stable as the normal form, resists all normal degradation, and templates the conversion of normal protein to the misfolded state. We will return to prions in detail in the misfolding section below.

Chaperones (including the Hsp70 family and the GroEL/GroES complex) are proteins that assist other proteins in folding correctly inside the cell. They do not encode structural information and do not do the folding themselves. What they do is bind to exposed hydrophobic regions on partially folded or misfolded proteins, preventing those hydrophobic patches from aggregating with other partially folded proteins (which would be thermodynamically favorable but catastrophic). They then release the protein in an ATP-dependent manner, giving it another chance to fold correctly. The GroEL/GroES system in bacteria provides a protected chamber where a single protein molecule can fold without interference from neighboring molecules. In the crowded environment of the cell, where protein concentration is extremely high, chaperones are essential for preventing the aggregation that would otherwise occur during the slow business of folding.

Chaperones are kinetics helpers: they lower the effective activation energy for folding and prevent kinetic traps. They do not change the thermodynamic endpoint. The native state remains the minimum free energy conformation; chaperones just help the protein find it faster and more reliably in the cellular environment. This is the same distinction from Chapter 1 applied to protein folding: thermodynamics determines the destination, kinetics determines how quickly you get there.

### Quaternary Structure

Many functional proteins consist of more than one polypeptide chain. The arrangement of multiple folded subunits (called **protomers**) into a functional complex is **quaternary structure**. The subunits are held together by the same non-covalent forces that stabilize tertiary structure: hydrophobic interactions, hydrogen bonds, ionic interactions, and van der Waals contacts at the interfaces between chains. Quaternary structure does not require covalent bonds between subunits, though some complexes are additionally stabilized by disulfide bonds.

Proteins with identical subunits are **homomers** (a homodimer, homotrimer, etc.). Proteins with different subunits are **heteromers**. Hemoglobin is a heterotetramer: two alpha chains and two beta chains, assembled as an $\alpha_2\beta_2$ complex.

Why evolve quaternary structure rather than simply making a larger single polypeptide? Several reasons. First, large structures can be built from smaller, independently folding units, each of which has a lower error rate during synthesis and folding. Second, subunit interfaces create new surfaces and cavities that do not exist in any individual subunit, enabling new functions. Third, and most importantly for biochemistry: **subunit interactions enable cooperativity and allosteric regulation**.

When subunits communicate through conformational changes, binding an effector molecule at one site can change the properties of a distant site on another subunit. Hemoglobin is the canonical example: binding oxygen to one subunit changes the conformation of all four subunits, increasing the affinity of the remaining sites for oxygen. This cooperativity allows hemoglobin to load oxygen efficiently in the lungs and unload it efficiently in peripheral tissues, a feat that no monomeric oxygen-binding protein can achieve. The full treatment of hemoglobin cooperativity is in a later chapter, but the structural basis is quaternary: without subunit-subunit communication, there is nothing to cooperate.

---

## When It Breaks

### Sickle Cell Disease: One Amino Acid, One Disease

The complete molecular account of sickle cell disease is now within reach.

Normal adult hemoglobin (HbA) is an $\alpha_2\beta_2$ tetramer. The beta chain carries glutamate at position 6 (Glu6): negatively charged, hydrophilic, at home on the protein surface in contact with water. The surface of HbA at this position is electrically normal; there is no unusual hydrophobic patch.

In sickle hemoglobin (HbS), the codon for Glu6 (GAG) is mutated to a codon for Val (GTG). Valine is nonpolar and hydrophobic. On the surface of the protein, exposed to aqueous solvent, valine is thermodynamically out of place. It creates a small hydrophobic sticky patch at position 6 of each beta chain.

Complementary to this patch is a hydrophobic pocket on the surface of another hemoglobin subunit. In oxygenated HbS, that pocket is occupied by a side chain from within the same molecule; the patch and the pocket cannot interact. In deoxygenated HbS, a conformational change (the T-state transition that normally accompanies oxygen release) exposes the hydrophobic pocket.

Now the sticky patch on one HbS molecule can insert into the exposed pocket of a neighboring HbS molecule. This nucleates a growing polymer: each molecule added exposes its own pocket at the end, ready to accept the next molecule's sticky patch. The result is long, rigid fibers of polymerized HbS that span the interior of the red blood cell, distorting it from a flexible biconcave disc into a stiff, crescent-shaped sickle.

The clinical consequences follow directly from the structural properties of sickled cells. Rigid cells cannot deform to squeeze through capillaries, so they obstruct small vessels: this causes the excruciating vaso-occlusive pain crises characteristic of the disease, and over time, ischemic damage to any organ with a microvascular supply (spleen, kidney, brain, bone). Sickled cells are also mechanically fragile and rupture prematurely, causing hemolytic anemia.

The molecular logic also explains the epidemiology. Sickling occurs specifically in deoxygenated conditions: in tissues with high metabolic demand, at altitude, during exertion, or in the low-oxygen environment that the malaria parasite creates inside red blood cells as it completes its lifecycle. Individuals with sickle cell trait (one normal and one sickle beta-globin gene, HbA/HbS) have enough HbA to prevent significant sickling under most conditions but enough HbS to create hostile conditions for malaria. In regions of sub-Saharan Africa where malaria is endemic, carrying one copy of the sickle mutation confers a survival advantage. The mutation persists in the population because heterozygotes survive malaria at higher rates than normal homozygotes, even though HbS homozygotes suffer from a severe disease.

### Protein Misfolding Diseases

The Anfinsen experiment shows that the native state is the thermodynamic minimum. But "thermodynamic minimum" means the most stable accessible state under physiological conditions, not the most stable state that could possibly exist. Some proteins can become trapped in alternative stable conformations that are not the native state but are too stable to spontaneously correct. These misfolded states can be not just non-functional but actively destructive.

**Prion diseases** are the most conceptually disturbing example. The prion protein (PrP) has a normal, functional form ($PrP^{C}$) that is predominantly alpha-helical. It also has a misfolded form ($PrP^{Sc}$) that is predominantly beta-sheet rich. $PrP^{Sc}$ is extremely stable: resistant to proteases, heat, radiation, and most conventional sterilization procedures. More disturbingly, $PrP^{Sc}$ acts as a template. When $PrP^{Sc}$ contacts $PrP^C$, it catalyzes the conversion of the normal protein to the misfolded form. This conversion propagates. No new genetic information is involved; the infectious agent is entirely protein. The misfolded protein is self-replicating.

The diseases caused by prion propagation include Creutzfeldt-Jakob disease in humans, scrapie in sheep, and bovine spongiform encephalopathy (BSE, "mad cow disease") in cattle. All are fatal and characterized by progressive neurodegeneration. From the energy funnel perspective, $PrP^{Sc}$ represents a deep local minimum that is thermodynamically stable but biologically catastrophic. Once a protein enters this well, it does not spontaneously escape, and it drags neighboring molecules in after it.

**Alzheimer's disease** involves a different misfolding problem with a similar structural logic. The amyloid-beta peptide, derived by proteolytic cleavage from a normal membrane protein (APP), is normally soluble. Under pathological conditions (which are not yet completely understood), amyloid-beta misfolds into a structure rich in cross-beta sheet, in which the beta strands from multiple peptide molecules run perpendicular to the long axis of growing fibril. These amyloid fibrils are thermodynamically stable and aggregate into the senile plaques found in Alzheimer's brain tissue. A similar cross-beta architecture characterizes tau protein aggregates, which form the neurofibrillary tangles characteristic of Alzheimer's and other tauopathies. Both represent proteins that have found a thermodynamically stable but biologically useless (and toxic) alternative conformation.

**Cystic fibrosis** presents a different failure mode. The most common cystic fibrosis mutation (${\Delta}F508$), a deletion of phenylalanine at position 508) causes the CFTR chloride channel to misfold. The misfolded CFTR is not aggregated or toxic; it is simply recognized by the cellular quality-control machinery (primarily chaperones of the Hsp70 and Hsp90 families) as having an abnormal conformation, and it is routed to proteasomal degradation before it can reach the plasma membrane.

The cruelty of this mechanism is that deltaF508 CFTR retains partial function: if it could reach the cell surface, it would transport chloride at reduced but potentially meaningful rates. The protein is not broken beyond all utility; it is being destroyed before it gets a chance. This is the rationale for the CFTR modulator drugs (correctors that help the misfolded protein escape quality control, potentiators that improve its function at the membrane) that have transformed CF treatment in recent years. The therapy is thermodynamic and kinetic: shift the folding equilibrium toward a conformation that passes quality control, then improve the function of whatever reaches the surface.

---

## The MCAT Angle

Protein structure is heavily tested on the MCAT, and the questions cluster around a few recurring reasoning patterns.

**Side chain charge at physiological pH.** You will be given a pKa and asked for the protonation state at pH 7.4. Apply Henderson-Hasselbalch: if pH > pKa, the group is predominantly deprotonated; if pH < pKa, it is predominantly protonated. Know the approximate pKa values for the ionizable groups: alpha-carboxyl (~2), aspartate/glutamate (~3.5-4.5), histidine imidazole (~6), alpha-amino (~9-10), cysteine thiol (~8.3), tyrosine hydroxyl (~10), lysine epsilon-amino (~10.5), arginine guanidinium (~12.5).

**Surface versus core.** Hydrophobic residues (Phe, Val, Leu, Ile, Met, Ala) belong in the core. Charged residues (Asp, Glu, Lys, Arg) belong on the surface. Histidine, Tyr, and Trp can appear in either location. If a question asks what happens when you mutate a charged residue to a nonpolar one in the interior of a protein, the answer depends on context: replacing a buried charged residue (which is already destabilizing) with a nonpolar one might actually increase stability.

**Mutation analysis.** The sickle cell question pattern: given a substitution, predict the structural and functional consequence using side chain chemistry. A hydrophobic residue on the surface creates a sticky patch. A charged residue buried in the core is destabilizing. A proline inserted mid-helix breaks the helix.

**Anfinsen reasoning.** What does spontaneous refolding prove? That the sequence contains all the structural information. What does failure to refold prove? That some factor required for the native state is absent (a cofactor, a disulfide-bonding environment, a specific post-translational modification). What does refolding to a non-native conformation prove? That the incorrect conformation is the thermodynamic minimum under the given conditions.

**Denaturing conditions.** Urea and guanidinium chloride at high concentration disrupt non-covalent interactions but do not break covalent bonds. Heat does the same (and eventually begins to disrupt covalent bonds at extreme temperatures). Reducing agents (BME, DTT) break disulfide bonds specifically. Extreme pH changes ionization states, disrupting ionic interactions and potentially changing the shape of the hydrophobic core by altering where charged residues prefer to sit.

---

## Worked Problems

### Problem 1: Side Chain Chemistry and Protein Location

A protein has a region of its sequence that reads: Lys-Phe-His-Asp-Ile-Arg-Leu. The protein is correctly folded at pH 7.4.

(a) Which residues in this segment carry a net positive charge? Which carry a net negative charge?

(b) Where would you expect the hydrophobic residues in this segment to be located in the folded protein? What about the charged residues?

(c) The protein is placed in a solution at pH 5.0. Predict qualitatively what happens to the charge distribution of this segment and what effect this might have on protein stability.

**Solution:**

(a) At pH 7.4, lysine (pKa ~10.5) is protonated: positive charge. Arginine (pKa ~12.5) is protonated: positive charge. Aspartate (pKa ~3.9) is deprotonated: negative charge. Phenylalanine, alanine, isoleucine, and leucine have no ionizable side chains: no charge.

(b) Phe, Ala, Ile, and Leu are nonpolar and hydrophobic. They are likely in the hydrophobic core of the protein, away from water. Lys, Asp, and Arg are charged at pH 7.4 and strongly hydrophilic. They are almost certainly on the surface of the protein in contact with solvent.

(c) We have 3 residues which contain ionizable functional groups in this peptide K, D and H with $Pk_{a}^{R}$ values of 10.5, 3.9 and 6.0 respectively. (Recall the $\alpha$ amino and carboxyl groups are no longer ionizable when they form a peptide bond). Changing the pH from 7.4 to 5.0 will not affect the K or D residues since K will still be at a pH below its $pK_a$ remaining protonated and D will still be above it's $pK_a$ remaining deprotonated. However, the H residue was above its $pK_a$ value of 6.0 at pH 7.4 and so was mostly deprotonated (+1) while at pH 5.0 (now below the pKa value of 6.0) it loses its ionizable proton adopting the neutral structure.

### Problem 2: Mutation Analysis

A point mutation in an enzyme changes leucine-47 to aspartate. Position 47 is located in the hydrophobic core of the protein, surrounded by several other nonpolar residues. Predict the effect of this mutation on protein stability and explain the thermodynamic reasoning.

**Solution:**

This mutation is expected to destabilize the protein substantially.

Leucine at position 47 is nonpolar and belongs in the hydrophobic core: burying it costs nothing thermodynamically and contributes to the favorable hydrophobic effect that drives folding. Aspartate carries a negative charge at physiological pH (pKa ~3.9, so fully deprotonated at pH 7.4).

Introducing a charged residue into the hydrophobic core creates several destabilizing problems. First, the charged carboxylate is surrounded by low-dielectric, nonpolar environment rather than high-dielectric water. Charged groups in low-dielectric environments are strongly destabilized: the electrostatic energy is much higher than in water, because there is no solvent to shield the charge. Second, the aspartate brings with it the thermodynamic cost of desolvation: a charged residue prefers to be in water, and burying it requires paying the energy cost of removing it from solvent without the compensating gain from hydrophobic burial. Third, the core geometry was shaped by evolution to pack nonpolar side chains tightly; the introduction of a larger, polar, charged residue will disrupt van der Waals packing.

The net $\Delta G$ of folding becomes less negative, and the protein is less stable. Depending on the magnitude of the destabilization, the protein may still fold (at reduced stability) or may not fold correctly at all, in which case it would likely be degraded by cellular quality-control machinery.

### Problem 3: Anfinsen Reasoning

A newly discovered enzyme has three disulfide bonds and 200 amino acids. It is denatured with urea plus beta-mercaptoethanol, then the denaturants are removed by dialysis in the presence of an oxidizing agent. The protein regains its correct secondary structure (verified by circular dichroism) but only 3% of enzymatic activity.

(a) What does the recovery of secondary structure tell you?

(b) What does the failure to recover enzymatic activity tell you about the role of the disulfide bonds in this protein?

(c) Propose an experiment to test whether the protein can find its correct disulfide bonds given enough time and the right conditions.

**Solution:**

(a) The recovery of secondary structure (alpha helices, beta sheets, as measured by the characteristic circular dichroism signal) tells you that the polypeptide backbone can adopt its correct local geometry. The primary structure contains the information for secondary structure formation, and removing the denaturants allows the backbone to return to its thermodynamically preferred phi/psi angles. This part of the Anfinsen result holds.

(b) The failure to recover enzymatic activity, despite correct secondary structure, tells you that the protein is not in its correct tertiary conformation, and the most likely reason is incorrect disulfide bond pairing. With three disulfide bonds and six cysteines, there are 15 possible pairings. If the protein refolds backbone-first and then traps disulfide bonds in the first oxidized configuration it encounters (rather than the thermodynamically correct one), most molecules will have scrambled disulfide bonds. Incorrect disulfide bonds can hold the protein in a non-native tertiary structure, preventing correct active site assembly. Only the 3% that happened to form the correct disulfide bonds by chance regain activity.

(c) Remove the oxidizing agent from the incorrectly folded, disulfide-scrambled protein, add a small amount of a thiol reagent (such as a small amount of beta-mercaptoethanol or DTT, enough to allow disulfide shuffling without fully reducing all bonds), and incubate. This allows the disulfide bonds to break and reform repeatedly (shuffling), exploring different pairings. If the correct disulfide bonds are the thermodynamically stable ones (as in the Anfinsen result), the protein should progressively find its correct native structure, and enzymatic activity should increase toward 100% over time. This is the direct analog of Anfinsen's scrambled ribonuclease control experiment.

---

## Opener Questions Revisited

**Question 1:** A protein is denatured by heating, then slowly cooled. Under what conditions would you expect it to refold correctly, and what does that tell you about where the structural information is stored?

Correct refolding requires conditions under which the native state is thermodynamically stable: physiological pH, physiological salt concentration, the presence of any required cofactors, and (for disulfide-containing proteins) an appropriate redox environment. If these conditions are met and no irreversible damage occurred during denaturation (aggregation, covalent modification, disulfide scrambling without opportunity to reshuffle), the protein should refold because the native state is the free energy minimum and folding is thermodynamically mandatory.

This tells you that the structural information is entirely in the amino acid sequence: the same conclusion as Anfinsen. No cellular machinery, no external template, and no additional biological information is required. The sequence encodes the fold; the fold is the function.

**Question 2:** A glutamate-to-valine substitution at position 6 of the hemoglobin beta chain. Predict the consequence.

Glutamate is negatively charged and hydrophilic at pH 7.4. Valine is nonpolar and hydrophobic. On the surface of a protein, a nonpolar residue is thermodynamically unfavorable: it prefers to be buried away from water. The valine at position 6 creates a hydrophobic patch on the surface of the HbS subunit. If a complementary hydrophobic surface exists elsewhere on the molecule (which in hemoglobin it does, specifically in the deoxygenated conformation), the sticky patch can insert into that pocket on a neighboring molecule, initiating polymerization. Polymerization distorts the red blood cell and causes the clinical disease.

The key reasoning step is: a hydrophobic residue on the protein surface is out of its preferred thermodynamic environment, and the way the protein can relieve that thermodynamic frustration is by burying the hydrophobic patch in contact with a complementary surface on another molecule. What looks like a molecular interaction problem is, at its core, a thermodynamics problem: the system is seeking a lower-energy state.

---

*Chapter 3: Molecular Binding & Hemoglobin*
