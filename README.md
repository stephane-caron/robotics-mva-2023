# Robotics MVA 2023

This repository contains tutorial notebooks for the 2023 [Robotics](https://www.master-mva.com/cours/robotics/) class at MVA.

## Getting started

### Clone this repository

Using Git via SSH:

```bash
git clone git@github.com:stephane-caron/robotics-mva-2023.git
```

Or via HTTPS:

```bash
git clone https://github.com/stephane-caron/robotics-mva-2023.git
```

### Install miniconda

- Linux: https://docs.conda.io/en/latest/miniconda.html
- macOS: https://docs.conda.io/en/latest/miniconda.html
- Windows: https://www.anaconda.com/download/

Only a little snippet is applied to your home .bashrc, everything else will be segmented!

### Run a notebook

- Go to your local copy of the repository.
- Open a terminal.
- Create the conda environment:

```bash
conda env create -f robotics-mva.yml
```

From there on, to work on a tutorial notebook, you only need to activate the environment:

```bash
conda activate robotics-mva
```

Then launch the notebook with:

```bash
jupyter-lab
```

The notebook will be accessible from your web browser at [localhost:8888](http://localhost:8888).

Meshcat visualisation can be access in full page in `localhost:700N/static/` where N denotes the Nth meshcat instance created with the running kernel.

## Troubleshooting

- Make sure you call ``jupyter-lab`` so that Python packages pathes are configured properly (for instance ``jupyter-notebook`` might not have paths configured properly; if that's the case, it will fail to import packages properly).
- Make sure the virtual environment is activated for ``jupyter-lab`` to work.

## Updating the notebooks

If the repository changes (for instance when new tutorials are pushed) you will need to update your local copy of it by "pulling" from the repository. To do so, go to the directory containing the tutorials and run:

```
git pull
```

If you already have local changes to a notebook `something.ipynb`, either you already know how to use git and you can commit them, or you don't and the safest way for you to update is to:

- Copy your modified `something.ipynb` somewhere else
- Revert it to its original version: ``git checkout -f something.ipynb``
- Pull updates from the remote repository: ``git pull``
