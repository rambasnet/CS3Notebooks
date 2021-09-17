
# Introduction to Algorithms using C++

- Jupyter notebooks for text **CS3 Data Structures and Algorithms:** https://opendsa-server.cs.vt.edu/ODSA/Books/CS3/html/

## View the notebooks online at [nbviewer.jupyter.org](https://nbviewer.jupyter.org/github/rambasnet/CS3Notebooks/tree/master/)

- github itself renders notebooks most of the time but not reliable and some contents may not render correctly
- click the above link or go to nbviewer.jupyter.org and copy pase this github repo URL
- NOTE: You can only read text and code but not execute it online
- see instructions below to run these notebooks (C++ code) on your system

## Run C++ Code in Notebooks
### Requirements
- Jupyter Notebook
- xeus-cling Notebook Kernel (C++ interpreter)

## Install Required Tools
### Linux/Mac
- Download and install Miniconda: https://conda.io/miniconda.html 
- download Miniconda3...sh shell script installer file
- open a terminal cd into the directory where the file was downloaded
- run the shell script installer file
    ``` 
    $ bash Miniconda3.....sh
    ```
- go through installation process; default works great on every prompt
- once conda is installed; use conda to install the following pacakages
- you have to close and start a new terminal to run freshly installed conda
    ```
    $ conda create -n cpp #create virtual environment for C++ 
    $ conda activate cpp
    $ conda install notebook
    $ conda install -c conda-forge xeus-cling
    $ conda install -c conda-forge jupyter_contrib_nbextensions
    $ conda install -c conda-forge jupyter_nbextensions_configurator
    $ jupyter nbextensions_configurator enable --user
    ```
    
### Windows
- On Windows, follow the instruction here: https://github.com/QuantStack/xeus-cling
to install xeus-cling
- NOTE: C++ interpreter kernel is experimental on Windows
- Recommended: 
    - enable and use WSL (Ubuntu) on Windows 10
    - follow Linux/Mac instructions above 


## Run Notebooks
- open a terminal and cd into this cloned/downloaded repository folder and run jupyter notebook
    ```
    $ cd <cs3notebooks folder>
    $ conda activate cpp
    $ jupyter notebook
    ```
- start from 00-TableOfContents.ipynb chapter or open any chapter

## Stop Jupyter Notebook server

- enter `ctrl+c` simultaneously on the Terminal where the jupyter notebook server is running on

```bash
$ conda deactivate # to deactivate cpp env and go to base env
```

