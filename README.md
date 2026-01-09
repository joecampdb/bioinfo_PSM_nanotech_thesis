# nanotech_thesis
[jac_enzo_thesis.docx](https://github.com/user-attachments/files/22586307/jac_enzo_thesis.docx)

# Characterizing the Bond Angle Distribution of DNA Origami Nanoswitches

This repository contains the research, data, and simulation workflows from my master’s thesis:  
**Characterizing the Bond Angle Distribution of DNA Origami Nanoswitches (2025)**

---

## Overview

DNA origami is one of the most powerful approaches in structural DNA nanotechnology, allowing researchers to build nanoscale devices with programmable shapes and functions.  
My thesis focuses on a fundamental mechanical property of these devices: **bond angle distributions across flexible linker sequences**.

I set out with a simple hypothesis: longer linker regions should increase conformational flexibility.  
But the results told a different story. Using coarse-grained molecular dynamics, I discovered that **longer linkers actually reduce angular variance**, producing a stabilizing effect rather than greater flexibility.

This project documents that journey—from design and modeling to simulation and analysis.

---

## Key Contributions

- Developed DNA origami nanoswitch models with linker lengths of 10, 20, 30, and 40 nucleotides  
- Simulated their conformational behavior with oxDNA in LAMMPS (Stable Release Aug 2024)  
- Quantified bond angle distributions and analyzed standard deviation trends  
- Found an inverse relationship between linker length and angular variance, following an exponential decay curve  
- Interpreted this result in the context of polymer physics, entropic effects, and design principles for nanoscale devices  

---

## Methods and Tools

- **Modeling**: oxView + TacoxDNA converter  
- **Simulation**: LAMMPS with oxDNA2 force field  
- **Analysis**: Python + VMD for bond angle measurements  
- **Data**: Linker lengths ranging from 10 to 40 nt  
- **Metrics**: Standard deviation (σ) of bond angle distributions  

---

## Results Snapshot

| Linker Length (nt) | σ (Bond Angle Std. Dev.) |
|--------------------|---------------------------|
| 10                 | 6.24°                     |
| 20                 | 3.74°                     |
| 30                 | 2.68°                     |
| 40                 | 2.27°                     |

**Trend:** Longer linkers stabilize nanoswitch geometry rather than destabilize it.

---

## Why It Matters

Understanding the mechanics of DNA origami nanoswitches is key to:  
- Drug delivery: ensuring payloads are released only under the right conditions  
- Biosensing: tuning sensitivity by engineering hinge flexibility  
- DNA computing: designing predictable conformational logic gates  

This project helps bridge design theory with simulation insight, offering principles that can guide the rational design of future DNA nanodevices.


---

## How to Reproduce

1. Install **LAMMPS (Aug 2024 release)** with `cgdna` package enabled  
2. Generate input data via TacoxDNA and import into LAMMPS  
3. Run MD simulations with provided `in.*` scripts  
4. Analyze trajectories with Python scripts in `analysis/` to reproduce plots and statistics  

---

## References

This thesis builds on foundational work in DNA origami nanotechnology, including:  
- Rothemund, P.W.K. (2006). Folding DNA to create nanoscale shapes and patterns. *Nature*  
- Castro, C.E. et al. (2015). Programmable motion of DNA origami mechanisms. *PNAS*  
- Doye, J.P.K. et al. (2013). Coarse-graining DNA for simulations of DNA nanotechnology. *PCCP*  

(Full reference list in `thesis/`.)

---

## Author

**Joseph Campagna**  
M.S. Thesis, 2025  
Advisor: Vincenzo Carnevale





