# conda-envs
Anaconda environments and set-up

1. [Install Miniconda](https://docs.conda.io/en/latest/miniconda.html). This is recommended as it uses much less space than the full Anaconda distribution, while still providing the package manager, conda. When installing, I like to select "Add Anaconda to path...", even though it is not recommended. I find the Anaconda prompt to be slow and I would rather just boot things through the terminal.

2. To create an environment from scratch, run:
    ```
    conda create --name myenvname
    ```
    Otherwise, build from an environment.yml file as (note that the name of the env is defined in the first line of environment.yml):
    ```
    conda env create -f environment.yml
    ```
