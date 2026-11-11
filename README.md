# Technical Portfolio — Kai Woodger

Medical physics, computational modelling and evidence-led scientific software engineering.

[View the GitHub Pages portfolio](https://kaiwooodger.github.io/technical-portfolio/) · [Open the technical portfolio PDF](CV.pdf) · [ORCID](https://orcid.org/0009-0004-0626-4899)

This repository is the navigable evidence layer for work in radiotherapy physics, biological response modelling and computational medicine. It links to the source repositories rather than duplicating their code. Each project record uses the same structure: problem, methods and architecture, implementation, verification and validation, then results and limitations.

## Selected work

| Project | Technical focus | Inspectable evidence |
| --- | --- | --- |
| [ASCEND](projects/ASCEND.md) | DICOM-RT validation, lattice radiotherapy dosimetry, spatial PVDR, research radiobiology | [Source](https://github.com/kaiwooodger/ASCEND), tests, validation records, release documentation |
| [Non-local radiobiology](projects/Nonlocal_Radiobiology.md) | Reaction–diffusion signalling, TOPAS dose, vascular uptake, biological reinterpretation | [Published article](https://doi.org/10.1088/1361-6560/ae94dd), [reproducibility package](https://github.com/kair98-boop/SFRT) |
| [Radiotherapy digital twin](projects/Digital_Twin.md) | Anatomy, motion, circulation, transport, radiation, oxygen and biological interfaces | Deterministic release, mesh checks, conservation tests, checkpoint comparison |
| [ESAPI lattice placement](projects/ESAPI_Lattice_Placement.md) | C# treatment-planning automation and geometric verification | [Source](https://github.com/kaiwooodger/ESAPI-Script), 375-trial parameter sweep, local phantom evidence |
| [Additional systems](projects/Additional_Engineering_Projects.md) | VHEE simulation, biological audit, contouring QA and FastAPI service development | Quantitative outputs, archived test records and interface captures |

## Repository map

```text
technical-portfolio/
├── README.md
├── index.html
├── styles.css
├── CV.pdf
├── projects/
│   ├── ASCEND.md
│   ├── Nonlocal_Radiobiology.md
│   ├── Digital_Twin.md
│   ├── ESAPI_Lattice_Placement.md
│   └── Additional_Engineering_Projects.md
├── publications/
│   └── research_outputs.md
├── engineering/
│   ├── software_architecture.md
│   ├── testing_and_validation.md
│   └── computational_methods.md
├── assets/
│   ├── ascend_dashboard.png
│   ├── dose_distribution.png
│   └── validation_results.png
└── downloads/
    ├── Kai_Woodger_Technical_Portfolio.pdf
    └── Kai_Woodger_Technical_Portfolio.docx
```

## Evidence standard

- A software test establishes implementation behaviour under its stated fixture. It does not automatically validate a scientific model.
- A manufactured or synthetic reference establishes numerical or interface behaviour under controlled conditions. It does not establish patient realism.
- External clinical claims remain blocked until independent patient data, commissioned systems and the required governance are available.
- Every research system records its intended use, unresolved assumptions and prohibited interpretation.



## Rights

Portfolio text and visual presentation are copyright Kai Woodger. Linked project repositories retain their own licence terms. Public visibility does not grant a licence to reuse project code or research assets outside those terms.
