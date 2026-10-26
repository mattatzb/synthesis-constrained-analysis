# Synthesis-constrained analysis

This repository brings together the analyses supporting the accompanying paper
on synthesis-constrained molecular design. It contains two projects, each with
its own environment, inputs, analysis commands, tests, and reference results.

- **[Retrosynthesis benchmark](syntheseus_benchmark/README.md)**
  (`syntheseus_benchmark/`): prepares the pesticide target dataset and compares
  retrosynthesis models and search algorithms. Use it to reproduce the benchmark
  summary tables and figure from archived search results, or to rerun searches.
- **[Green chemistry vs docking analysis](green_vs_docking/README.md)**
  (`green_vs_docking/`): evaluates green-chemistry metrics for saved synthetic
  routes and compares them with docking scores. Use it to reproduce the
  green-chemistry summary tables and figure, either from saved comparisons or
  by rescoring the archived routes.

Conda is required to create and manage the project environments. Install it
before following the steps below; see the
[Conda installation instructions for Linux](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html).

To use either project:

1. Open its subfolder from this repository's root:

   ```bash
   cd syntheseus_benchmark
   # Or: cd green_vs_docking
   ```

2. Follow that project's README to create and activate its environment and
   download the required archived inputs.
3. Run its reproduction commands and verification checks from that subfolder.

Paths and references to the **repository root** in each project's README refer
to that project's subfolder. Extract its downloaded archives there, preserving
the documented directory structure.

Both projects support analysis of saved results. Their READMEs describe the
additional dependencies for route rescoring or new searches, along with detailed
commands, output locations, and reproducibility limits.
