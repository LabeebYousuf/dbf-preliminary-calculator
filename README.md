# DBF Preliminary Calculator (MATLAB)

A MATLAB calculator for preliminary aircraft performance calculations and airfoil data visualization for the AIAA Design/Build/Fly competition.

This repo contains:
- **Airfoil plotting/analysis** from provided airfoil polar data (`.csv` files in `data/`)
- **Preliminary flight/performance calculations** to support early design decisions (trade-study style workflow)
- Exported outputs (PDF) for quick viewing (in `docs/`)

---

## Repository Structure

```text
.
├── src/        # MATLAB code (scripts / live scripts)
├── data/       # Airfoil polar / lookup CSV files
├── docs/       # Exported results (PDF/HTML), reports, snapshots
├── .gitignore
└── README.md

---

## Requirements

- MATLAB (recommended: R2021b or newer; older versions will not work)
- No special toolboxes assumed

---

## Quick Start

1. **Clone this repository**
   - Download as ZIP, or clone via Git:
     ```bash
     git clone https://github.com/LabeebYousuf/dbf-preliminary-calculator.git
     ```

2. **Open MATLAB and set the project folder**
   - In MATLAB, navigate to the repo folder (the one containing `src/`, `data/`, `docs/`).

3. **Run the scripts**
   - Airfoil plotting / analysis:
     - Open and run: `src/dbfAirfoilPlotter.m` (or `.mlx` if included)
   - Flight/performance calculations:
     - Open and run: the flight calculations script in `src/` (e.g., `dbfFlightCalculations...`)

> Tip: If you’re using Live Scripts (`.mlx`), you can run section-by-section and export results to PDF for portfolio viewing.

---

## Data Files

Airfoil polar / lookup data lives in `data/` and is read by the plotting and/or performance scripts.

Example files:
- `data/naca4412.csv`
- `data/sd7037.csv`
- `data/mh32.csv`
- `data/mh84.csv`
- `data/e423.csv`
- `data/clarky.csv`

If you want to add more airfoils, drop new `.csv` files into `data/` and update the script inputs/menus accordingly.

---

## Outputs

Depending on which scripts you run, outputs may include:
- Lift/drag polars and efficiency plots (e.g., CL vs α, CD vs α, CL/CD vs α)
- Preliminary performance estimates and trade-study calculations
- Exported reports/figures saved to `docs/` (optional)

If `docs/` is empty, it simply means exports haven’t been generated yet.

---

## Notes / Known Limitations

- This is intended for **early-stage sizing and comparison**.
- Results depend heavily on the quality/assumptions of the input data (airfoil polars, weight, power limits, etc.).
- If you change units, be consistent across inputs and constants.

---

## How to Cite / Use

This is a personal portfolio project. If you reuse ideas or code, please provide attribution.

---

## Author

**Labeeb Yousuf**  
GitHub: https://github.com/LabeebYousuf
