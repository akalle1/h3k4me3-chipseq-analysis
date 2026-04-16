# H3K4me3 ChIP-seq Analysis in K562 Leukemia Cells

## Objective
Map active gene promoters in K562 chronic myelogenous 
leukemia cells using H3K4me3 ChIP-seq data.

## Data
- Source: ENCODE experiment ENCSR000AKY
- Cell line: K562 (CML, BCR-ABL positive)
- Treatment: ENCFF994FIB + ENCFF283HQV (rep2), 
             ENCFF156ECZ + ENCFF561WFK (rep3)
- Control: ENCFF000BWK (input)
- Read type: Single-end, 36nt

## Reference Genome
Biologically justified chromosome selection (chr8, chr9, 
chr17, chr19, chr22) based on known CML chromosomal 
abnormalities including the Philadelphia chromosome 
translocation (chr9/chr22).

## Pipeline
Snakemake workflow covering:
1. Quality control (FastQC, MultiQC)
2. Alignment (BWA)
3. Peak calling (MACS3)
4. Replicate concordance (bedtools)
5. Gene annotation (bedtools closest, RefGene)

## Results
- 325 high confidence consensus peaks
- Active promoters identified at leukemia-relevant genes 
  including RUNX1T1, IKZF3, BCL2L13
- Mapping rate: ~25% (subset reference limitation)

## Limitations
Subset reference genome used due to local compute 
constraints. Full genome analysis recommended for 
complete peak detection including BCR and ABL1 loci.

## Tools
Python, Bash, Snakemake, BWA, SAMtools, MACS3, 
FastQC, MultiQC, bedtools
