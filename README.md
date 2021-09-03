Instructions to develop jupyterlab extensions

# jupyterlab_apod
Show a random NASA Astronomy Picture of the Day in a JupyterLab panel

1-create-environment

conda create -n jupyterlab-ext --override-channels --strict-channel-priority -c conda-forge -c nodefaults jupyterlab=3 cookiecutter nodejs jupyter-packaging git

2-activate-environment


 To activate this environment, use

     $ conda activate jupyterlab-ext

 To deactivate an active environment, use

     $ conda deactivate

3-initialize-from-cookiecutter

cookiecutter https://github.com/jupyterlab/extension-cookiecutter-ts

4-activate-and-start

conda activate jupyterlab-ext
jupyter lab

5-link-development-sources

jupyter labextension develop --overwrite .

6-build

jlpm run build

or

jlpm run watch


