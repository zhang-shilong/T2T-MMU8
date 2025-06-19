# T2T-MMU8 Q100 project

The complete sequence of a rhesus macaque. All resources are available on this site.

This project’s objective is to produce a telomere-to-telomere assembly of the rhesus macaque genome at **Q100** accuracy. Here, Q100 signifies that every 21‑mer in the final assembly is corroborated by Illumina or PacBio HiFi reads, guaranteeing an essentially error-free result when validated via the same k-mer–based strategy used in prior high-quality assemblies (e.g., the gold-standard human genome [T2T-CHM13](https://www.science.org/doi/10.1126/science.abj6987)).

To achieve this, we derived autosomes, chrX, and chrMT from a "haploid" parthenogenetic cell line (MMU2019108-1), while chrY was obtained from a separate individual (MMU1003063). The initial assembly combined PacBio HiFi data with ONT reads using Hifiasm’s integration mode. Afterward, contigs were manually assigned to chromosomes, and regions with complex tangles were further resolved through ONT R10.4.1–based local assemblies. We then applied a technology-customized polishing pipeline—addressing homopolymer errors, ONT strand bias and other known artifacts—to boost base accuracy while minimizing over-polishing. Finally, we generated a Q100 assembly.

As sequencing and assembly technologies continue to advance, we will update both the assembly and its annotations on an ongoing basis. If you identified any issues, please check [Issues](https://github.com/zhang-shilong/T2T-MMU8?tab=readme-ov-file#issues).

Check our sister reference genome: [T2T-MFA8](https://github.com/zhang-shilong/T2T-MFA8).

## Resources

### NCBI Genome

- T2T-MMU8v2.0: Coming soon.
- T2T-MMU8v1.0: [GCA_049350105.1](https://www.ncbi.nlm.nih.gov/datasets/genome/GCA_049350105.1/)

### Assembly

- [T2T-MMU8v2.0](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/v1.0/T2T-MMU8.v2.0.fasta.gz): unmasked, 20 autosomes + chrX + chrY + chrMT, **Q100** (Merqury QV, _k_=21);
- [T2T-MMU8v1.0](https://synplotter.sjtu.edu.cn/disk2/T2T-MMU8/v1.0/T2T-MMU8.v1.0.fasta.gz): unmasked, 20 autosomes + chrX + chrY + chrMT, Q80.11 (Merqury QV, _k_=21).

### Sequencing data

- MMU2019108-1 (autosomes, chrX and chrMT)
  - PacBio WGS: [SRR32560529](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560529), [SRR32560530](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560530), [SRR32560537](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560537) and [SRR32560538](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560538);
  - Nanopore WGS: [SRR32560528](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560528);
  - Illumina WGS: [SRR32560527](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560527).
- MMU1003063 (chrY)
  - PacBio WGS: [SRR32560524](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560524);
  - Nanopore WGS: [SRR32560525](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560525) and [SRR32560526](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560526);
  - Illumina WGS: [SRR27194597](https://www.ncbi.nlm.nih.gov/sra/?term=SRR27194597);
  - Hi-C: [SRR32560531](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560531), [SRR32560532](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560532), [SRR32560533](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560533), [SRR32560534](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560534), [SRR32560535](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560535) and [SRR32560536](https://www.ncbi.nlm.nih.gov/sra/?term=SRR32560536).

Sequencing data will be released upon manuscript submission.

### Annotations

Coming soon.

## Issues

Known issues are tracked in [GitHub issues](https://github.com/zhang-shilong/T2T-MMU8/issues). If you find any errors in the latest version, please raise an issue. Your feedback will help us build more perfect genomic resources.

## Previous versions

To avoid confusion, previous versions are not displayed on this page, but you can still access them through the links.

## License

All data is released to the public domain ([CC0](https://creativecommons.org/publicdomain/zero/1.0/)).

## Changelog

```
2025-06-19: Q100 release (T2T-MMU8v2.0).
2025-03-01: First release (T2T-MMU8v1.0).
```
