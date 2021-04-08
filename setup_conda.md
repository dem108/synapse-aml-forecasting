# setup_conda

## how to

If it's the first time setting up conda in your bash environment,

```bash
conda init bash
```

Then,

```bash
conda create -n synapse-aml python=3.8.*
conda activate synapse-aml
pip install -r requirements.txt
```

If you want to use this conda environment as a Jupyter Kernel,

```bash
jupyter nbextension install --py --user azureml.widgets
jupyter nbextension enable azureml.widgets --user --py

ipython kernel install --user --name synapse-aml --display-name "Python (synapse-aml)"

```

Some require installing libraries:

```bash
sudo apt-get install graphviz
```
