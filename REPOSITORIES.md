# Repository map

Every repository in this organization belongs to one category, and its name follows that
category's rule (NeutronOS ADR-037). Names are lowercase and hyphenated; a Python package
inside keeps its snake_case import name.

| Category | Name rule |
|---|---|
| Platform extension | `axiom-ext-<code-or-capability>` (one code or backend; Axiom ADR-044) |
| Product | `neutron-os-core`; standalone product extensions `neutron-os-<capability>` |
| Site | `<org>-<facility>-site` |
| Library | the package name |
| Facility twin or tool | `<site-id>-twin`, `<site-id>-<tool>` |
| Reference set | `progression-problems` (by scope as it grows) |
| Workspace | `<person>-workspace` or `<person>-<topic>`; never cited by product docs |
| Archived | kept read-only for the record |

The platform itself (`axiom-os`, `axiom-appkit`) lives in the B-Tree Labs organization.
Export-controlled repositories live only on the institutional GitLab and follow the same rule.

**Status as of 2026-10-26:** proposed names are pending each owner's agreement.
- GitHub redirects a renamed repository, so old clone URLs, issue links and badges keep
  working.
- Updating a local remote is optional:
  `git remote set-url origin git@github.com:UT-Computational-NE/<new-name>.git`.
- A repository whose owner prefers its current name keeps it, and the reason is listed here.

## GitHub: UT-Computational-NE

| Repository | Category | Owner(s) | Proposed name |
|---|---|---|---|
| neutron-os-core | Product | Ben Booth | (unchanged) |
| neutron-os-shadow | Product extension | Nick Luciano | (unchanged; may fold into neutron-os-core, to discuss) |
| ut-triga-site | Site | Ben Booth | (unchanged) |
| acu-flowloop-site | Site | Ben Booth | (unchanged) |
| vcu-flowloop-site | Site | Ben Booth | (unchanged) |
| tamu-flowloop-site | Site | Ben Booth | (unchanged) |
| axiom-ext-openmc | Platform extension | Ben Booth | (unchanged) |
| axiom-ext-langgraph | Platform extension | Ben Booth | (unchanged) |
| CoreForge | Library | Cole Gentry | `coreforge` |
| MPACTPy | Library | Cole Gentry, Nick Luciano | `mpactpy` |
| rocksteady | Library | Nick Luciano | (unchanged) |
| carve | Library | Nick Luciano | (unchanged) |
| dt_tools | Library | Ben Collins | `dt-tools` |
| FlowLoopDT | Library | Wesley Lao | `flowloopdt` |
| FlowForge | Library | Charlie Owen, Caleb Miller | `flowforge` |
| NeutronicsNeuralOperators | Library | Wesley Lao | `neutronics-neural-operators` |
| CompartmentBateman.jl | Library (Julia) | Shayan Shahbazi | (unchanged; `.jl` is Julia's convention) |
| check-trailing-whitespace | Library (tool) | (former member) | (unchanged) |
| netl_triga_dt | Facility twin | Cole Gentry, Ben Collins | `ut-triga-twin` |
| netl_triga_fuel_loader | Facility tool | Nick Luciano | `ut-triga-fuel-loader` |
| TexasAMFlowLoop | Facility twin | Wesley Lao, Cole Gentry | `tamu-flowloop-twin` |
| bubble_flow_loop_tamu | Facility twin | Andres Fierro, Cole Gentry | owner to decide: fold into `tamu-flowloop-twin`, or archive |
| progression_problems | Reference set | Cole Gentry | `progression-problems` |
| syth | (owner to confirm) | Braden Pecora, Charlie Owen | by its category once confirmed |
| stncl | (owner to confirm) | Cole Gentry | by its category once confirmed |
| pinnicelln | (owner to confirm) | Nick Luciano | library name, or archive |
| veracity_microapps | (owner to confirm) | Wesley Lao, Cole Gentry | archive, if no longer used |
| neutronic_toys | Workspace | Nick Luciano | `nick-neutronic-toys` |
| AndrewWorkSpace | Workspace | Andres Fierro Lopez | `andres-workspace` |
| physor2026_andrew | Workspace | Andres Fierro Lopez | `andres-physor2026` |
| EthanWorkspace | Workspace | Ethan Rozak | `ethan-workspace` |
| msrr_depletion | Archived | (former member) | archive |
| msrr_mpact_input_builder | Archived | (former member) | archive |
| mpact_msrr_inputs | Archived | (former member) | archive |
| omnibus_msrr_inputs | Archived | (former member) | archive |
| albedo_demos | Archived | (former member) | archive |
| SHIFT_Albedo_Calc | Archived | (former member) | archive |

## Institutional GitLab (export controlled)

These follow the same rule. They're renamed only with their owners, at a natural break.

| Repository | Category | Owner(s) | Proposed name |
|---|---|---|---|
| triga_digital_twin/triga_modsim_tools | Facility tool (controlled) | Nick Luciano | `ut-triga-modsim` |
| triga_digital_twin/netl_triga_digital_twin | Program tracker | Ben Booth | (unchanged) |
| msr_digital_twin_open | Facility twin (controlled) | Cole Gentry | to discuss with the MSR work |
