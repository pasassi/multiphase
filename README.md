# multiphaseML

Repository for applying Machine-Learning techniques to multi-phase flows:

* Flow regime recognition

## Installation in Linux OS

1. Clone the repo in the desired drectory

    ```bash
    git clone git@github.com:pasassi/multiphaseML.git
    ```

1. Create a virtual environment (venv must be installed)

    i. Create a virtual environment (here is named `.venv`)

    ```bash
    python3 -m venv .venv
    ```

    ii. Activate it

    ```bash
    source .venv/bin/activate
    ```

1. Install necessary dependencies via `requirements.txt` (I recommend `pipenv`)

    ```bash
    pipenv install
    ```

    This will read the `requirements.txt` file and generate `Pipfile` and `Pipfile.lock` files

1. Add your virtual environment to Jupyter (the interactive IDE)

    ```bash
    python -m ipykernel install --user --name=.venv
    ```

1. Add your virtual environment as preferred python interpret in VSC

    i. Create a folder called `.vscode` in the repo root dir if you haven't already.

    ```bash
    mkdir .vscode
    ```

    ii. Create the user settings file inside that folder

    ```bash
    touch ./.vscode/settings.json
    ```

    iii. Add this line to your `settings.json` file to set the default Python interpreter for VS Code.

    ```json
    // Sets this project's .venv Python interpreter
    {
      "python.defaultInterpreterPath": "<path_to_multiphaseML>/multiphaseML/.venv/bin/python3",
    }
    ```

    Where `<path_to_multiphaseML>` is the absolute path to `multiphaseML` repository.

## TensorFlow in GPU

Follow the installation guide for using [TensorFlow with GPU](https://www.tensorflow.org/install/gpu)
