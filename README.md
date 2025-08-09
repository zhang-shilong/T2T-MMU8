# T2T-MMU8 QV100 project

The complete sequence of a rhesus macaque (_Macaca mulatta_). All resources are available on this site.

This project’s objective is to produce a telomere-to-telomere assembly of the rhesus macaque genome at **QV100** accuracy. Here, QV100 signifies that every 21‑mer in the final assembly is corroborated by Illumina or PacBio HiFi reads, guaranteeing an essentially error-free result when validated via the same _k_-mer–based strategy used in prior high-quality assemblies (e.g., the gold-standard human genome [T2T-CHM13](https://www.science.org/doi/10.1126/science.abj6987)).

To achieve this, we derived autosomes, chrX, and chrMT from a "haploid" parthenogenetic cell line (MMU2019108-1), while chrY was obtained from a separate individual (MMU1003063). The initial assembly combined PacBio HiFi data with ONT reads using Hifiasm’s integration mode. Afterward, contigs were manually assigned to chromosomes, and regions with complex tangles were further resolved through ONT R10.4.1–based local assemblies. We then applied a technology-customized polishing pipeline—addressing homopolymer errors, ONT strand bias and other known artifacts—to boost base accuracy while minimizing over-polishing. Finally, we generated a QV100 assembly.

As sequencing and assembly technologies continue to advance, we will update both the assembly and its annotations on an ongoing basis. If you identified any issues, please check [Issues](https://github.com/zhang-shilong/T2T-MMU8?tab=readme-ov-file#issues).

Check our sister reference genome: [T2T-MFA8](https://github.com/zhang-shilong/T2T-MFA8).

## Resources

### NCBI Genome

- **T2T-MMU8v2.0**: [GCA_049350105.2](https://www.ncbi.nlm.nih.gov/datasets/genome/GCA_049350105.2/)
- T2T-MMU8v1.0: [GCA_049350105.1](https://www.ncbi.nlm.nih.gov/datasets/genome/GCA_049350105.1/)

### UCSC Track Hub

- **T2T-MMU8v2.0**
  - Hub connect: [US](https://genome.ucsc.edu/cgi-bin/hgTracks?hubUrl=https://synplotter.sjtu.edu.cn/disk2/T2TMacaqueHub/hub.txt&genome=hub_605438_T2T-MMU8v2.0&position=lastDbPos) / [Euro](https://genome-euro.ucsc.edu/cgi-bin/hgTracks?hubUrl=https://synplotter.sjtu.edu.cn/disk2/T2TMacaqueHub/hub.txt&genome=hub_605438_T2T-MMU8v2.0&position=lastDbPos) / [Asia](https://genome-asia.ucsc.edu/cgi-bin/hgTracks?hubUrl=https://synplotter.sjtu.edu.cn/disk2/T2TMacaqueHub/hub.txt&genome=hub_605438_T2T-MMU8v2.0&position=lastDbPos)
  - [Hub URL](https://synplotter.sjtu.edu.cn/disk2/T2TMacaqueHub/hub.txt)

### Assembly

- [**T2T-MMU8v2.0**](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.fasta.gz): unmasked, 20 autosomes + chrX + chrY + chrMT, complete and near-perfect genome ([Merqury](https://github.com/marbl/merqury) estimated QV = 100, _k_ = 21; GCI = 100; and no unassembled / collapsed regions and unplaced contigs)
- [T2T-MMU8v1.0](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v1.0/T2T-MMU8v1.0.fasta.gz): unmasked, 20 autosomes + chrX + chrY + chrMT, complete genome (Merqury estimated QV = 80.11, _k_ = 21; and no unplaced contigs)

### Sequencing data

- MMU2019108-1 (autosomes, chrX and chrMT)
  - PacBio WGS: [SRR32560529](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560529), [SRR32560530](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560530), [SRR32560537](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560537) and [SRR32560538](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560538)
  - ONT Ultra-long WGS (HAC): [SRR32560528](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560528)
  - ONT Ultra-long WGS (SUP):
    - R10.4.1 SUP: [SRR34896721](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896721), [SRR34896722](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896722), [SRR34896723](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896723), [SRR34896724](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896724), [SRR34896726](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896726) and [SRR34896727](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896727)
    - R9.4.1 SUP: [SRR34896719](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896719) and [SRR34896720](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896720)
  - Illumina WGS: [SRR32560527](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560527) and [SRR34896718](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896718)
- MMU1003063 (chrY)
  - PacBio WGS: [SRR32560524](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560524)
  - ONT Ultra-long WGS (HAC): [SRR32560525](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560525) and [SRR32560526](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560526)
  - ONT Ultra-long WGS (SUP):
    - R10.4.1 SUP: [SRR34896717](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896717) and [SRR34896725](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896725)
  - Illumina WGS: [SRR27194597](https://www.ncbi.nlm.nih.gov/sra/?term=SRR27194597) and [SRR34896692](https://www.ncbi.nlm.nih.gov/sra/?term=SRR34896692)
  - Hi-C: [SRR32560531](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560531), [SRR32560532](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560532), [SRR32560533](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560533), [SRR32560534](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560534), [SRR32560535](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560535) and [SRR32560536](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560536)

Sequencing data will be released upon manuscript submission.

<hr>

⬇️ **The following annotations are based on T2T-MMU8v2.0.**

### Gene annotation

- NCBI RefSeq: under processing
- [Liftoff from T2T-MFA8v1.1 (GCF_037993035.2-RS_2025_03)](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.liftoff-RefSeq_GCF_037993035.2_AXY-Mmul_10_M.gff3.gz)
- [Liftoff from Mmul_10 (GCF_003339765.1 Annotation Release 103)](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.liftoff-RefSeq_Mmul_10.gff3.gz)

### Sequence profile

- Base percentage: [AT](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.pct_AT_w50.bigwig) / [GC](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.pct_GC_w50.bigwig) (50-bp windows) // [AT](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.pct_AT_w128.bigwig) / [GC](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.pct_GC_w128.bigwig) (128-bp windows)
- Microsatellites: [AT](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.microsatellite_AT_w128.bigwig) / [GA](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.microsatellite_GA_w128.bigwig) / [GC](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.microsatellite_GC_w128.bigwig) / [TC](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.microsatellite_TC_w128.bigwig) (128-bp windows)

### Mappability

- [21-mer with no error](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.k21_e0_mappability.bigwig)
- [31-mer with no error](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.k31_e0_mappability.bigwig)

### Repeat annotation

- [Alpha satellites](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.alpha_satellite.bed)
- Segmental duplications: [native bed](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.SDs.bed.gz) / [merged bed](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.SDs.merged.bed.gz)
- Tandem repeats: [native bed](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.TRF.bed.gz) / [merged bed](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.TRF.merged.bed.gz)
- RepeatMasker: [native out](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.RepeatMasker-4.1.9.Dfam-3.9_full.RepeatModeler.out.gz) / [native bed](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.RepeatMasker-4.1.9.Dfam-3.9_full.RepeatModeler.bed.gz) / [merged bed](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.RepeatMasker-4.1.9.Dfam-3.9_full.RepeatModeler.merged.bed.gz) // [RepeatModeler family fasta](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.RepeatModeler_families.fasta)
- [WindowMasker (with SDust)](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.windowmasker_SDust.bed.gz)
- [Longdust](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.longdust.bed.gz)
- [NUMT](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.NUMTs.bed)
- [G-quadruplexes](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.G4Hunter_w25s1.5.merged.bed.gz)
- [Telomeres](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.telomere.bed)
- [rDNA models](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.rDNA.bed)

### Epigenetic profile

- [CpG islands](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.cpg_islands.bed)
- CpG methylation from ONT: [autosomes + chrX, traditional preset](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/T2T-MMU8v2.0.AXM.Nanopore_R10_5mCG.ge5.bigwig)

### Liftover chains

- Among versions
  - T2T-MMU8v1.0: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-T2T-MMU8v1.0.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-T2T-MMU8v1.0.swapped.chain)
- Human (_Homo sapiens_)
  - T2T-CHM13v2.0: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-T2T-CHM13v2.0.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-T2T-CHM13v2.0.swapped.chain)
- Crab-eating macaque (_Macaca fascicularis_)
  - T2T-MFA8v1.1: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-T2T-MFA8v1.1.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-T2T-MFA8v1.1.swapped.chain)
- Rhesus macaque (_Macaca mulatta_)
  - Mmul_10: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-Mmul_10.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-Mmul_10.swapped.chain)
  - rheMacS_v1.0: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-rheMacS_1.0.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-rheMacS_1.0.swapped.chain)
- Chimpanzee (_Pan troglodytes_)
  - NHGRI_mPanTro3-v2.0_pri: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPanTro3_v2.0_pri.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPanTro3_v2.0_pri.swapped.chain)
- Bonobo (_Pan paniscus_)
  - NHGRI_mPanPan1-v2.0_pri: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPanPan1_v2.0_pri.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPanPan1_v2.0_pri.swapped.chain)
- Gorilla (_Gorilla gorilla_)
  - NHGRI_mGorGor1-v2.0_pri: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mGorGor1_v2.0_pri.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mGorGor1_v2.0_pri.swapped.chain)
- Bornean orangutan (_Pongo pygmaeus_)
  - NHGRI_mPonPyg2-v2.0_pri: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPonPyg2_v2.0_pri.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPonPyg2_v2.0_pri.swapped.chain)
- Sumatran orangutan (_Pongo abelii_)
  - NHGRI_mPonAbe1-v2.0_pri: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPonAbe1_v2.0_pri.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mPonAbe1_v2.0_pri.swapped.chain)
- Siamang (_Symphalangus syndactylus_)
  - NHGRI_mSymSyn1-v2.0_pri: [forward](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mSymSyn1_v2.0_pri.chain) / [swapped](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/liftover_chains/ref-T2T-MMU8v2.0_qry-mSymSyn1_v2.0_pri.swapped.chain)

All chains were generated with [transanno](https://github.com/informationsea/transanno) minimap2chain. `Forward` means using T2T-MMU8v2.0 as reference genome.

### Non-syntenic regions

- Rhesus macaque (_Macaca mulatta_)
  - [Mmul_10](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/non_syntenic_regions/non_syntenic_regions.Mmul_10.bed)
  - [rheMacS_1.0](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/release_v2.0/non_syntenic_regions/non_syntenic_regions.rheMacS_1.0.bed)

## Issues

Known issues are tracked in [GitHub issues](https://github.com/zhang-shilong/T2T-MMU8/issues). If you find any errors in the latest version, please raise an issue. Your feedback will help us build more perfect genomic resources.

## License

All data is released to the public domain ([CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/)).

## Citation

We would appreciate if you would acknowledge and cite our paper:

Zhang, S. _et al_. A complete and near-perfect rhesus macaque reference genome: lessons from subtelomeric repeats and sequencing bias. _bioRxiv_ (2025). https://doi.org/10.1101/2025.08.04.668424

## Changelog

```
2025-08-08: UCSC track hub for T2T-MMU8v2.0.
2025-08-05: Annotation release for T2T-MMU8v2.0.
2025-06-19: QV100 release (T2T-MMU8v2.0).
2025-03-01: First release (T2T-MMU8v1.0).
```
