# Computational Algorithms for Invariant Reduction of Variational Forms

This repository contains the Maple implementation accompanying the paper **“Computational Algorithms for Invariant Reduction of Variational Forms”** by Kostya Druzhkov and Alexey Shevyakov.

The project develops computational procedures for reducing conservation laws, variational forms, and presymplectic structures under symmetries of partial differential equations. The accompanying worksheets provide complete worked examples for the evolution, descent, and contraction-based reduction procedures described in the paper.

## Requirements

- **Maple 2026** — used to develop and verify the worksheets.

The worksheets use Maple's `DifferentialGeometry` and `JetCalculus` packages. They are self-contained and do not require third-party or project-specific packages.

## Repository contents

| File | Model | Computation |
| --- | --- | --- |
| `algorithm.mw` | General implementation illustrated with the running example | Complete Maple implementation of the evolution reduction algorithm described in the paper and its appendix |
| `ws1_kdv_conservation_law_p0.mw` | KdV equation | Reduction of conservation laws (`p = 0`) under a travelling-wave symmetry |
| `ws2_eq33_examples1to4.mw` | Equation (3.3) in the paper | Cosymmetry, variational 1-form, and presymplectic-operator computations |
| `ws3_example5_evolution_algorithm_p2.mw` | Equation (3.3) in the paper | Evolution reduction algorithm for a presymplectic structure (`p = 2`) |
| `ws4_example6_pavlov_p0.mw` | Cotangent system of Pavlov’s equation | Conservation-law reduction (`p = 0`) under a higher symmetry |
| `ws5_example7_laplace_descent.mw` | Laplace equation | Descent algorithm for a presymplectic structure (`p = 2`) under rotations |
| `ws6_example8_euler_rotation.mw` | Two-dimensional incompressible Euler equations | Rotational reduction of the energy conservation law |

## Running the computations

1. Open a `.mw` file in Maple 2026.
2. Execute the worksheet from the beginning.
3. For `ws1`–`ws6`, check the numbered verification outputs.

Every computational stage in the six worked-example worksheets ends with a numbered checkpoint whose expected output is `0`. There are 38 checkpoints across this suite, so an unsuccessful step can be identified immediately.

The worksheets are organized as complete examples: each specifies its input data, carries out the relevant reduction procedure, verifies intermediate identities, and displays the resulting reduced object.

Potentials produced by a homotopy are defined modulo horizontally exact terms. Consequently, Maple may return a representative that differs from the formula printed in the paper by an exact term while representing the same cohomology class.

## Citation

If this repository contributes to your work, please cite it as follows:

```bibtex
@misc{DruzhkovShevyakov2026code,
  author       = {Druzhkov, Kostya and Shevyakov, Alexey},
  title        = {Computational Algorithms for Invariant Reduction of
                  Variational Forms: Maple Implementation of Examples},
  howpublished = {\url{https://github.com/afshevyakov/Computational-Algorithms-for-Invariant-Reduction-of-Variational-Forms}},
  year         = {2026},
  note         = {GitHub repository}
}
```

## Repository URL

<https://github.com/afshevyakov/Computational-Algorithms-for-Invariant-Reduction-of-Variational-Forms>
