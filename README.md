# Test Driven Development with C++

This repo contains documents served by `mkdocs`. For more information, see [Getting Started](https://www.mkdocs.org/getting-started/)

We use `venv` to create a Python virtual environment from which we can serve our documentation using `mkdocs`. Specifically, we create on named `.venv` using:

```shell
python3 -m venv .venv
```

To activate this virtual python environment, simply type

```shell
source .venv/bin/activate
```

To deactivate the virtual environment, simply type

```shell
deactivate
```

## Prerequisites

Given the configuration we have in this repository, you'll need to install some modules to serve them up using `mkdocs`

```shell
pip install mkdocs
pip install pymdown-extensions
pip install mkdocs-material
```

## Serving locally

```shell
mkdocs build
mkdocs serve
```

For more information on pip, see [Install packages in a virtual environment using pip and venv](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/).
