This is a docker image which can simulate running docker as a local standalone instance.

## How to Run
For simplicity running this as a remote container in VS Code will best simulate running locally.
Use the Remote - Containers (ms-vscode-remote.remote-containers) extension and execute `Rebuild and open in container` from the command pallete.  This builds the container and opens a VS code server within the container.

## Adding more extensions at build time
To add more extensions at build time in the remote VS Code instace just add to the array in `.devcontainer/devcontainer.json` config file.  See [here](https://code.visualstudio.com/docs/remote/containers) for official Microsoft docs.

## Pip install while container is running
Due to a currently unresolved build issue, when pip installing the version of python needs to be targeted e.g. `python -m pip install numpy`