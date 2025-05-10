# Sudoku PCGRL

This repository contains code for Procedural Content Generation via Reinforcement Learning (PCGRL) applied to Sudoku board generation.

**Clone the Repo**
```
git clone https://github.com/saniyaismail/sudoku_board_gen.git
cd sudoku_board_gen/
```



## Installation

1. **Install System Dependencies**
   
    ```bash
    sudo apt update
    sudo apt install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev git
    ```


2.  **Install `pyenv` and Python 3.7:**


    ```bash
    curl [https://pyenv.run](https://pyenv.run) | bash
    ```

3.  **Configure your shell for `pyenv`:**

    Add the following lines to your `~/.bashrc` or `~/.zshrc` file:

    ```bash
    export PATH="$HOME/.pyenv/bin:$PATH"
    eval "$(pyenv init --path)"
    eval "$(pyenv init -)"
    eval "$(pyenv virtualenv-init -)"
    ```

4.  **Reload your shell:**

    ```bash
    exec "$SHELL"
    ```

5.  **Install and set up the required Python version and virtual environment:**

    ```bash
    pyenv install 3.7.17
    pyenv virtualenv 3.7.17 pcgrl-env
    pyenv local pcgrl-env # Activate the virtual environment for this directory
    ```

6.  **Install Python Dependencies:**

    Ensure `pip` and `setuptools` are at the required versions before installing the project dependencies.

    ```bash
    pip install pip==20.2.4 setuptools==49.6.0
    pip install -r requirements.txt
    ```
## Running Inference

To generate a Sudoku board using the trained model, run the `inference.py` script:

```bash
python inference.py
```
Image can be found saved as final_board.png
gif showing the procedural generation of the sudoku board can be found saved as board_generation.gif
