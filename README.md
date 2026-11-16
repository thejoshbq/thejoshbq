# Joshua Boquiren

[![](https://img.shields.io/badge/@thejoshbq-grey?style=for-the-badge&logo=X)](https://x.com/thejoshbq)
[![](https://img.shields.io/badge/thejoshbq@proton.me-grey?style=for-the-badge&logo=proton)](mailto:thejoshbq@proton.me)

---

## 👨🏻‍💻 &nbsp;About Me

I'm a research software engineer at the [Otis Lab](https://www.otis-lab.org) at the Medical University of South Carolina. I build and maintain the software that runs our behavior and imaging experiments, from Arduino firmware up to desktop apps and analysis pipelines. Outside the lab I run my own Linux and network setup, and I'm working toward my CCNA.

### 🔬 Research software

- **[REACHER](https://github.com/Otis-Lab-MUSC/reacher)**: runs mouse behavior experiments, logging every lever press, lick and reward as it happens. In use at four labs across MUSC and the University of Alabama.<br>
  <sub>Python FastAPI server with REST and WebSocket streaming; drives Arduino chambers over a serial JSON protocol (pyserial); C++ firmware for five reinforcement schedules (fixed ratio, progressive ratio, variable interval, omission, Pavlovian); event timestamps aligned to microscope frames; zeroconf discovery for multi-rig setups. On PyPI as [`reacher2p`](https://pypi.org/project/reacher2p/).</sub>
- **[Labrynth](https://github.com/Otis-Lab-MUSC/labrynth)**: the app researchers open to set up and watch those experiments, on Windows, macOS and Linux.<br>
  <sub>React 19 + TypeScript front end (Vite, Zustand, Tailwind) over the REACHER backend; a prompt_toolkit terminal client for headless Raspberry Pi rigs; PyInstaller builds with bundled avrdude for firmware uploads; installers released through a GitHub Actions pipeline.</sub>
- **[ROIGBIV](https://github.com/thejoshbq/roigbiv)**: finds individual neurons in microscope movies of the brain and recognizes the same cells across recording days.<br>
  <sub>Suite2p motion correction and a truncated-SVD low-rank/sparse split, then a four-stage subtractive detection cascade (Cellpose spatial, Suite2p temporal, GCaMP template matching, tonic-neuron search), each behind a validation gate; cross-session matching with ROICaT embeddings and a calibrated logistic posterior; SQLAlchemy/Alembic registry; Dash/Plotly review app; PyTorch on CUDA.</sub>
- **[Axplorer](https://github.com/thejoshbq/axplorer)**: lines up brain activity with what the animal was doing and turns it into figures.<br>
  <sub>ingests `.npy` traces with Excel/MATLAB event logs; peri-event windows with ΔF/F, z-score and Gaussian smoothing applied per window; FastAPI backend with a React 19/TypeScript Plotly dashboard; HDF5 export.</sub>
- **[Phoxel Workbench](https://thejoshbq.github.io/phoxel-workbench/)**: one page that ties the whole toolset together, from rig hardware to final figure.<br>
  <sub>React 19 single-page app (React Router, Vite, Tailwind) on GitHub Pages, with an embedded demo of the control app.</sub>

### 🤖 Agents and infrastructure

- **[Revisionist](https://github.com/kedartech/revisionist)**: a multiplayer alternate-history strategy game where players take on real historical figures and an AI game master runs the rest of the world. AI coding agents write most of the code; I plan the work, set the rules they build under, and review what lands.<br>
  <sub>Python 3.12 engine with a deterministic referee for outcomes and a language model for narration and non-player characters; Typer CLI, Discord bot and web client; SQLite for solo play, Postgres for multiplayer; offline test mode with fixtures so the suite runs without model calls.</sub>
- **Self-hosted agent system**: a small team of AI agents I run on my own Linux server for scheduling, notes, briefings and code review.<br>
  <sub>Linux and systemd; scheduled jobs with delivery checks; a Git-backed knowledge base with commit hooks that reject writes outside each agent's lane; review gates before agent-written code merges; Tailscale-only remote access. A public write-up of the tooling and my home network setup is in progress.</sub>

### 📝 Publications

- Doncheck, E.M. et al. [Drug self-administration in head-fixed mice](https://doi.org/10.1038/s41596-026-01406-1). *Nature Protocols* (2026). *(See the [meta-repository](https://github.com/Otis-Lab-MUSC/doncheck-et-al-nature-protocols-2026).)*
- Manusky, L.M. et al. [Goal-directed actions and habits in head-fixed mice](https://doi.org/10.3389/fnbeh.2026.1751553). *Frontiers in Behavioral Neuroscience* (2026).
- Ward, A.L. et al. [A model of ethanol self-administration in head-fixed mice](https://doi.org/10.1111/acer.70132). *Alcohol: Clinical and Experimental Research* (2025).

### ✍️ Outside of code, I'm into:
  - Dates with my wife
  - Playing with my daughter
  - Hiking scenic trails
  - Disc golfing
  - *Cities: Skylines II* builds
  - Traveling to new places
  - Finding the best local coffee spots

💬 Unapologetically, pineapple belongs on pizza, and the only *correct* way to drink coffee is black.

<br>

*"The heavens declare the glory of God, and the sky above proclaims His handiwork." - Psalm 19:1*
