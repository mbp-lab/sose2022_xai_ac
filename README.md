# Explainable AI for Affective Computing

SoSe2022 Bielefeld University

In this seminar we will learn about the latest research in eXplainable AI (XAI) and its application for the field of affective computing.  This reposity will contain a series of [Jupyter Notebooks](https://jupyter.org/) to give you practical experience using various Python toolkits.

## Installation Instructions

### Install Anaconda

We will use Anaconda for the management of virtual environments and python package installations.

Download and install [miniconda](https://docs.conda.io/en/latest/miniconda.html), a lightweight installation of anaconda (if you already have the full version of anaconda installed, that will work as well).

### Create Virtual Environment and Install Necessary Python Packages

After installing miniconda, you now have the ability to easily create and manage Python virtual environments using the `conda` command. For the Jupyter Notebooks used in this seminar, we recommend you create a new virtual environment to manage the various Python packages we will use through out the semester.  

If you're not already familiar with `conda`, you may want to familiarize your self with the [documentation](https://docs.conda.io/projects/conda/en/latest/commands.html) and the various commands in [this cheat sheet](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)

To create a new virutal env for this seminar, run the following commands from your conda terminal.

1. Create a new virtual env named 'ml_bias_seminar' with the latest version of Python3:
 	- `conda create -n xai_ac python=3`
2. Activate the new virtual env:
	- `conda activate xai_ac`
3. Install the required Python packages
	- `conda install -c conda-forge jupyterlab scikit-learn matplotlib pandas seaborn`


## Getting Started with the Notebooks

### Clone the Seminar GitHub Repo

All notebooks during the semester will be provided through this GitHub repository.  The easiest way to obtain the notebooks is to `clone` this repository, and then perfrom a `git pull` when we announce that new notebooks are available. Here I will provide terminal instructions to clone and pull the repo, but you are free to use your preferred GUI or Git interface.

1. To `clone` the repository:
	- First make sure you have in a directory where you would like to store the repository
	- `git clone \<LINK TO REPO\>`
	- This will download all the current notebooks and material into a folder named \<REPO NAME\>

2. If we announce a new notebook or repository changes, then `pull` from the repo to get the latest material
	- make sure you are in the cloned directory named \<REPO NAME\>
	- run: `git pull`
	- You should recieve a message indicating new files were downloaded

### Running a JupyterLab and Launching a Notebook

For this seminar, we will use [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) to run and manage our Notebooks.

1. Start JupyterLab
	- make sure you virtual env is activated
	- run: `jupyter-lab`
	- This should automatically open JupyterLab in your browswer window
	- if not, open the URL provided in your terminal output
2. To create a new Notebook
	- Go to the "Launcher" tab and click the Python icon in the "Notebook" section
3. To open an existing notebook
	- In the file explorer pane on the left, browse to an `.ipynb` file and doubleclick it

### Validate Your Virtual Environmenmt Installation

To validate your virtual env installation, and make sure you are able to run a simple notebook

1. In JupyterLab, open `validate_installation.ipynb`
2. Follow the instructions in the Notebook


### (Optional) Intro to ML Notebook

As an example, you can also familiarize yourself with the Notebook we will use in our first lecture: `intro_ml.ipynb`

## Notebook 1 Instructions - Simplification and Feature Attribution

*This section assumes you've already gone through all above steps.*

1. Pull the most recent updates from the reposititory by running `git pull` from your local repository. 
2. Activate your conda env, `conda activate xai_ac`.
3. Install the following Python Packages:
    1. [Tensorflow](https://www.tensorflow.org/install): `pip install tensorflow` (there is no training so a GPU is not needed)  
    2. [LIME](https://github.com/marcotcr/lime): `pip install lime`
    3. [SHAP](https://shap.readthedocs.io/en/latest/index.html#): `conda install -c conda-forge shap`
4. Run Jupyter Lab: `jupyter lab`
5. Open `Notebooks/1. simplification_attribution.ipynb` 
6. Complete the tasks as described in the Notebook.