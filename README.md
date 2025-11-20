# Generality-oriented Optimization Campaign Dataset
Repository for the .xyz structural files for:

"Experimental Lineage and Computational Analysis of a General Aminoxyl-Based Oxidation Catalyst: Generality from Substrate-Specific Interactions"

Rozema, S. D.<sup>‡</sup>; Tampellini, N.<sup>‡</sup>; Rein, J.; Sigman, M. S.; Lin, S.; Miller, S. J. *ACS Catal.* **2025**, *15* (20), 17548-17557. DOI: [10.1021/acscatal.5c05893](https://doi.org/10.1021/acscatal.5c05893)

**EDIT:**
Added complete ground state DFT structures dataset (full_dataset.tar.gz) - this includes ALL DFT structures that successfully converged to a local minimum at the R<sup>2</sup>SCAN-3c level (~3000 .xyz files). In the comment line, salient properties are exported in a parse-friendly format: charge, multiplicity, electronic energy (Eh) and frequencies (cm<sup>-1</sup>).

If you find this dataset useful in your research, we ask you to cite the [original manuscript](https://doi.org/10.1021/acscatal.5c05893).

### Computational details (from the paper [supporting information](https://pubs.acs.org/doi/suppl/10.1021/acscatal.5c05893/suppl_file/cs5c05893_si_001.pdf))
Initial geometries for the covalent adducts were obtained using the Avogadro GUI. Every complex 
was modeled using the same absolute configuration for *tert*-leucine (*D* amino acid, *i.e.* **R** absolute 
configuration) for ease of comparison. 
Conformational searches were performed with CREST 2.12 at the GFN2-xTB//GFN-FF level using 
the ALPB solvation model for dichloromethane. The resulting conformational ensembles were 
refined via FIRECODE 1.0.0 at the GFN2-xTB/ALPB(CH2Cl2) level (RMSD threshold = 0.5 Å, energy 
window = 10 kcal/mol).
These ensembles were then subjected to a single-point energy calculation at the R2SCAN-3c/CPCM(CH2Cl2) level via ORCA 5.0.4 (keywords: Defgrid3). Structures within 5 kcal/mol 
(Electronic Energy) from the most stable were then optimized at the same level of theory. Vibrational 
analysis was carried out to confirm the nature of the stationary points (zero imaginary modes for 
equilibrium geometries, one imaginary mode for transition states) and to extract thermochemical 
corrections at the temperature of -40 °C (233.15 K). Structures within 3 kcal/mol from the most stable 
(Free Energy, -40 °C, R2SCAN-3c/CPCM(CH2Cl2)), after a similarity pruning process via FIRECODE 
(RMSD threshold = 0.5 Å), were subjected to single-point energy calculations at the ωB97M-V/def2
TZVPP/SMD(CH2Cl2) level of theory. The free energies used for qualitative comparisons are 
therefore obtained by the composite method ωB97M-V/def2-TZVPP/SMD(CH2Cl2)//R2SCAN-3c/CPCM(CH2Cl2) adding the electronic energy from the high-level single point calculation to the 
vibrational correction for free energy at the lower level.
