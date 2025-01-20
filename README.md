# Website

This website is built using [Mintlify](https://mintlify.com/docs/quickstart), a modern website generator.

## How to get a notebook rendered on the website

See [here](https://github.com/ag2ai/ag2/blob/main/notebook/contributing.md#how-to-get-a-notebook-displayed-on-the-website) for instructions on how to get a notebook in the `notebook` directory rendered on the website.

## Build documentation locally

1. To build and test documentation locally, first install [Node.js](https://nodejs.org/en/download/). For example,

```bash
nvm install --lts
```

Then, install the required packages by running the following commands:

```bash
pip install pydoc-markdown pyyaml termcolor nbclient
```

2. You also need to install quarto. Please click on the `Pre-release` tab from [this website](https://quarto.org/docs/download/) to download the latest version of `quarto` and install it. Ensure that the `quarto` version is `1.5.23` or higher.

3. Finally, run the following commands to build and serve the documentation:

```console
./scripts/docs_serve.sh
```

The last command starts a local development server and opens up a browser window.
Most changes are reflected live without having to restart the server.

## Build with devcontainer

To build and test documentation using devcontainer, open the project using [VSCode](https://code.visualstudio.com/), press `Ctrl+Shift+P` and select `Dev Containers: Reopen in Container`.

This will open the project in a devcontainer with all the required dependencies installed.

Open a terminal and run the following command to build and serve the documentation:

```console
./scripts/docs_serve.sh
```

Once done you should be able to access the documentation at `http://localhost:3000/`.
