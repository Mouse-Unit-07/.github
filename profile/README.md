# Mouse Unit 07 GitHub Organization

All Mouse Unit 07 development related repos, files, etc live here!

## `sketches`

- Just for brainstorming and light reference (not strict documentation)
  - As per *UML Distilled*, the idea is that work should document itself
- Software architecture sketch
  - Dependency diagram of all software repos and parts
- Development tools sketch
  - Dependency/deployment diagram of all tools and platforms in use

## `hardware-`

- `hardware-motherboard`
  - Design explanation for micromouse motherboard
  - PDF's for schematics, layouts, mechanical drawings
- `hardware-uart-bridge`
  - Sparkfun Bluetooth UART bridge module documentation

## `software-`

- Layers that make up the micromouse firmware include:
  - `software-application`
  - `software-maze-solver`
  - `software-mouse-driver`
  - `software-device-drivers`
  - `software-hardware-abstraction-layer`
  - `software-at32uc3l0256-drivers`
  - `software-runtime-diagnostics`
  - Where `software-application` is the topmost layer, and `software-at32uc3l0256-drivers` is the lowest
- `software-development-environment`
  - Uniform software development environment to build all software projects w/ CMake
  - Exists as a Docker container substitute, w/ a Python script to invoke builds in place of a CI pipeline
- `software-mouse-simulator`
  - A C++ project to simulate micromouse hardware (`software-device-drivers`) to find the optimal feedback control constants and navigation algorithms to implement in `software-mouse-driver`

## `mechanical-`

- `mechanical-3d-parts`
  - Storage for 3D models made w/ Fusion 360
  - Migrated out of hardware repo to reduce clutter in hardware repos

## `experiment-`

- Experiments that are worth documenting, software/hardware or anything else
- `experiment-software-hello-world`
  - A simple project to reference as a software repo compatible w/ `software-development-environment`
- `experiment-software-repeat-hello-world`
  - Same concept as `experiment-software-hello-world`, except this project has a dependency
- `experiment-software-repeat-hello-world-cpp`
  - Same as `experiment-software-repeat-hello-world`, but in C++
- `experiment-software-build-environment`
  - What led to the final uniform build environment repo to act as a Docker container substitute

## Supplement

- `fundamental-engineering-notes`
  - Ryuichi's engineering notes from books, school, and work
- `team-guides`
  - Guides for team members including development rules, micromouse assembly guide, etc
- `discussions`
  - Development logs, troubleshooting w/ links to references, etc to be formally documented later if needed
- `reference-documents`
  - Helpful micromouse related read-only documentation (old IEEE documents, links to other micromouse efforts, etc)
- Archived/read-only repos
  - `Micromouse_2024`
  - `mouse-7-monorepo`

## Projects

- Mouse Unit 07 Kanban
  - A Kanban style log/billboard for task allocation and management

## External Links

Everything (documentation, code, etc) should be under this GitHub organization whenever possible, but external items include:

- Fusion 360
  - 3D model and schematic/PCB development
  - Private due to license requirement
- Discord
  - All threads that don't need to be tracked
  - Private
- YouTube
  - www.youtube.com/@MouseUnit07
  - Storage for all videos due to GitHub storage limitation
  - Private/unlisted unless there're videos to share w/ the universe
