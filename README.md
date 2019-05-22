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
3. Set-up IPython kernels (docs [here](https://ipython.readthedocs.io/en/latest/install/kernel_install.html#kernels-for-python-2-and-3)). From within a given environment, the name of the kernel can be defined by running:
   ```
   conda activate myenv
   python -m ipykernel install --user --name myenv --display-name "Python (myenv)"
   ```
This ensures that the environment will show up as a kernel in your jupyter notebooks.
