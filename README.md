# learning-machines
everything that i forgot from cs370 and cs371

## Setup

```bash
uv sync                  # install deps into .venv
uv run jupyter lab       # launch JupyterLab
```

Or `source .venv/bin/activate` to use the venv directly.

## Layout

- `notebooks/` — Jupyter notebooks (start with `00_sanity_check.ipynb`)
- `src/` — reusable modules
- `data/` — datasets (gitignored)
- `models/` — saved weights (gitignored)

PyTorch is pinned to CPU. For CUDA, swap the index in `pyproject.toml` (`pytorch-cpu` → `pytorch-cu124` with `https://download.pytorch.org/whl/cu124`).
