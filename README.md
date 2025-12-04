# Spinning Synth: MCU + FPGA Audio System Website

This repository contains a Quarto website documenting an analog-style synthesizer that produces real-time audio controlled by a spinning gyroscope, keypad, and knobs. The system uses an STM32L432KC MCU and a Lattice iCE40 UP5K FPGA (UPduino v3.1).

## Structure

- `_quarto.yml` — site configuration (navbar, theme, output to `docs/`)
- `index.qmd` — project overview
- `technical.qmd` — architecture, block diagram, calculations, risks
- `mcu.qmd` — MCU design details (inputs, timing, generation)
- `fpga.qmd` — FPGA design details (DSP, filters, I/O)
- `bom.qmd` — bill of materials table
- `results.qmd` — measurements and outcomes
- `references.qmd` + `references.bib` — citations and links
- `team.qmd` — team bios and links
- `acknowledgements.qmd` — thanks
- `media.qmd` — demo video and photos

Add images to an `images/` folder as needed for the Media page.

## Building the Site

1. Install Quarto: see https://quarto.org
2. From the project root, run:

```bash
quarto preview
```

The site will be served locally and will hot-reload as you edit files.

## Publishing

The site outputs to the `docs/` directory (configured in `_quarto.yml`) which can be used with GitHub Pages. Push the repository and configure Pages to serve from the `docs/` folder on the `main` branch.

## Code Repositories

Include all project code (software and HDL) in this Git repository (e.g., `mcu/`, `fpga/`, and `scripts/` folders). Add READMEs in those subfolders to explain build steps and structure.


