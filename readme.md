# Py Torch Play

A bit of a play with data science using [PyTorch](https://pytorch.org/get-started/locally/).

## Random notes on setting up a Python Virtual Envioronment

You can set up the environment you need using Python, Virtual Environments and pip. But to be honest, its all easier using [Anaconda](https://www.anaconda.com/).

`python -m pip install --upgrade pip`

`python -m pip install virtualenv`

`virtualenv venv`

`python -m virtualenv venv`

`pip install torch torchvision torchaudio`

## Anaconda

Anaconda seems to support the whole thing, its like a sandbox where the packages can be installed, andyou can also configure a completely independently version of Python. Kool.

Once Anaconda was installed, the following random commands were helpful.

`conda create --name bio-env`

`conda create --name bio-env python=3.9.13 --debug`

`conda env remove --name bio-env --debug`

`activate bio-env`

`pip install jupyter`

`conda install pytorch torchvision torchaudio cpuonly -c pytorch`

The following `pwsh` is also good to perhaps put into a script: 

``` pwsh
C:\ProgramData\Anaconda3\shell\condabin\conda-hook.ps1; `
conda activate "C:\ProgramData\Anaconda3";
```

Then set an alias in the profile:

`Set-Alias -Name condap -Value "C:/playground/conda/conda_profile.ps1"`

Then just call it on `pwsh` line using the command:

`condap`

Now you can fire up a terminal and manage the environment using the command line or VS Code.

## References

<https://learn.microsoft.com/en-us/training/modules/intro-machine-learning-pytorch/?WT.mc_id=aiml-7486-cxa>

<https://pytorch.org/get-started/locally/>

<https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf>
