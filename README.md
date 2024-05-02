# HDOCK_p53_dna_results

Explanation of files:

**wtp53_all_HDCOK_output and R273H_all_HDCOK_output**
- All output files from all HDOCK predictions for wild type p53 and mutp53 respectively, compressed

- **validating_with_2ATA_pro_struct_and_na_seq**
- All output files for validating HDOCK prediction of a known crystal structure from the PDB database (PDB code 2ATA), compressed

**wt_out and mut_out**
- Just the .out files from HDOCK predictions which contain information for translations, rotations, binding score, ligand RMSD, and tralsnlational ID. More information can be found here:
- http://hdock.phys.hust.edu.cn/help.php

**scatter_plot_docking_stats**
- This is a dataframe with information for creating a scatter plot to compare docking models. The model with the lowest RMSD from the first 10 predictions was appended along with the ligand RMSD, and Confidence Score (calculated from the given docking score)

**scatter_plot_confidence_score** 
-  Scatter plot comparing RMSD and confidence scores between wild type and R273H mutant.
  
**wt_averaged_residue_pairs and mutp53_averaged_residue_pairs**
- HDOCK provides residue interface information for the first 10 predictions for wild type p53 and mutp53 respectively. For each of the predicted strctures that were chosen for the scatter plot, residue interactions were taken and averaged across all protein-dna pairs. This dataframe contains the information for these residue pairs.

**wt_p53_contact_heatmap and mutp53_contact_heatmap** 
- png files that contain residue heatmaps for wild type p53 and mutp53 respectively.
