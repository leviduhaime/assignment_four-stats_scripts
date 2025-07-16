# Assignment 4 – Python Statistics Walkthrough

This repository contains a Jupyter notebook explaining the use of various statistical analyses and data visualization tools for Python. The notebook is based on exercises from a SciPy-Lectures.org tutorial. This repository also contains environment.yml and requirements.txt files for easily recreating the Python environment used to create and run the notebook with Conda and/or Pip, respectively.

The goal of this assignment is to practice applying common statistical and plotting techniques in Python that will be useful in future data analysis labs.

## Source

The SciPy-Lectures tutorial can be found at:
https://scipy-lectures.org/packages/statistics/index.html

Author: Gaël Varoquaux

## Contents

```
assignment_four-stats_scripts/
├── notebooks/
│ └── stats_python.ipynb # Notebook with tutorial walkthrough
├── .gitignore # Tells Git which files and folders to ignore 
├── README.md # This file
├── environment.yml # Conda environment definition
└── requirements.txt # Pip-based environment definition

```

## Getting Started

### Clone the Repository and Set Working Directory

```
git clone https://github.com/leviduhaime/assignment_four-stats_scripts.git
cd assignment_four-stats_scripts
```

### Create the Python Environment

```
module load miniconda3/24.1.2-py310
conda env create -f environment.yml
conda activate stats-env
```

*Or use pip:*

```
pip install -r requirements.txt
```

### Launch Jupyter Lab

```
jupyter lab
```

### Interact With the Notebook

Navigate to `../notebooks/stats_python.ipynb` and open the notebook.

Run each code block, from top to bottom and read the markdown cells for explanations of the code statistical analyses and plotting functions. If you want to recreate any of the plots or tests from the tutorial, you will need to access the source data files from the tutorial website:

https://scipy-lectures.org/packages/statistics/index.html

Those files are:

```
brain_size.csv
iris.csv
wages.txt
```

The notebook assumes that those files are located in the git repo clone directory

```
../assignment_four-stats_scripts/
```

If you want to change the location of the source data files, simply replace each instance of...

```
data = pd.read_csv('../brain_size.csv',
```

...in code blocks with another file location of your preference.

## License

This repository is intended for educational use only.

## Acknowledgments

Based on exercises from:
https://scipy-lectures.org/packages/statistics/index.html
Author: Gaël Varoquaux
© The SciPy Lecture Notes author(s).