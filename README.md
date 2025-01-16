# rob599learning

Repo for UMich ROB599: Robot Learning for Planning and Control Winter 2025

## Installation

- Install ROCm: `paru -S rocm-opencl-runtime`
- Install PyTorch: `paru -S python-pytorch-rocm`
- Install other dependencies: `pipenv install --dev`
- Set pyenv to use system-wide dependencies (for pytorch):

```bash
cd <location of the virtualenv>
vim pyvenv.cfg
# change include-system-site-packages to true
```

- Test Installation

```bash
pipenv shell
python
import torch
torch.cuda.is_available()
```

- The result should look like this

```bash
$ pipenv shell
Launching subshell in virtual environment...
[akshatd@akshatd-tp rob599learning_repo]$  source /home/akshatd/.local/share/virtualenvs/rob599learning_repo-UbsyU0pF/bin/activate
$ python
Python 3.13.1 (main, Dec  4 2024, 18:05:56) [GCC 14.2.1 20240910] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import torch
>>> torch.cuda.is_available()
True
```
