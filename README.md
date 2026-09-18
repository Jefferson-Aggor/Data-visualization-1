Data Visualization

A Python-based learning project focused on data analysis and visualization using Pandas, NumPy, Matplotlib, Seaborn, and Plotly.

The project is organized into lessons, with datasets stored separately for practice and analysis.

🛠️ Technologies

Python 3.11

uv

NumPy

Pandas

Matplotlib

Seaborn

Plotly

JupyterLab

📁 Project Structure
Data-visualization/
│
├── data/
│   └── # Datasets used throughout the lessons
│
├── lesson/
│   └── lesson-1/
│       └── # Lesson 1 materials
│
├── lesson-1/
│   └── # Current lesson work
│
├── .venv/
│   └── # Python virtual environment
│
├── pyproject.toml
├── uv.lock
└── README.md

🚀 Setup

This project uses uv for Python and dependency management.

1. Install uv

If uv is not already installed:

pip install uv


Or install it using the official installer:

curl -LsSf https://astral.sh/uv/install.sh | sh


After installation, make sure uv is available:

uv --version


If the installer tells you to run source $HOME/.local/bin/env but that file doesn't exist, you can simply use the uv installed by pip if uv --version works.

2. Install Python

The project uses Python 3.11:

uv python install 3.11

3. Create the project

Initialize the project with Python 3.11:

uv init --python 3.11

4. Install dependencies
uv add matplotlib seaborn pandas numpy plotly jupyterlab


This creates the .venv virtual environment and installs the required packages.

🔌 Activate the Virtual Environment

From the project root:

source .venv/bin/activate


You should then see something similar to:

(data-visualization) @jotokx88 ➜ /workspaces/Data-visualization $


You can also run commands through uv without manually activating the environment:

uv run python

📊 Libraries
NumPy

Used for numerical computing and working with arrays.

import numpy as np

Pandas

Used for loading, cleaning, transforming, and analyzing datasets.

import pandas as pd

Matplotlib

Used to create static charts and visualizations.

import matplotlib.pyplot as plt

Seaborn

Built on Matplotlib and useful for creating statistical visualizations.

import seaborn as sns

Plotly

Used for interactive charts and dashboards.

import plotly.express as px

JupyterLab

Used for interactive Python notebooks and experimentation.

Start JupyterLab with:

uv run jupyter lab

📚 Lessons
Lesson 1

The first lesson focuses on setting up the Python environment and getting started with data visualization.

Topics will include:

Python environment setup

NumPy basics

Pandas basics

Loading datasets

Data cleaning

Basic Matplotlib charts

Seaborn visualizations

Interactive Plotly charts

Additional lessons will be added as the project develops.

📂 Working With Data

Place datasets inside the data/ directory:

data/
├── dataset.csv
├── another-dataset.csv
└── ...


Example:

import pandas as pd

df = pd.read_csv("data/dataset.csv")

print(df.head())

🔄 Updating Dependencies

To add a new package:

uv add package-name


For example:

uv add scikit-learn


To synchronize the environment with the project dependencies:

uv sync

🎯 Goal

The goal of this repository is to build practical data visualization skills through hands-on lessons and real datasets.

The project will gradually cover:

Data collection

Data cleaning

Exploratory data analysis

Statistical analysis

Data visualization

Interactive visualization

Data storytelling

Building complete data