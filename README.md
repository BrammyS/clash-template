# Clash template
This project uses the official [Haskell devcontainer](https://github.com/microsoft/vscode-dev-containers/tree/main/containers/haskell) and the [clash starter project](https://github.com/clash-lang/clash-starters/tree/main/simple) as a base.

## Using the template

See
the [Create reposotiry from a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)
guide for a more detailed explanation.

1. Navigate to the main page of the repository.
2. Above the file list, click `Use this template`.
   ![Use template button](https://cdn.brammys.com/2022/02/use-this-template-button.png)
3. Enter the name for your new repository and choose a visibility option.
4. Click the `Create repositoiry from template` button.

## Running the devcontainer
Please follow the [official tutorial](https://code.visualstudio.com/docs/devcontainers/tutorial) on how to get a devcontainer up and running.

## Building and testing this project
The recommened way of building this project is by using the stack command, which is installed by defaulted in the devcontainer.

Build the project with:

```bash
stack build
```

To run the tests defined in `tests/`, use:

```bash
stack test
```

To compile the project to VHDL, run:

```bash
stack run clash -- Example.Project --vhdl
```

You can find the HDL files in `vhdl/`. The source can be found in `src/Example/Project.hs`.

## Project overview
More information about the structure of this template can be found [here](https://github.com/clash-lang/clash-starters/tree/main/simple#project-overview).