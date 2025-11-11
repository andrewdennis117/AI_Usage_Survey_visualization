# AI Usage Visualization Project

The goal of this project is to explore and visualize responses from an internal AI usage survey. The work is organized around a data exploration notebook that produces charts highlighting how different teams and developer types rely on AI tools in their day-to-day workflows.

## Repository Structure
- `responses.csv` – raw survey export provided by the user
- `data/` – reserved for cleaned datasets or derived exports (none checked in yet)
- `notebooks/01_eda.ipynb` – exploratory notebook with data preparation and visualizations
- `scripts/` – placeholder for future automation or batch jobs
- `reports/` – placeholder for presentation-ready assets

## Environment Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

To add new dependencies, install them with `pip` and update `requirements.txt` using `pip freeze > requirements.txt`.

## Working with the Notebook
1. Launch the environment:
   ```bash
   source .venv/bin/activate
   jupyter lab
   ```
2. Open `notebooks/01_eda.ipynb`.
3. Run the cells sequentially to:
   - Load and clean the survey data
   - Produce team-level views (workflow usage, tech stack, AI tools)
   - Explore cross-team comparisons (heatmaps, stacked bars)
   - Summarize AI helpfulness perceptions

The notebook intentionally keeps raw identifiers (e.g. `Email`, `Name`). Remove or anonymize them before sharing externally.

## Next Steps
- Export cleaned datasets into `data/`
- Polish presentation-ready charts and move finals into `reports/`
- Consider interactive dashboards (Plotly, Voila) for stakeholders

## Notes
- The repository assumes Python 3.9+.
- For reproducibility, commit only derived artifacts that are required for reports.
- Review the notebook comments for details on each visualization and any data caveats.
