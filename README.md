# PyTorch with devcontainer

## Prerequisites

- Docker
- Devcontainer CLI
- Visual Studio Code

## Usage

1. Clone this repository

2. Create conda envs/pkgs directory in local (optional)

```bash
mkdir -p ~/conda_docker/pkgs
mkdir -p ~/conda_docker/envs
```

3. Open this repository with Visual Studio Code

4. Run `Remote-Containers: Reopen in Container` command

### Running experiments via SSH/tmux

Use `tmux` to run experiments via SSH.

```bash
# Start a new tmux session
$ tmux 

# Start Devcontainer
$ devcontainer up --workspace-folder .

# Attach to the running Devcontainer
$ devcontainer exec --container-id <id> bash

# Run an experiment
$ python3 my-experiment.py

# Stop Devcontainer
$ docker rm -f <id>
```
