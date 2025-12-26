# Bioinformatics_Project_SafinaSherzaliKhan
Computational analysis of unknown DNA sequences using bioinformatics tools.
## Project summary

- **Objective:** Analyze an unknown DNA sequence to determine its species origin and characterize the encoded protein.

### Methods
1. Sequence similarity
    - NCBI BLASTN: identify closest nucleotide matches and taxonomic origin.
2. Gene and coding region identification
    - ORF Finder (NCBI): detect open reading frames and predict coding sequences.
    - ExPASy tools: validate translations and detect protein features from predicted ORFs.
3. mRNA sequence derivation
    - BioModel: obtain predicted mRNA sequence corresponding to the identified ORF.
4. RNA analysis
    - ExPASy and RNAfold (ViennaRNA): analyze mRNA properties and predict secondary structure.
5. Protein annotation and properties
    - UniProt and InterPro: annotate protein family, domains, and functional motifs.
    - ProtParam (ExPASy): compute molecular weight, pI, instability index, and other physicochemical properties.
6. Subcellular localization
    - TargetP and PSORT: predict likely subcellular localization signals and cellular compartment.
7. Phylogenetic and interaction analysis
    - CLUSTAL W: perform multiple sequence alignment and build a phylogenetic context.
    - STRING: explore predicted and known protein–protein interactions.

### Results
- Taxonomic assignment: the sequence best matches Solanum lycopersicum (tomato).
- Protein identification: the translated product corresponds to a small Heat Shock Protein (sHSP) of approximately 20 kDa (Heat Shock Protein 20 family).
- Supporting evidence: high BLASTN similarity to S. lycopersicum genomic/transcript sequences, ORF-predicted coding region translating to an sHSP-like sequence with conserved HSP motifs (InterPro/UniProt), physicochemical properties consistent with known sHSP20 proteins (ProtParam), predicted cytosolic/chaperone localization signals (TargetP/PSORT), and clustering with plant sHSP sequences in CLUSTAL W alignments; STRING analysis indicates interactions consistent with stress-response chaperone networks.