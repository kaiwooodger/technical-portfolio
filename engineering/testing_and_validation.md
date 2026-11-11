# Testing and Validation

## Claim hierarchy

The portfolio uses four evidence levels:

1. **Software verification:** the implementation behaves as specified under the test fixture.
2. **Numerical verification:** the method agrees with a manufactured, analytic or independently calculated reference within declared tolerance.
3. **Scientific validation:** the model agrees with relevant independent evidence for its intended scientific domain.
4. **Clinical validation:** the system is supported by commissioned workflows, patient evidence, governance and approval for the declared use.

Passing one level does not grant the next.

## Test design

### Unit tests

Cover geometry predicates, model equations, conversion functions, state transitions, schemas and failure handling.

### Integration tests

Exercise DICOM relationships, multi-stage scientific workflows, export and reload, adapter boundaries, report generation and checkpoint restart.

### Synthetic and manufactured references

Provide known geometry, conservation, analytic dose or solver behaviour without requiring private patient data.

### Regression tests

Freeze scientific results, release contracts, state behaviour and artifact identity. Tolerances are attached to the quantity and method rather than selected after observing the result.

### Independent comparison

Use manual calculations, external TPS evidence, independent mesh checks, pinned reference implementations or a separately compiled form of the deployed source.

## Quantitative examples

| Project | Verification result | Boundary retained |
| --- | --- | --- |
| ASCEND | 395 tests plus 40 subtests passed locally; retained CI passed 229 tests plus 28 subtests on each of six configurations; 69/70 cross-platform metric comparisons were exact and one differed by 8.88e-16; 19/19 available Eclipse dose comparisons passed | Eclipse evidence is one stored case; four of nine volume comparisons failed and eight D2 endpoints were not assessed; research software only |
| Digital twin | 39,664-triangle watertight mesh; byte-identical clean rerun | Engineering validation only |
| ESAPI | 375 trials; 336 valid; 39 correct no-lattice outcomes; zero geometry failures | Eclipse execution remains installation-specific |
| HEDOS adapter | 20 seeds × 100,000 particles per seed reproduced field and DVH modes | Does not validate human physiology |
| Non-local model | 65/70 sink endpoint shifts exceeded the combined 95% uncertainty band | Does not establish clinical benefit |

## Failure and uncertainty reporting

- Unavailable results are not forced to zero.
- Parameter conflicts remain visible rather than being averaged away.
- Small-sample descriptive results are labelled as such.
- Model outputs derived from the same chain are not treated as independent confirmations.
- Clinical-use blocks remain active in code, outputs and documentation.

[Back to portfolio](../README.md)
