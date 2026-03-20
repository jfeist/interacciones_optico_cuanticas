# Hands-on Notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jfeist/interacciones_optico_cuanticas/HEAD)

This repository is configured to run in three ways from a single dependency source:

1. Binder
2. GitHub Codespaces + VS Code notebooks
3. Local machine with `uv`

All Python packages are defined in `pyproject.toml`.

## 1) Binder

Binder uses:

- `pyproject.toml` for Python package installation (`pip install -e .` via repo2docker)
- `runtime.txt` for Python version

You can launch with the Binder badge above.

## 2) GitHub Codespaces

The repository includes `.devcontainer/devcontainer.json`.
When a Codespace starts, it will:

1. Install `uv`
2. Create/update `.venv`
3. Sync dependencies from `pyproject.toml`

Then open any notebook in VS Code and select the `.venv` kernel if prompted.

## 3) Local machine with uv

From the repository root:

```bash
uv run jupyter lab
```

This will automatically create/manage the environment and install project dependencies.

If you want to pre-sync once (optional):

```bash
uv sync
```

Then run again:

```bash
uv run jupyter lab
```
