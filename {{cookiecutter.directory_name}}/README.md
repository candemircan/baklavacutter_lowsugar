# {{cookiecutter.directory_name}}

> Project description goes here.

## Setup

For setup, you need to do the following things:


1. Clone the repository
    ```bash
    git clone https://github.com/{{cookiecutter.user_name}}/{{cookiecutter.directory_name}}.git
    ```

2. Install the local packages
    ```bash
    cd {{cookiecutter.directory_name}}
    pip install .
    ```

3. Define environment variables.
    You need to define `{{cookiecutter.directory_name | upper}}_DIR` as an environment variable, so that the code can find the relevant data and files. You can do this by running the following lines in your terminal:

    ```bash
    export {{cookiecutter.directory_name | upper}}_DIR=/PATH/TO/{{cookiecutter.directory_name | upper}}
    ```

    or put the same lines in a file that is run during your session startup (e.g. `~/.bashrc`)

    Note: I am using Python {{cookiecutter.python_version}}, not sure about the compatability with other versions.

## Folder Structure

```bash
├── bin # all the *.py, *.sh, *.slurm scripts
├── data # all the raw data generated by the tasks
├── figures # all the figures generated by docs/Visualisation*.ipynb
├── {{cookiecutter.directory_name}} # the local package, contains all the custom functions
├── logs # all the logs generated by the scripts, nothing is committed
└── results # all the results generated by analyses, modelling, simulations etc.
```