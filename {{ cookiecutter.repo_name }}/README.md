{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
------------

    │
    ├── data/               <- The original, immutable data dump. 
    │
    ├── figures/            <- Figures saved by scripts or notebooks.
    │
    ├── notebooks/          <- Jupyter notebooks. Naming convention is a short `-` delimited 
    │                         description, a number (for ordering), and the creator's initials,
    │                        e.g. `initial-data-exploration-01-hg`.
    │
    ├── output/             <- Manipulated data, logs, etc.
    │
    ├── paper/              <- Draft of paper using pandoc flavored markdown. Edit the `bib`
    │                        and  `.md` files in this directory then `make paper` to compile.
    │                        The required fonts are available in the `.pandoc` directory
    │
    ├── tests/              <- Unit tests.
    │
    ├── {{ cookiecutter.python_module_name }}/      <- Python module with source code of this project.
    │
    ├── environment.yml     <- conda virtual environment definition file.
    │
    ├── LICENSE
    │
    ├── Makefile            <- Makefile with commands like `make environment`
    │
    ├── README.md           <- The top-level README for developers using this project.
    │
    └── tox.ini             <- tox file with settings for running tox; see tox.testrun.org


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>.</p>


Set up
------------

Install the virtual environment with conda and activate it:

```bash
$ conda env create -f environment.yml
$ conda activate example-project 
```

Install `{{ cookiecutter.python_module_name }}` in the virtual environment:

```bash
$ python setup.py develop
```

Write in the paper directory. Use `make paper` to compile the draft to pdf, html and latex. 
If your article requires formatting for a particular journal, you can recompile the output latex along with the appropriate template
