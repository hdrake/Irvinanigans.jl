# Irvinanigans.jl

A (probably incomplete) set of instructions for running the Julia notebooks in this repository:

## Forking this repository

- At the top of this repository's main page, press the "Fork" button at the top right to create your own fork of this repository, which should create a new browser tab with at the URL `https://github.com/YOUR-GITHUB-USERNAME/Irvinanigans.jl` (with `YOUR-GITHUB-USERNAME` being your actual username).

## Installation and launching Julia
- Install [Julia v1.10.2](https://julialang.org/downloads/#current_stable_release) (may be under "Older Releases") and run the newly installed Julia program.

- This should launch a Julia "REPL" with the following command line prompt:
```julia
julia>
```

## Cloning Irvinanigans.jl from Github's cloud (remote server) to your laptop/workstation (local server).

- Type `;` in the Julia REPL to switch it to "shell" mode, which functions like a UNIX terminal. Use the change directory command (`cd`) in a UNIX terminal to go into whatever root directory you would like to download this repository into. Use the `pwd` command to check that you are indeed in the correct location.


- Clone your fork of the repository into your current working directly by running the following command in Julia's "shell" mode (with `YOUR-GITHUB-USERNAME` being your actual username):
```bash
git clone https://github.com/YOUR-GITHUB-USERNAME/Irvinanigans.jl.git
```

- Still in the "shell" mode, change into this newly cloned working directory with `cd Irvinanigans.jl`

- Press the `Delete` key to get back to Julia's "REPL" mode and then the `]` key to transition from Julia's "REPL" mode to the "package manager" mode. Activate and build this repository's environment (a coordinated set of Julia software packages) with:
```
activate .
```
and then
```
build
```

- Press the 'Delete' or 'Backspace' key to exit the package manager mode and return to the REPL mode.

- Import the IJulia package and launch an instance of the browser-based JupyterLab programming environment with:
```julia
using IJulia
jupyterlab(dir=pwd())
```
