# Research Outputs

## Peer-reviewed publication

### Biology-informed reinterpretation of lattice radiotherapy using non-local bystander signalling and anatomy-aware vascular sink modelling

Kai Woodger. *Physics in Medicine & Biology*. 2026;71(16). Published online 18 August 2026.

- [DOI: 10.1088/1361-6560/ae94dd](https://doi.org/10.1088/1361-6560/ae94dd)
- [PubMed PMID 42551488](https://pubmed.ncbi.nlm.nih.gov/42551488/)
- [Reproducibility package](https://github.com/kair98-boop/SFRT)
- ORCID: [0009-0004-0626-4899](https://orcid.org/0009-0004-0626-4899)

### Contribution

The work developed and tested a hypothesis-generating computational framework for biological reinterpretation of lattice radiotherapy. It combined TOPAS-derived dose, a reaction–diffusion representation of ROS-like and cytokine-like signalling, anatomy-aware vascular uptake, controlled synthetic head-and-neck geometries, uncertainty analysis and falsification controls.

### Key results

- Cohort-mean PVDR-like ratio: 1.817 physical-only, 1.292 biology-informed without vascular uptake and 1.270 with anatomical uptake.
- Rank changes: 5/10 cases for no-sink versus physical-only, 6/10 for with-sink versus physical-only and 2/10 for with-sink versus no-sink.
- Biology-added brainstem-adjacent burden flags: 2/10 cases.
- Sink-related endpoint shifts exceeding the combined 95% uncertainty band: 65/70.
- Noise-qualified sink-driven rank changes: 0/10.

### Evidence boundary

The study is computational and hypothesis-generating. It requires patient-derived RTDOSE/RTSTRUCT data, realistic vascular segmentation and experimental validation before clinical use.

## Software and reproducibility outputs

### ASCEND 2.4.2

A public Qt 6 workstation for DICOM-RT validation, lattice radiotherapy dosimetry and research radiobiology.

- [Source repository](https://github.com/kaiwooodger/ASCEND)
- Versioned validation status, release records, synthetic references and repository checks
- Citation metadata in the project repository

### ESAPI lattice sphere placement

A public C# implementation with independent synthetic geometry evidence.

- [Source repository](https://github.com/kaiwooodger/ESAPI-Script)
- 375-trial parameter sweep
- Worked phantom and regression evidence

## Technical report

The [12-page technical portfolio](../downloads/Kai_Woodger_Technical_Portfolio.pdf) records major systems, quantitative verification, images, evidence boundaries and capability mapping.

[Back to portfolio](../README.md)
