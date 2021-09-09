# 🥱 Setup without Docker

* We need to install:
    * [Python 3.9](https://www.python.org/downloads/release/python-397/)
    * [Conda](https://docs.conda.io/projects/conda/en/latest/)
    * Pip using  `python -m pip install -U pip`

## 🐍 Basic Setup Anaconda

```bash
conda create --name test-tdd-docs
```

```bash
Proceed ([y]/n)? y
```

```bash
conda activate test-tdd-docs
```

Dependencies

```bash
conda install -c conda-forge jupyterlab
conda install -c conda-forge numpy
conda install -c conda-forge pandas
```

If we want to deactivate environment we need to use:

```bash
conda deactivate
```

## 🤔 Anaconda basic usage

Check to see if a package you have not installed named "pandas" is available from the Anaconda repository (must be
connected to the Internet):

```bash
conda search pandas
```

Conda displays a list of all packages with that name on the Anaconda repository, so we know it is available.

Install this package into the current environment:

```bash
conda install pandas
```

Check to see if the newly installed program is in this environment:

```bash
conda list
```



# 🐳 Setup with Docker for mkdocs

Windows 
```bash
docker run --rm -it -p 8000:8000 -v "%cd%":/docs squidfunk/mkdocs-material
```

Linux
```bash
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```

# 🧪 Setup without Docker for mkdocs

We need to install pip
```bash
pip install mkdocs-material
```
## 📄 Commands


* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## References
* [mkdocs](https://www.mkdocs.org)
* [mkdocs material](https://squidfunk.github.io/mkdocs-material/)