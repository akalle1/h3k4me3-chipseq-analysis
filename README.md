# H3K4me3 ChIP-seq Analysis Pipeline

## Project Status
**In Development** —Pipeline runs end-to-end. Next: analyze results, annotate peak regions, and inspect signal tracks in IGV.

## Overview
Automated Snakemake workflow for identifying active gene promoters via H3K4me3 ChIP-seq analysis.

## Technical Stack
- **Workflow**: Snakemake
- **Languages**: Python, Bash  
- **Tools**: BWA-MEM, SAMtools, MACS3, FastQC, MultiQC
- **Platform**: WSL (Ubuntu 24.04)

## Pipeline Architecture
```
Raw FASTQ → QC → Alignment → Sorting → Indexing → Peak Calling → Reports
```

## Current Status
- ✅ Pipeline structure complete
- ✅ All rules functional with test data
- ✅ real ENCODE data download
- ⏳ Results validation pending

## Next Steps
- Validate peak calling results
- Generate visualization outputs
