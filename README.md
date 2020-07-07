# FlowKit tutorials

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Flowminder/FlowKit-tutorials-Ghana/new_content?urlpath=lab/tree/index.ipynb)

This is a Binder repository of tutorials for learning how to use [FlowKit](https://flowkit.xyz/) for CDR analysis. The tutorials are Jupyter notebooks which use the [FlowClient](https://flowkit.xyz/analyst/#flowclient) python client to interact with FlowKit. These tutorials are designed to be used with the Ghana FlowCloud deployment.

## Running the tutorials

### Locally (using conda)

To run the tutorials on your local machine, you will need to do the following (these instructions assume that you have [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) installed):

1. Clone this repository  
2. Create a `conda` environment for the tutorials, using `environment.yml`  
3. Activate the `flowkit-tutorials` environment you just created  
4. Install the jupyter-widgets lab extension (so that FlowKit progress bars will appear in the notebooks)  
5. Start a Jupyter Lab session (or Jupyter Notebook, if you prefer), and open `index.ipynb`  

You can run the following in a `bash` shell to set everything up:

```bash
git clone https://github.com/Flowminder/FlowKit-tutorials-Ghana
cd FlowKit-tutorials-Ghana
conda env create -f environment.yml
conda activate flowkit-tutorials
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter lab index.ipynb
```

### Binder
To run the tutorials online, click the Binder badge at the top of this README. This will start a Jupyter server in the cloud with all dependencies installed, which you can use to run the tutorial notebooks.