<p align="center">
  <img src="https://raw.githubusercontent.com/UT-Computational-NE/.github/main/avatar.png" width="160" alt="The University of Texas at Austin" />
</p>

<h1 align="center">UT Computational Nuclear Engineering</h1>

<p align="center">
  <em>Computational nuclear engineering at UT Austin, Clarno group.</em>
</p>

---

We build open-source reactor modeling, neutronics and thermal-fluids tools in the
[Nuclear and Radiation Engineering program](https://me.utexas.edu/) at
The University of Texas at Austin, led by
[Dr. Kevin Clarno](https://sites.utexas.edu/clarno/).

The group's research areas are multiphysics coupling methods for nuclear reactor
simulation; multiscale neutronics, fuel performance and thermal-hydraulics;
design, optimization and analysis of advanced commercial and test reactors;
software integration for advanced nuclear manufacturing; and propagating
uncertainty through multiphysics applications.

## Open-source tools

| Repository | What it does |
|---|---|
| [**CoreForge**](https://github.com/UT-Computational-NE/CoreForge) | A collection of Python tools for setting up nuclear reactor models. |
| [**MPACTPy**](https://github.com/UT-Computational-NE/MPACTPy) | A Python API for the MPACT neutronics solver. |
| [**FlowForge**](https://github.com/UT-Computational-NE/FlowForge) | A frontend interface for multichannel thermal-fluids system solvers. |
| [netl_triga_fuel_loader](https://github.com/UT-Computational-NE/netl_triga_fuel_loader) | GUI and generator for per-location TRIGA fuel loading. It produces `specs.py` inputs for MPACT/OpenMC reactor models. |

All are Python and licensed BSD-3-Clause. Install any of them from source with `python -m pip install .`
(use `-e .[dev]` for development). Each repo's README covers testing (`pytest`), linting (`pylint`)
and formatting (`black`).

## Repository map

Every repository here belongs to one category and is named by that category's rule. See
[REPOSITORIES.md](https://github.com/UT-Computational-NE/.github/blob/main/REPOSITORIES.md)
for each repository's category, owner and name.

## Contributing

Contributions are licensed under each repository's license (BSD-3-Clause).
Open an issue or pull request on the relevant repository.

<sub>The University of Texas at Austin wordmark is a trademark of The University of Texas at Austin and is used in accordance with the university's brand standards.</sub>
