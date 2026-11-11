# Software Architecture

## Architectural principles

### Separate scientific logic from interfaces

Scientific calculations are implemented as services with explicit inputs and outputs. Desktop pages, command-line entry points and report generators call those services rather than duplicating algorithms.

### Make state and prerequisites visible

Complex research workflows are represented as ordered states. A calculation remains disabled until its prerequisites are satisfied. Failures identify the missing evidence instead of allowing partial or ambiguous execution.

### Preserve provenance

Production research outputs record the software version, exact source revision, configuration hash, parameter identities, input identity and artifact hashes where applicable.

### Use adapters at evidence boundaries

External systems such as TOPAS, XCAT, HEDOS, Eclipse ESAPI and TPS-derived DVH evidence are integrated through named adapters and data contracts. An adapter being executable does not imply that its external scientific claim has been validated.

## Architecture by project

| System | Structure | Key boundary |
| --- | --- | --- |
| ASCEND | Qt workstation, scientific services, validation state, structured export, report generation | Research radiobiology remains separate from physical validation and clinical claims |
| Digital twin | Anatomy, motion, circulation, transport, radiation, biology, scheduler and verification modules | Synthetic fixtures can grant engineering statuses but not patient or physiological validation |
| ESAPI automation | Candidate generation, geometry predicates, structure-set transaction and cleanup | Local geometry tests do not replace Eclipse installation validation |
| SFRT paper package | Cohort generation, TOPAS transport, biological solver, endpoints, uncertainty and figure pipeline | Public curated outputs exclude large raw transport intermediates but retain regeneration scripts |

## Release architecture

- Source, package and release identities are versioned together.
- Test, quality, repository-boundary and documentation checks run before release.
- Patient data, machine logs, case directories and private clinical exports stay outside public repositories.
- Licences and citation metadata remain project-specific.

[Back to portfolio](../README.md)
