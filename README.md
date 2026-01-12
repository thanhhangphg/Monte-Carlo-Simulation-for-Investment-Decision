# Keissi — Vektorisoitu (Python / NumPy)

A simulation-based decision analysis project comparing industrial oven investment alternatives over a **5-year horizon**. The model estimates **NPV distributions** under uncertainty in **energy prices**, **capacity-driven storage**, and **failure/repair events**.

## Skills demonstrated
- Vectorized programming with **NumPy arrays** (avoiding slow Python loops)
- Numerical analysis / scientific computing with **SciPy**
- Clear visualization of results using **Matplotlib**
- Reproducible workflow with a minimal dependency set

## Data
Input CSVs are included under `data/`.

## Setup
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
```

## Run
```bash
jupyter lab
```
Open:
- `monte_carlo_simulation_project.ipynb`.

## Outputs
- A full written summary is included in `monte_carlo_simulation_report`.
- Uncertain inputs are modeled with probability distributions (e.g., energy prices, demand/batch sizes, failures).
- Each alternative is simulated many times to produce an NPV distribution.
- Decision-making can consider risk metrics such as **mean NPV, percentiles (P5/P50/P95), probability of loss**, and robustness under stress scenarios.
