## Quick steps to develop jupyterlab extensions

 this jupyterlab_apod extension shows a random NASA Astronomy Picture of the Day in a JupyterLab panel

## 1 Create conda environment

    conda create -n jupyterlab-ext --override-channels --strict-channel-priority -c conda-forge -c nodefaults jupyterlab=3 cookiecutter nodejs jupyter-packaging git

## 2 Activate conda environment


 To activate this environment, use

     $ conda activate jupyterlab-ext

 To deactivate an active environment, use

     $ conda deactivate

## 3 Initialize project from cookiecutter

     cookiecutter https://github.com/jupyterlab/extension-cookiecutter-ts

## 4 Acivate environment and start jupyterlab

    conda activate jupyterlab-ext
    jupyter lab

## 5 Link development sources to jupyterlab

    jupyter labextension develop --overwrite .

## 6 Build

    jlpm run build

  or

    jlpm run watch


# 7 Enjoy!!!

  Go to View -> Ativate Command Palette -> Random Astronomy Picture
  Take a beer ... or a coffee!!
