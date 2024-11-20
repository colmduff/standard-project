# Python Project Template with Copier

This repository contains a customizable Python project template powered by [Copier](https://copier.readthedocs.io/). It allows you to quickly scaffold Python projects with a standardized structure, preconfigured tools, and dynamic settings.

## Features

- **Dynamic Configuration**: Define project-specific details like the project name, author, and directory paths at generation time.
- **Poetry Integration**: Includes a `pyproject.toml` file preconfigured for managing dependencies and development tools.
- **Flexible Directory Structure**: Easily customize the structure to fit your needs using Copier variables.
- **Preconfigured Tools**:
  - [pytest](https://docs.pytest.org/): For testing.
  - [black](https://black.readthedocs.io/): For code formatting.
  - [isort](https://pycqa.github.io/isort/): For import sorting.

## Project Structure

The generated project includes:

```plaintext
{{ project_name }}/
├── pyproject.toml      # Project metadata and dependencies
├── README.md           # Project readme
├── data/               # Data directory
├── source/             # Source code directory
└── tests/              # Tests directory
```

Usage
1. Install Copier:

```bash
pip install copier
```

2. Clone this template:
```bash
git clone <repository-url>
cd <repository-folder>
```

3. Generate a new project:
```bash
copier copy ./ path/to/new_project
```

4. Answer the prompts:
```plaintext
Your project name [my_project]: awesome_project
Author name [Your Name]: Jane Doe
Author email [your.email@example.com]: jane.doe@example.com
```

5. Navigate to the new project and install dependencies:
```bash
cd path/to/new_project
poetry install
```


### Getting Started with This Template
To customize this template or contribute, fork this repository and modify the files as needed. Key files to look at:

`copier.yaml`: Defines the prompts and variables.
`pyproject.toml.jinja`: Template for project configuration.
`README.md.jinja`: Template for the project readme.
