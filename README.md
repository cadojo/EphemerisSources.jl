[![Tests](https://github.com/JuliaAstro/EphemerisSources.jl/actions/workflows/Tests.yml/badge.svg)](https://github.com/JuliaAstro/EphemerisSources.jl/actions/workflows/Tests.yml)
[![Documentation](https://github.com/JuliaAstro/EphemerisSources.jl/actions/workflows/Documentation.yml/badge.svg)](https://juliaastro.org/EphemerisSources.jl/docs/stable)
[![JOSS](https://joss.theoj.org/papers/2ecaf389e70086ec2b560cb10f454267/status.svg)](https://joss.theoj.org/papers/2ecaf389e70086ec2b560cb10f454267)

# 🪐 `EphemerisSources.jl`

> [!IMPORTANT]
>
> The packages described in this documentation are not affiliated with or
> endorsed by NASA, JPL, Caltech, or any other organization! They are
> independently written packages by an astrodynamics hobbyist.

## Installation

Choose one of the following, or manually install one or more of the sub-packages
below.

```julia
pkg> add EphemerisSources
```

```julia
import Pkg
Pkg.add("EphemerisSources")
```

## Packages

This repository includes the top-level documentation for several solar system
ephemeris tools, all written with the Julia Programming Language. To learn
more about how to use these tools, consult the
[documentation website](https://juliaastro.org/EphemerisSources.jl).

| Package                                         | Description                                                                                                                           |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| [`EphemerisSources.jl`](lib/EphemerisSources)   | A top-level package which provides, and re-exports, names from `HorizonsAPI`, `HorizonsEphemeris`, `SPICEKernels`, and `SPICEBodies`. |
| [`HorizonsAPI.jl`](lib/HorizonsAPI)             | A precise JPL Horizons REST API client implementation, with keyword arguments for each acceptable parameter.                          |
| [`HorizonsEphemeris.jl`](lib/HorizonsEphemeris) | Convenience wrappers around the JPL Horizons REST API.                                                                                |
| [`SPICEKernels.jl`](lib/SPICEKernels)           | All [generic kernels](https://naif.jpl.nasa.gov/naif/data_generic.html) exported as variable constants.                               |
| [`SPICEBodies.jl`](lib/SPICEBodies)             | Idiomatic wrappers around SPICE and [`SPICE.jl`](https://github.com/JuliaAstro/SPICE.jl) methods.                                     |

## Paper

This repository holds a [JOSS](https://joss.theoj.org) submission under
[`paper/`](paper/paper.md). The paper is published to as a pre-print to
HTML, PDF, and Markdown on the [`gh-pages` branch](https://juliaastro.org/EphemerisSources.jl/paper).

## External Resources

Other Julia packages for interfacing with solar system ephemeris data are
available, including the three external packages below. These are not affiliated
with this repository, or this documentation's author.

| Package                                                                       | Description                                                        |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| [`Horizons.jl`](https://github.com/PerezHz/Horizons.jl)                       | Functions for spawning the `telnet` interface, and querying files. |
| [`SPICE.jl`](https://github.com/JuliaAstro/SPICE.jl)                          | A Julia interface to the `CSPICE` library provided by NASA JPL.    |
| [`Ephemerides.jl`](https://github.com/JuliaSpaceMissionDesign/Ephemerides.jl) | Ephemeris kernel reading and interpolation in pure Julia.          |
