# PyTorch with devcontainer

## Prerequisites

- Docker
- Devcontainer CLI
- Visual Studio Code

## Usage

1. Clone this repository

2. Open this repository with Visual Studio Code

3. Run `Remote-Containers: Reopen in Container` command

### Running experiments via SSH/tmux

Use `tmux` to run experiments via SSH.

```bash
# Start a new tmux session
$ tmux 

# Start Devcontainer
$ devcontainer up

# Attach to the running Devcontainer
$ devcontainer exec bash

# Run an experiment
$ python3 my-experiment.py
```
