# Repository map

Every repository in this organization belongs to one category, and its name follows that
category's rule (NeutronOS ADR-037). Names are lowercase and hyphenated; a Python package
inside keeps its snake_case import name.

How to tell a library from the product: if someone could use it without NeutronOS, it is a
library (a solver, a toolkit). If it is the system people deploy and sign in to, it is the product.
The platform reaches a library through a separate `axiom-ext-<code>` adapter.

| Category | Name rule |
|---|---|
| Platform extension | `axiom-ext-<code-or-capability>` (one code or backend; Axiom ADR-044) |
| Product | `neutron-os-core`; standalone product extensions `neutron-os-<capability>` |
| Site | `<org>-<facility>-site` |
| Library | the package name (includes physics codes; usable without the product) |
| Facility twin or tool | `<site-id>-twin`, `<site-id>-<tool>` |
| Reference set | `progression-problems` (by scope as it grows) |
| Workspace | `<person>-workspace` or `<person>-<topic>`; never cited by product docs |
| Archived | kept read-only for the record |

The platform itself (`axiom-os`, `axiom-appkit`) lives in the B-Tree Labs organization.
Export-controlled repositories live only on the institutional GitLab and follow the same rule.

**Status as of 2026-11-09:** the renames below are done, except where a note says otherwise.
- GitHub redirects a renamed repository, so old clone URLs, issue links and badges keep working.
- Updating a local remote is optional:
  `git remote set-url origin git@github.com:UT-Computational-NE/<new-name>.git`.
- A repository whose owner prefers its current name keeps it, and the reason is listed here.
- New repositories follow this rule from the start.

## GitHub: UT-Computational-NE

| Repository | Category | Owner(s) | Note |
|---|---|---|---|
| neutron-os-core | Product | Ben Booth |  |
| program-tracker | Program tracker | Ben Booth | Program items, schedule and the program wiki; nothing export-controlled |
| ut-triga-twin | Facility twin | Ben Booth | Twin code on NeutronOS dtwin; to be reconciled with `netl_triga_dt` |
| neutron-os-shadow | Product extension | Nick Luciano | May fold into neutron-os-core, to discuss |
| ut-triga-site | Site | Ben Booth |  |
| acu-flowloop-site | Site | Ben Booth |  |
| vcu-flowloop-site | Site | Ben Booth |  |
| tamu-flowloop-site | Site | Ben Booth |  |
| axiom-ext-openmc | Platform extension | Ben Booth |  |
| axiom-ext-langgraph | Platform extension | Ben Booth |  |
| coreforge | Library | Cole Gentry | Renamed from `CoreForge` |
| mpactpy | Library | Cole Gentry, Nick Luciano | Renamed from `MPACTPy` |
| rocksteady | Library | Nick Luciano |  |
| carve | Library | Nick Luciano | Owner notes it may become a workspace, `nick-carve` |
| dt-tools | Library | Ben Collins | Renamed from `dt_tools` |
| flowloopdt | Library | Wesley Lao | Renamed from `FlowLoopDT` |
| flowforge | Library | Charlie Owen, Caleb Miller | Renamed from `FlowForge` |
| neutronics-neural-operators | Library | Wesley Lao | Renamed from `NeutronicsNeuralOperators` |
| CompartmentBateman.jl | Library (Julia) | Shayan Shahbazi | `.jl` is Julia's convention |
| check-trailing-whitespace | Library (tool) | (former member) |  |
| netl_triga_dt | Facility twin | Cole Gentry, Ben Collins | Rename held: `ut-triga-twin` is now a separate repository; the two are to be reconciled |
| ut-triga-fuel-loader | Facility tool | Nick Luciano | Renamed from `netl_triga_fuel_loader` |
| tamu-flowloop-twin | Facility twin | Wesley Lao, Cole Gentry | Renamed from `TexasAMFlowLoop` |
| bubble_flow_loop_tamu | Facility twin | Andres Fierro, Cole Gentry | Owner to decide: fold into `tamu-flowloop-twin`, or archive |
| progression-problems | Reference set | Cole Gentry | Renamed from `progression_problems` |
| syth | Library (physics code: a 1D thermal-hydraulics code for MSR analysis) | Braden Pecora, Charlie Owen |  |
| stncl | (owner to confirm) | Cole Gentry | Owner to confirm category |
| pinnicelln | Archived | Nick Luciano | Archived 2026-11-09 |
| veracity_microapps | (owner to confirm) | Wesley Lao, Cole Gentry | Owner to confirm: archive if no longer used |
| nick-neutronic-toys | Workspace | Nick Luciano | Renamed from `neutronic_toys` |
| andres-workspace | Workspace | Andres Fierro Lopez | Renamed from `AndrewWorkSpace` |
| andres-physor2026 | Workspace | Andres Fierro Lopez | Renamed from `physor2026_andrew` |
| ethan-workspace | Workspace | Ethan Rozak | Renamed from `EthanWorkspace` |
| msrr_depletion | Archived | (former member) | Archived 2026-11-09 |
| msrr_mpact_input_builder | Archived | (former member) | Archived 2026-11-09 |
| mpact_msrr_inputs | Archived | (former member) | Archived 2026-11-09 |
| omnibus_msrr_inputs | Archived | (former member) | Archived 2026-11-09 |
| albedo_demos | Archived | (former member) | Archived 2026-11-09 |
| SHIFT_Albedo_Calc | Archived | (former member) | Archived 2026-11-09 |

## Institutional GitLab

Only export-controlled content needs to stay here. Everything else moves to GitHub. Ben Booth signs off on whether content is export controlled.

| Repository | Category | Owner(s) | Content controlled? | Note |
|---|---|---|---|---|
| triga_digital_twin/triga_modsim_tools | Facility tool (controlled) | Nick Luciano | Yes, pending review: drives MPACT and MCNP, holds multigroup cross-section data and facility calibration data | Proposed name `ut-triga-modsim`, renamed only with its owner |
| triga_digital_twin/netl_triga_digital_twin | Program tracking | Ben Booth | No; some issues reference controlled details | Program tracking moved to GitHub `program-tracker`; this project is archived once the move finishes |
| msr_digital_twin_open | Program tracking (MSR) | Cole Gentry | No; one wiki page, MSR Progression Problems, is under review | Tracking moves to GitHub under Flow Loop Twins |
