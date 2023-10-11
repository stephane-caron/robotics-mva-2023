# Robotic MVA 2023

This repository contains tutorial notebooks for the 2023 [Robotics](https://scaron.info/robotics-mva/) class at [MVA](https://www.master-mva.com/cours/robotics/).

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
conda env create -f robotics_course_env.yml
```

From there on, to work on a tutorial notebook, you only need to activate the environment:

```bash
conda activate robotics_course
```

Then launch the notebook with:

```bash
jupyter-lab
```

The notebook will be accessible from your web browser at [localhost:8888](http://localhost:8888).

Meshcat visualisation can be access in full page in `localhost:700N/static/` where N denotes the Nth meshcat instance created with the running kernel.

## Updating the notebooks

If the repository changes (for instance when new tutorials are pushed) you will need to update your local copy of it by "pulling" from the repository. To do so, go to the directory containing the tutorials and run:

```
git pull
```
