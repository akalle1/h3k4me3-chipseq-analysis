# H3K4me3 ChIP-seq Analysis Pipeline

## Project Status
🚧 **In Development** - Currently tested with simulated data

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
- ⏳ Awaiting real ENCODE data download
- ⏳ Results validation pending

## Next Steps
- Download ENCODE K562 H3K4me3 data (chr22)
- Validate peak calling results
- Generate visualization outputs
