# 3clpro-rupintrivir-visualization

# Structural Analysis of the Rupintrivir–SARS-CoV-2 3CLpro Complex

Visualization and binding-pocket analysis of the SARS-CoV-2 main protease (3CLpro / Mpro) in complex with the covalent inhibitor **rupintrivir**, performed in PyMOL.

## Overview

3CLpro (also called Mpro) is the enzyme responsible for cleaving the SARS-CoV-2 polyprotein into the individual non-structural proteins required for viral replication. Because this cleavage step is essential to the viral life cycle, 3CLpro is one of the most extensively validated antiviral drug targets to emerge from the pandemic.

The enzyme functions as a homodimer and relies on a **Cys145–His41 catalytic dyad**: His41 deprotonates the Cys145 thiol, enabling nucleophilic attack on the substrate's scissile peptide bond. The substrate-binding cleft shows a strong preference for a Leu-Gln motif at the P2–P1 positions, with cleavage occurring at the P1–P1′ bond.

**Rupintrivir** was originally developed as an inhibitor of human rhinovirus/enterovirus 3C protease. It has since been investigated against coronaviral main proteases because 3CLpro shares structural similarity with the active-site domain of enteroviral 3C protease — making this structure a useful example of drug repurposing guided by structural homology.

## Structure Used

- **PDB ID:** [7P35](https://www.rcsb.org/structure/7P35)
- **Description:** SARS-CoV-2 3CL protease in complex with rupintrivir
- **Reference:** Fabrega-Ferrer, M., Herrera-Morande, A., Muriel-Goni, S., et al. (2022). *Antiviral Research*, 208, 105458. https://doi.org/10.1016/j.antiviral.2022.105458
- **Source:** Downloaded directly from RCSB PDB

## Method

1. Downloaded the 7P35 coordinate file from RCSB PDB.
2. Loaded the structure into PyMOL and rendered the protein as a green cartoon.
3. Isolated the co-crystallized rupintrivir ligand and recolored it in cyan for visual contrast against gray active-site side chains.
4. Generated a cavity/pocket mesh surface (magenta/pink) around the substrate-binding cleft to visualize pocket geometry independent of the bound ligand.
5. Rendered comparative views of the empty pocket, the ligand-occupied pocket, the isolated ligand, and the final composite complex.

## Figures

| Figure | Description |
|---|---|
| `panel1_protein.png` | Active-site region with pocket-detection mesh overlaid on protein cartoon and residue side chains |
| `panel2_ligand.png`, `panel2_ligand_2.png` | Whole-protein overview establishing the overall fold |
| `panel3_pocket.png` | Zoomed view of the mesh-defined cavity at the domain interface, near the catalytic dyad |
| `panel5_ligand_prep.png`, `panel5_ligand_prep_2.png` | Rupintrivir (cyan sticks) modeled within the detected pocket, showing pocket–ligand fit |
| `panel6_grid_box.png` | Isolated ligand geometry, showing rupintrivir's peptidomimetic scaffold |
| `panel9_final_complex.png` | Final composite view: protein + pocket mesh + ligand together |



## Skills Demonstrated

- Retrieval and interpretation of experimental structures from RCSB PDB
- PyMOL-based molecular visualization and rendering
- Binding-pocket/cavity detection and visualization
- Structural rationale for a drug-repurposing target (enterovirus 3C protease inhibitor → coronaviral main protease)

## Notes / Next Steps

- Future extension: quantify pocket volume and key contact residues (e.g., using fpocket or POVME) for a more rigorous computational comparison.
- Future extension: dock additional candidate ligands into the same pocket using AutoDock Vina to compare predicted vs. co-crystallized binding poses.

---
*Project created as part of independent structural biology skill-building, supporting graduate research (PhD) applications in molecular/cell biology.*
