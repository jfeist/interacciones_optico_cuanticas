# Hands-on Notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jfeist/interacciones_optico_cuanticas/HEAD)

These notebooks can be run in three different ways. Choose whichever suits you best.

## Option 1 — Binder (easiest, no account needed)

Click the **Launch Binder** badge above. A computing environment will be built in the cloud and JupyterLab will open in your browser. Nothing needs to be installed on your computer.

**Pros:** No account, no setup, works from any browser.  
**Cons:** Takes a minute or two to start. The session shuts down automatically after about 10 minutes of inactivity, and any changes you make (edited notebooks, saved results) are lost when it does — the environment is completely temporary.

## Option 2 — GitHub Codespaces (persistent, GitHub account required)

Go to the repository page on GitHub and click **Code → Codespaces → Create codespace on main**. VS Code will open in your browser with everything already installed.

**Pros:** Your work is saved between sessions. Feels like a proper editor (VS Code). Reasonably fast to start once the environment has been built.  
**Cons:** Requires a free GitHub account. GitHub's free tier includes 60 hours/month of Codespace usage, which should be plenty for this course.

## Option 3 — Your own computer (most control, some setup required)

If you want to run the notebooks on your own machine, you need to install [uv](https://docs.astral.sh/uv/getting-started/installation/), a Python package manager. Then, from a terminal in the folder where you downloaded this repository, run:

```
uv run jupyter lab
```

This will download all required packages automatically on the first run and then open JupyterLab in your browser.

If you prefer opening the notebooks in VS Code, run:

```
uv sync
```

Then select the environment created by `uv` as your notebook kernel in VS Code.

**Pros:** Works offline. Full control over your environment. Changes are saved locally.  
**Cons:** Requires installing software and using a terminal. Initial package download can take a few minutes.
